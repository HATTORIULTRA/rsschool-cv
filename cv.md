# Vadim Bashirov
## Contacts
* **Location:** Russia, Bashkortostan Republic, Sterlitamak
* **Phone:** +7 999 999 99 99
* **E-mail:** throwbvck@gmail.com
* **GitHub:** [HATTORIULTRA](https://github.com/HATTORIULTRA)
## About Me
I have good interpersonal skills, am an excellent team worker and very willing to learn and develop new skills.
I am reliable and dependable and often seek new responsibilities within a wide range of employment areas.
## Education
* RS School JS Course
## Skills
* HTML
* CSS
* JavaScript
* React
* Git
## Code Example
```**JavaScript**  Object with methods
const personalMovieDB = {
    count: 0,
    movies: {},
    actors: {},
    genres: [],
    privat: false,
    start: function () {
        personalMovieDB.count = +prompt('Сколько фильмов вы уже посмотрели?', '');
        while (personalMovieDB.count == '' || personalMovieDB.count == null || isNaN(personalMovieDB.count)) {
            personalMovieDB.count = +prompt('Сколько фильмов вы уже посмотрели?', '');
        }
    },
    rememberMyFilms: function () {
        for(let i = 0; i < 2; i++) {
            const a = prompt('Один из последних просмотренных фильмов?'),
                b = prompt('На сколько оцените его?');
            if(a != null && b != null && a != '' && b != '' && a.length < 50) {
                personalMovieDB.movies[a] = b;
                console.log('Done!');
            } else {
                console.log('Error!');
                i--;
            }
        }
    },
    detectPersonalLevel: function () {
        if (personalMovieDB.count < 10) {
            console.log('Просмотрено довольно мало фильмов.');
        } else if (personalMovieDB.count >= 10 && personalMovieDB.count < 30) {
            console.log('Вы классический зритель.');
        } else if (personalMovieDB.count >= 30) {
            console.log('Вы киноман.');
        } else {
            console.log('Произошла ошибка.');
        }
    },
    showMyDB: function (hidden) {
        if (!hidden) {
            console.log(personalMovieDB);
        }
    },
    toggleVisibleMyDB: function() {
        if(personalMovieDB.privat) {
            personalMovieDB.privat = false;
        } else  {
            personalMovieDB.privat = true;
        }
    },
    writeYourGenres: function () {
        for(let i = 1; i <= 3; i++) {
            let genre = prompt(`Ваш любимый жанр под номером ${i}`);

            if(genre == '' || genre == null) {
                console.log('Вы ввели некорректные данные.');
                i--;
            } else {
            personalMovieDB.genres[i - 1] = genre;
            };
        };
        personalMovieDB.genres.forEach((item, i) => {
            console.log(`Любимый жанр ${i + 1} - это ${item}`);
        });
    },
};

console.log(personalMovieDB);
```
## English
A2