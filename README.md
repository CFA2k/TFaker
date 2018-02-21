# TFaker 
:crystal_ball: **TFaker** is a fake data generator for Delphi/Pascal projects, inspired by [fzaninotto/Faker](https://github.com/fzaninotto/Faker) and many others, because of **test enhancements** and **time saving**.

**Feel free to contribute with your PR. :alien:**

## Usage

First, you will need to download the file <a href="https://github.com/abekroenem/TFaker/blob/master/src/Faker.pas" download>Faker.pas</a>. Then, add on **Library Path** of your Delphi, by going at **Tools** > **Options** > **Environment Options** > **Delphi Options** > **Library** > *Library Path*.


## Avaliable Methods

```pascal
  lorem = TFaker.loremIpsum();
  // "Lorem ipsum dolor sit amet [...]"

  firstName = TFaker.firstName();
  // returns an ordinary first name, e.g 'Bill', 'Adam', 'Paul'

  lastName = TFaker.lastName();
  // returns an ordinary last name, e.g 'Clark', 'Arin', 'Graham'
  
  fullName = TFaker.fullName();
  // returns an combination of TFaker.firstName and TFaker.lastName
  // e.g 'Bill Clark','Adam Arian', 'Paul Graham'
  
  userName = TFaker.userName();
  // returns an username created by using TFaker.fullName() as name generator
  // e.g 'bill_clark', 'adam2345arian', 'paul.graham'
  
  email = TFaker.email();
  customEmail = TFaker.email('my.custom.domain.io');
  // returns an random email generated by using TFaker.fullName() and some of 100 most used domains
  // or your given custom domain
  
  password = TFaker.password();
  // returns an completely random string with numbers and chars, with upper and lower case
  
  birthDate = TFaker.birthDate();
  // returns an birthdate whose age is between 0 and 100 years old
  
  thing = TFaker.thing();
  // returns an completely random thing

  otan = TFaker.otan();
  x_otan = TFaker.OTAN_ALPHABET[23]; // 23 index of 'X' ('X-ray')
  // returns an random otan Phonetic Alphabet member 
  // e.g 'Alpha', 'Quebec', 'Foxtrot'
  // or you can use directly indexing for otan alphabet, 
  // that goes from 0 (A - Alpha) to 25 (Z - Zulu)

  randomWord = TFaker.word();
  // random word

  text = TFaker.text();
  text = TFaker.text(200);
  // random text using TFaker.words() combination,
  // or a text with defined number of words

```

## License
[MIT](https://github.com/abekroenem/TFaker/blob/master/LICENSE)