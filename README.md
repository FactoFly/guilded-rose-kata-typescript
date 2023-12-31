# Gilded Rose Kata

We're excited to learn more about your coding skills and get to know you better! In this task, we'd like you to complete the Gilded Rose Kata, which is a programming exercise allowing you to demonstrate your problem solving and refactoring skills.

## Instructions

1. Clone this repository
2. Refactor the existing codebase to improve its maintainability and readability, while following the specifications below.
3. Record your screen while you work on the refactoring. Ensure that your face is visible in the recording.
    - You can use any recording software that you feel comfortable with. 
    - If you don't have any screen recording software already, then we suggest using [ScreenRec](https://screenrec.com/).
4. During the screen recording, explain your thought process, the changes you're making, and why you're making them. We're interested in your problem-solving skills and coding practices.
5. Try and commit your code to your repo as you go along, so that we can see a clean git history.
6. Spend at least 30 minutes on this exercise.
7. When finished, create a public GitHub repository and upload your code.

## Specification
Hi and welcome to team Gilded Rose. 

As you know, we are a small inn with a prime location in a prominent city ran by a friendly innkeeper named Allison. We also buy and sell only the finest goods. Unfortunately, our goods are constantly degrading in quality as they approach their sell by date. We have a system in place that updates our inventory for us. It was developed by a no-nonsense type named Leeroy, who has moved on to new adventures. Your task is to add the new feature to our system so that we can begin selling a new category of items. First an introduction to our system:

- All items have a SellIn value which denotes the number of days we have to sell the item
- All items have a Quality value which denotes how valuable the item is
- At the end of each day our system lowers both values for every item

Pretty simple, right? Well this is where it gets interesting:

- Once the sell by date has passed, Quality degrades twice as fast
- The Quality of an item is never negative
- “Aged Brie” actually increases in Quality the older it gets
- The Quality of an item is never more than 50
- “Sulfuras”, being a legendary item, never has to be sold or decreases in Quality
- “Backstage passes”, like aged brie, increases in Quality as it’s SellIn value approaches; Quality increases by 2 when there are 10 days or less and by 3 when there are 5 days or less but Quality drops to 0 after the concert

We have recently signed a supplier of conjured items. This requires an update to our system:

- “Conjured” items degrade in Quality twice as fast as normal items

Feel free to make any changes to the UpdateQuality method and add any new code as long as everything still works correctly. However, do not alter the Item class or Items property as those belong to the goblin in the corner who will insta-rage and one-shot you as he doesn’t believe in shared code ownership (you can make the UpdateQuality method and Items property static if you like, we’ll cover for you).

## Getting started

Install dependencies

```sh
npm install
```

## Running app
_You may need to install `ts-node`_

```sh
npx ts-node test/golden-master-text-test.ts
```

Or with number of days as args:
```sh
npx ts-node test/golden-master-text-test.ts 10
```

## Running tests

To run all tests

### Jest way

```sh
npm run test:jest
```

To run all tests in watch mode

```sh
npm run test:jest:watch
```

### Mocha way

```sh
npm run test:mocha
```
