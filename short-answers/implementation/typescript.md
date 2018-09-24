# Typescript (10-15 mins)

1. Explain why this code does not compile (it runs fine in JavaScript):

```
    class Animal {
      isAnimal: true
      makeNoise() {
        return 'noise'
      }
    }
    class Bird extends Animal {
      isBird: true
      makeNoise() {
        return 'chirp'
      }
    }
    const checkBird = (bird: Animal|Bird) => {
      return bird.isBird
    }
```

2. Change checkBird to a _type guard_ function
3. Explain the difference between a type assertion and a type annotation
