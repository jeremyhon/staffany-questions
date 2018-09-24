# Testing (5-10 mins)

This is some code written in Typescript. It fetches a user and times out automatically after a provided number of milliseconds.

    const getUserOrTimeout = async (
      id: string,
      milliseconds: number = 1000,
    ): Promise<User | null> => {
      return new Promise<User | null>(async (resolve, reject) => {
        const timeout = setTimeout(() => resolve(null), milliseconds)
        const userOrError = await getUser(id)
        if (userOrError instanceof Error) {
          return reject(userOrError)
        }
        resolve(userOrError)
        clearTimeout(timeout)
      })
    }

Write a test that tests this function. Your test should cover the code path that involves the timeout (you don’t need to cover the other code paths).
