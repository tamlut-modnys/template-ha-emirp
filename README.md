# `Emirp`


A prime number is a number that is only divisible by 1 and itself, for example, `7`. An [emirp](https://en.wikipedia.org/wiki/Emirp) is a prime number that results in a different prime when its decimal digits are reversed. For example, `107` and `701` are a pair of emirps, and `3,049` and `9,403`.

Palindromic numbers are not emirps.`101` is a prime and its reverse is itself -- it is not an emirp.

Your task for this challenge is write a generator that will add up all the first `n` emirps. To be precise, you should write a generator `emirp` which takes a `@ud` number `n` as an input, and returns a `@ud` number which is the sum of the first `n` emirps.

Example usage:
```
> +emirp 10
638
```

The first 10 emirps are `13, 17, 31, 37, 71, 73, 79, 97, 107, 113`, and their sum is `638`.

Two winners will be rewarded. **Fastest Solution** will go to the first person to send in a working solution. **Best Style** will be measured by a variety of factors, including clarity, elegance, following Hoon-ish conventions, being well-commented, and code runtime. For examples, see the challenges and winners from our last competition [[1]](https://docs.urbit.org/language/hoon/examples/abc-blocks) [[2]](https://docs.urbit.org/language/hoon/examples/luhn-number) [[3]](https://docs.urbit.org/language/hoon/examples/water-towers). You can also refer to the [Hoon Style Guide](https://docs.urbit.org/language/hoon/guides/style).


For submission, fill out this [google form](https://forms.gle/hDPtjPZQeEJjmxxr8) with your information. See instructions to create the repository below. Remember to make your repo private and add tamlut-modnys as a collaborator.

This challenge opens at 11am ET (8am PT, 5pm Central Europe) on Feb 17, and will close at the same time on Feb 24. Good luck!

## Using this Repository

**Please _do not fork this repository directly on GitHub._**  Instead, please use GitHub's "template" function following [the instructions below](#creating-a-repository) to copy this repository and customize it for your project.

If you are working with a fakeship, this is one way to set things up for rapid development:

1. Start a fakeship and `|mount %base`.
2. Clone this repo into the same directory as the fakeship, then copy the contents of `src/` into `zod/base/`.
3. Develop either in `zod/base/` or in this repo folder directly.  It's probably a bit easier to develop in the fakeship and copy back here frequently.

## Testing

This repo provides test cases you can use to verify that your code submission works correctly.

To run the tests, make sure you have mounted and committed the files into the `base` folder of your fake ship. Then from dojo run
```
-test %/tests/emirp/hoon
```
This will run several tests, each of which will pass or fail. For debugging help you can inspect the test code to see which ones passed and failed.

To avoid issues, make sure your generator is written in the provided file at `/gen/emirp.hoon`

For more info on testing in Hoon, see [this link](https://docs.urbit.org/userspace/apps/guides/unit-tests).

## Creating a Repository

1.  Log in to GitHub.
    (If you do not have an account, you can quickly create one for free.)
    You must be logged in for the remaining steps to work.

2.  On this page, click on the green "Use this template" button (top right)

3.  Select the owner for your new repository.
    (This will probably be you, but may instead be an organization you belong to.)

4.  Choose a name for your copy of the archetype repository.
    We recommend you call it `ha-emirp` (no 'template').

5.  Make sure the repository is **private**, leave "Include all branches" unchecked, and click on "Create repository from template". You will be redirected to your new copy of the template respository.

6.  Share the repo with tamlut-modnys on Github as a collaborator.

After this is complete, you can use this repo to handle your competition development and submission. Please note that by submitting a solution, you allow it to be made public under the MIT license.