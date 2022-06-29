### How to console.log....

I honestly was looking for so long, on how to have my terminal return the doubled numbers. I kept writing console.log(doubledNumbers), only to get it undefined consistently...

Finally, I actually found a site that had a code snippet that would be more straight forward...not inputting the code into an html or calling it by document.

It's honestly ridiculous to me that it took so long looking in Google, "how to console.log a function", "how to call a function", "how to...", you get gist 🤦🏻‍♂️

        const numbers = [1, 2, 4, 2];
        numbers.forEach((number) => {
        const message = number _ 2;
        console.log(message);
        });
        const doubled = numbers.map((number) => number _ 2);
        console.log(doubled);
