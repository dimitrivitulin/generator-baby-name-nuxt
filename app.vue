<script setup lang="ts">
interface Name {
  id: number;
  name: string;
  gender: Gender;
  popularity: Popularity;
  length: Length;
}

 enum Gender {
  GIRL = "Girl",
  BOY = "Boy",
  UNISEX = "Unisex",
}

 enum Popularity {
  TRENDY = "Trendy",
  UNIQUE = "Unique",
  NORMAL = "Normal"
}

 enum Length {
  SHORT = "Short",
  LONG = "Long",
  ALL = "All",
}

interface OptionsState {
        gender: Gender;
        popularity : Popularity;
        length : Length;
}

const options = reactive<OptionsState>({
        gender : Gender.GIRL,
        popularity :Popularity.TRENDY,
        length : Length.ALL,

});

 const names: Name[] = [
  {
    id: 2,
    name: "Jake",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 4,
    name: "Abraham",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 5,
    name: "Barthelemy",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 6,
    name: "Noah",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 7,
    name: "Benjamin",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 8,
    name: "William",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 9,
    name: "Lucius",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 10,
    name: "Harrison",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 11,
    name: "Selma",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 12,
    name: "Asher",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 13,
    name: "Tucker",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },

  {
    id: 14,
    name: "Arya",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 15,
    name: "Olivia",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 16,
    name: "Fay",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 17,
    name: "Brooklyn",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 18,
    name: "Genevieve",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 19,
    name: "Zoe",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 20,
    name: "Valentina",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 21,
    name: "Joséphine",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 22,
    name: "Maya",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 27,
    name: "Jude",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 28,
    name: "Adrien",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 29,
    name: "Sunny",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 30,
    name: "Channing",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 33,
    name: "Zephyr",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 34,
    name: "Tery",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 35,
    name: "Damien",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 36,
    name: "Enzo",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 37,
    name: "Robert",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 38,
    name: "Alain",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 39,
    name: "Didier",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 40,
    name: "Julien",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 41,
    name: "Jules",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 42,
    name: "Diego",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 43,
    name: "Dimitri",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 44,
    name: "Louis",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 45,
    name: "Hugo",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 46,
    name: "Nathan ",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 47,
    name: "Paul",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 48,
    name: "Maceo",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 49,
    name: "Rudy ",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 50,
    name: "Guy",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 51,
    name: "Gauthier",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 52,
    name: "Jimmy",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 53,
    name: "Yohan",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 54,
    name: "Johan(ne)",
    gender: Gender.UNISEX,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 55,
    name: "Jonathan",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 56,
    name: "Ritchie",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 57,
    name: "Rony",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 58,
    name: "Roméo",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 59,
    name: "Lucien",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 60,
    name: "Lucius ",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 61,
    name: "Lothaire",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 62,
    name: "Alan",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 63,
    name: "Nolan",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 64,
    name: "Maxence ",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 65,
    name: "Maxime",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 66,
    name: "Nawafel",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 67,
    name: "Théo",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 68,
    name: "Quentin",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 69,
    name: "Corentin",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 70,
    name: "Guillaume",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 71,
    name: "Dorian",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 72,
    name: "Baptiste",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 73,
    name: "Tiego",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 74,
    name: "Kanan",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 75,
    name: "Luc",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 76,
    name: "Jean-Marie",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 77,
    name: "Jean-Edouard",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 78,
    name: "Jean-Philippe",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 79,
    name: "Jean-Louis",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 80,
    name: "Philippe",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 81,
    name: "Marc",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 82,
    name: "Matthieu",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 83,
    name: "Teddy",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 84,
    name: "Ted",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 85,
    name: "Teddy",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 86,
    name: "Léonard",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 87,
    name: "Bastien",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 88,
    name: "Grégoire",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 89,
    name: "Grégory",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 90,
    name: "Brian",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 91,
    name: "Julian",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 92,
    name: "Xavier",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 93,
    name: "Jérémie",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 94,
    name: "Jorah",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 95,
    name: "Othniel ",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 96,
    name: "Eliott",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 97,
    name: "Alexandre ",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 98,
    name: "Alex",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 99,
    name: "Aldo",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 100,
    name: "Albert",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 101,
    name: "Norbert",
    gender: Gender.BOY,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 102,
    name: "Kevin",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 103,
    name: "James",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 104,
    name: "Luther",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 105,
    name: "Martin",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 106,
    name: "Marceau",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 107,
    name: "Eddie",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 108,
    name: "Olivier",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 109,
    name: "Lucien",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 110,
    name: "Kylian",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 111,
    name: "Karim",
    gender: Gender.BOY,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 112,
    name: "Tim",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 113,
    name: "Timothée",
    gender: Gender.BOY,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 114,
    name: "Lia",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 115,
    name: "Julie",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 116,
    name: "Juliette",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 117,
    name: "Marie",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 119,
    name: "Marilyn",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  
  {
    id: 120,
    name: "Marie-Ange",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 121,
    name: "Marie-Pierre",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 122,
    name: "Marie-France",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 123,
    name: "Mathilde",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 124,
    name: "Laura",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 125,
    name: "Laure",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 126,
    name: "Florence",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 127,
    name: "Louise",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 128,
    name: "Huguette",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 129,
    name: "Alison",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 131,
    name: "Cindy",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 132,
    name: "Léa ",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 133,
    name: "Ornella",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 134,
    name: "Chloé",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 135,
    name: "Ornella",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 136,
    name: "Léna",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 135,
    name: "Lola",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 136,
    name: "Océane",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 137,
    name: "Amandine",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 138,
    name: "Melina",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 139,
    name: "Tiphaine",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 140,
    name: "Audrey",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 141,
    name: "Serena",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 142,
    name: "Maria",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 143,
    name: "Elena",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 144,
    name: "Eglantine",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 145,
    name: "Constance",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 146,
    name: "Gwendoline",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 147,
    name: "Nina",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 148,
    name: "Lisette",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 149,
    name: "Ruth",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 150,
    name: "Esther",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 151,
    name: "Ida",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 152,
    name: "Mélissa",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 153,
    name: "Aurore",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 154,
    name: "Manon",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 155,
    name: "Ilona",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 156,
    name: "Alicia",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 157,
    name: "Alice",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 158,
    name: "Sacha",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 159,
    name: "Ondine",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 160,
    name: "Anna",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 161,
    name: "Arielle",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 162,
    name: "Salmina",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 163,
    name: "Loïs",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 164,
    name: "Laetitia",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 165,
    name: "Désiré(e)",
    gender: Gender.UNISEX,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 166,
    name: "Carmen",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 167,
    name: "Nadège",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 168,
    name: "Nathalie",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 169,
    name: "Nathalia",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 170,
    name: "Xena",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 171,
    name: "Vénus",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 172,
    name: "Rose",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 173,
    name: "Lila",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 174,
    name: "Kim",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 175,
    name: "Charlotte",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 176,
    name: "Emma",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 177,
    name: "Émeline",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 178,
    name: "Émeraude",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 179,
    name: "Émy",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 180,
    name: "Elizabeth",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 181,
    name: "Virginie",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 182,
    name: "Manuela",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 183,
    name: "Élodie",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 184,
    name: "Sophie",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 185,
    name: "Olivia",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 186,
    name: "Olive",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 187,
    name: "Sophia",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 188,
    name: "Sarah",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 189,
    name: "Inès",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 190,
    name: "Stacy",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 191,
    name: "Clotilde",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 192,
    name: "Céline",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 193,
    name: "Christelle",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 194,
    name: "Manoah",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 195,
    name: "Shana",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 196,
    name: "Hélène",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 197,
    name: "Morgane",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 198,
    name: "Mégane",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 199,
    name: "Meg",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 200,
    name: "Lilou",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 201,
    name: "Marion",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 202,
    name: "Marine",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 203,
    name: "Juliana",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 204,
    name: "Maeva",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 205,
    name: "Eva",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 206,
    name: "Grace",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 207,
    name: "Cannelle",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 208,
    name: "Prisca",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 209,
    name: "Fanny",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 209,
    name: "Stéphanie",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 210,
    name: "Lucie",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 211,
    name: "Lucile",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 212,
    name: "Luce",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 213,
    name: "Camomille",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 214,
    name: "Ambre",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 215,
    name: "Alma",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 216,
    name: "Ada",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 217,
    name: "Alexia",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.LONG,
  },
  {
    id: 218,
    name: "Trixia",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 219,
    name: "Théa",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 220,
    name: "Tina",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 221,
    name: "Beckie",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 222,
    name: "Ashley",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 223,
    name: "Shurley",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 224,
    name: "Amanda",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 225,
    name: "Eléonore",
    gender: Gender.GIRL,
    popularity: Popularity.UNIQUE,
    length: Length.LONG,
  },
  {
    id: 226,
    name: "Ella",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 227,
    name: "Ève",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 228,
    name: "Isabelle",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 229,
    name: "Isabella",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 230,
    name: "Bella",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 231,
    name: "Ninon",
    gender: Gender.GIRL,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  {
    id: 232,
    name: "Maude",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 233,
    name: "Aude",
    gender: Gender.GIRL,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 234,
    name: "Camille",
    gender: Gender.UNISEX,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 235,
    name: "Gabriel(le)",
    gender: Gender.UNISEX,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 236,
    name: "Dominique",
    gender: Gender.UNISEX,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 237,
    name: "Frédéric(que)",
    gender: Gender.UNISEX,
    popularity: Popularity.NORMAL,
    length: Length.LONG,
  },
  {
    id: 238,
    name: "Michel(le)",
    gender: Gender.UNISEX,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 239,
    name: "Pascal(e)",
    gender: Gender.UNISEX,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 240,
    name: "Aimé(e)",
    gender: Gender.UNISEX,
    popularity: Popularity.UNIQUE,
    length: Length.SHORT,
  },
  {
    id: 241,
    name: "René(e)",
    gender: Gender.UNISEX,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 242,
    name: "Claude",
    gender: Gender.UNISEX,
    popularity: Popularity.NORMAL,
    length: Length.SHORT,
  },
  {
    id: 243,
    name: "Joyce",
    gender: Gender.UNISEX,
    popularity: Popularity.TRENDY,
    length: Length.SHORT,
  },
  
];
  
const computeSelectedNames = () =>{
  const filteredNames = names
    .filter((name) => name.gender === options.gender )
    .filter((name) => name.popularity === options.popularity)
    .filter((name) => {
      if(options.length === Length.ALL) return true
      else return name.length === options.length
    })
    selectedNames.value = filteredNames.map((name) => name.name);
}
const selectedNames = ref<string[]>([]);

</script>
<template>
  <div class="container">
    <h1>Générateur de Noms de Bébé </h1>
    <p>Trouvez un Nom pour votre futur Bébé</p>
    <div class="options-container">
      <div class="option-container">
        <h4>Choisissez un genre</h4>
        <div class="option-buttons">
          <button class="option" 
          :class="options.gender === Gender.BOY && 'option-active'"
          @click="options.gender = Gender.BOY" 
          >Garçon</button>
          <button class="option" 
          :class="options.gender === Gender.GIRL && 'option-active'"
          @click="options.gender = Gender.GIRL" 
          >Fille</button>
          <button class="option" 
          :class="options.gender === Gender.UNISEX && 'option-active'"
          @click="options.gender = Gender.UNISEX" 
          >Unisexe</button>
        </div>
      </div>
      <div class="option-container">
         <h4>Popularité du Nom</h4>
        <div class="option-buttons">
          <button class="option" 
          :class="options.popularity === Popularity.TRENDY && 'option-active'"
          @click="options.popularity = Popularity.TRENDY" 
          >Hype</button>
          <button class="option" 
          :class="options.popularity === Popularity.NORMAL && 'option-active'"
          @click="options.popularity = Popularity.NORMAL" 
          >Commun</button>
          <button class="option" 
          :class="options.popularity === Popularity.UNIQUE && 'option-active'"
          @click="options.popularity = Popularity.UNIQUE" 
          >Original</button>
        </div>
      </div>
      <div class="option-container">
         <h4>Longueur du nom</h4>
        <div class="option-buttons">
          <button class="option" 
          :class="options.length === Length.LONG && 'option-active'"
          @click="options.length = Length.LONG"
          >Long</button>
          <button class="option" 
          :class="options.length === Length.SHORT && 'option-active'"
          @click="options.length = Length.SHORT"
          >Court</button>
          <button class="option" 
          :class="options.length === Length.ALL && 'option-active'"
          @click="options.length = Length.ALL"
          >Tous</button>
        </div>
      <button class="primary" @click="computeSelectedNames">Choisir un Nom</button>
      </div>
    </div>
      <div class="cards-container">
        <div v-for="name in selectedNames" :key="name" class="card">
          <img src="./assets/baby_name.png" alt="">
           <p >{{name}}</p>
        </div>
      </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Asap:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,700&display=swap');
*,::before,::after{
margin: 0;
padding: 0;
box-sizing: border-box;
}
body{
  margin: 0!important;
  padding: 0!important;
  box-sizing: border-box;
}
.container{
    font-family: Arial, Helvetica, sans-serif;
    color:#B7DAEB;
    background: rgb(252,252,248);
    background: linear-gradient(180deg, rgba(252,252,248,1) 31%, rgba(240,240,240,1) 94%);
    max-width: 600px;
    margin: 30px auto;
    text-align: center;
    border: 2px solid #83cae86a;
    border-radius: 20px 20px 60px 60px;
    box-shadow: 5px 5px 20px #f5c5a8c8;
  }
.options-container{
  background-color: #F4F5F0;
}

h1{
  font-family:'Asap', sans-serif;
  font-size: 2.5rem;
  padding: 30px 0;
}
p{
  font-family:system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif ;
  font-weight: 500;
}
h4{
  font-size: 1.75rem;
  color:#fff;
  font-family: 'Asap', sans-serif;
  font-weight: 500;
  font-style: italic;
}
.container p{
  padding-bottom: 30px;
}
.options-container{
  background-color: #EA9C91;
  padding: 25px 0;
  border-radius: 0 0 60px 60px ;
  display: flex;
  flex-direction: column;
  gap: 20px;
  box-shadow: inset -5px -5px 10px rgba(255, 255, 255, 0.367);
}
.option-buttons{
  padding: 30px 0;
}

button{
  border: none;
  outline: none;
  width: 110px;
  border-radius: 15px;
  padding: 10px 15px;
  margin: 0 10px;
  transition:linear .2s ;
  cursor: pointer;
  font-family:system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif ;
  font-weight: 500;
  box-shadow: 3px 3px 15px rgba(128, 128, 128, 0.31);
}
.option-active{
 outline:1px solid linen;
 transform: scale(1.1);
 background-color: #B7DAEB;
 color: #fff;
  box-shadow: 3px 4px 20px rgba(128, 128, 128, 0.651);
}

.primary{
  background-color: crimson;
  color: #fff;
  border-radius: 15px;
  border: none;
  padding: 15px 20px;
  margin-top: 20px;
  cursor: pointer;
  width: 150px;
}
.cards-container{
  display: flex;
  flex-wrap: wrap;
  padding: 0 65px;
  gap:15px;

}
.card{
  width: 100px;
  height: 150px;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
}
.card img{
  width: 100%;
  position: absolute;
}
.card p{
  color:#fff;
  padding: 5px;
  border-radius: 10px;
  background-color: #F4B58E;
    z-index: 10;
}


</style>
