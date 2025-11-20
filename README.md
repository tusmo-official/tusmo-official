# Ku soo dhawaaw Tusmo 🇸🇴


### Luuqad Compiler ah oo aad u xawaara sareysa


Waxaan dhisnay something very special. Tani waa **Tusmo**.

<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="tusmoLogo.png" alt="Tusmo Logo - Blue Eyes" width="200"/>
</p>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<i>Taasi waa wajigga dhabta ah ee <strong>Tusmo</strong>!</i></p>

### Tusmo Waa sidee?

* **Waa luuqad cusub** Tusmo waa luuqad cusub, waana luuqadda 2aad ee soomaali ah.
* Waa luuqad **Static** ah oo u baahan in la cadeeyo **datatype-keeda**.
* Waa luuqad **100% Pure Somali Syntax leh**! .
* Waa luuqad **OOP** ah 
* Waxay leedahay **design** la mid ah luuqadaha sida: **C, C++, C#, Java, iyo Typescript.**



## Tusmo syntax
**sidda loo declare-kareeyo variable-ladda nooc yadooda kala duwan (variable declaration)**
```tusmo

// variable string
keyd:eray name = "Mubaarak";

//variable int
keyd:tiro number = 06112345678;

//variable char
keyd:xaraf latter = 'A';

// boolean
keyd:miyaa diyaar = run;

//variable int array
keyd:tix:tiro numbers = [0,9,8,7,6];


//variable string array
keyd:tix:eray names = ["cabdi", "cali", "faatima"];


// dynamic array
keyd:tix isku_dhaf = ["Jimce", 0099, 'A', run];

// 2D array
keyd:tix:tix:tiro matrix = [[1, 2], [3, 4]];

// dictionary 
keyd:tix:qaamuus ardayda = [
    {"magac": "Abdixamiid", "da": 20, "kulliyad": "Mathematics"},
    {"magac": "maxamed", "da": 20, "kulliyad": "Languages"},
    {"magac": "Omar", "da": 20, "kulliyad": "Computer Science"},
    {"magac": "Abdirahim", "da": 20, "kulliyad": "IT"},
    {"magac": "Abdirisaaq", "da": 20, "kulliyad": "Software Engineering"},
    {"magac": "Abdixamiid", "da": 20, "kulliyad": "Mathematics"},
    {"magac": "maxamed", "da": 20, "kulliyad": "Languages"},
];

```
**Xaaladda (condition)**
```tusmo

keyd:tiro age = 14;

haddii(age == 18){
  qor("Waa laguu ogolaaday kamid ahaanshiyaha ");
}ama_haddii(age == 15){
  qor("Waa laguu ogolaaday kamid ahaanshiyaha ");
}haddii_kale{
  qor("laguu ma ogolo kamid ahaanshiyaha madaama adan ahayn 18 jir ama 15 jir");
}

```
**Function**
```tusmo
// function

shaqo show_name() => {
  qor("mubaarak ");
}



// function with parameter

shaqo greeting(name:eray){
  qor($"waa ku salaamnay!, {name}");
}
qor(greeting("Mubaarak"));
```
**Loops**
```
// For loop
soco i laga bilaabo 0..100{
  qor(i,"\n");
}qor("Done !"); 
//output
0
1
2
...
99

// for each
keyd:tix:tiro n = [100, 200, 300];

soco mid kasta laga helo n {
    qor(mid);
}

//output
100
200
300


// While loop
keyd:tiro a = 0;
inta ay (a < 100) {
  qor(a);
  a = a + 1;
}
//output
0
1
2
3
..
99


// do while loop
keyd:tiro a = 0;
samay {
  qor(a);
  a = a + 1;
} inta ay (a > 100);
//output
0
1
2
3
..
99

```

**Koox (class)**
```tusmo
//class

koox Qof {
    // Xubnaha (Members)
    keyd: eray magac;
    keyd: tiro da;

    // Dhisaha (Constructor)
    dhis(m: eray, d: tiro) : waxbo {
        kan.magac = m;
        kan.da = d;
    }

    // shaqaalaha (Method)
    shaqo hadal() : waxbo {
        qor("Magacaygu waa ", kan.magac, ", waxaan jiraa ", kan.da, " sano.");
    }
}



qor("Abuurista  qof1...");
keyd: Qof qof1 = Qof("Axmed", 25) cusub;

qor("Abuurista  qof2...");
keyd: Qof qof2 = Qof("Caasha", 30) cusub;

qof1.hadal(); // Wuxuu daabacayaa macluumaadka Axmed
qof2.hadal(); // Wuxuu daabacayaa macluumaadka Caasha

qor("Da'da Axmed waa: ", qof1.da);
```
## tusmo built-in-functions qaar kamid ah

**gali**
```tusmo
//gali waa buil-in-functions ka mid ah tusmo kaas oo loo isticmaalo in xog lagu galiyo array/list

keyd:tix:tiro numbers = [0,9,8,7,6];
numbers.gali(30);

qor(numbers) // [0,9,8,7,6,30];

```

**tix_cayiman**
```tusmo
// tix_cayim waa built-in-fn kaas oo siinaya array/list size cayiman

keyd:tix:tiro my_list = tix_cayiman(5);
my_list.gali(4);
my_list.gali(3);
my_list.gali(43);
my_list.gali(443);

qor(my_list);

```

**dherer**
```tusmo
keyd:tix:tiro numbers = [0,9,8,7,6];

qor(dherer(numbers)); // output: 5

```
**nooc**
```tusmo
keyd:tiro n = 4;
qor(nooc(n)); // output: tiro
```
**eray**
```tusmo
keyd:tiro t = 123;
keyd:eray ubadal_eray = eray(t);
qor(nooc(ubaddal_eray)); //output: eray
```

**tiro**
```tusmo
keyd:eray e = "456";
keyd:eray ubadal_tiro = eray(e);
qor(nooc(ubaddal_tiro)); //output: tiro
```


**jajab**
```tusmo
keyd:eray t = 33;
keyd:eray ubadal_jajab = jajab(e);
qor(nooc(ubaddal_jajab)); //output: jajab
```

**miyaa**
```tusmo
keyd:miyaa run_miyaa = miyaa(100);
keyd:miyaa been_miyaa = miyaa(0);

qor(run_miyaa); //outpput: run
qor(been_miyaa); //output: been
```


## tusmo waxay leedahay import module 

**add.tus**
```tusmo
shaqo add(n1:tiro, n2:tiro) => tiro{
  soo_celi n1+n2;
}

```

**main.tus**
```tusmo
// import == keen

keen "add.tus";
qor(add(12,12));//output: 24
```

## Stdlib

**os**

    - halkee 
    - u_guur 
    - itus
    - abuur_folder
    - tirtir_* 
    - majiraa
    - fayl_miyaa
    - folder_miyaa
    - hel_deegaan 
    - deji_deegaan
    - fuli
    - koobi/nuqul
    - u_dhaqaaji
    - aqri_fayl
    - qor_fayl
    - isku_dar_waddo
    - cabbir_fayl

```tusmo
//test os code




```

### 🚧 Under Construction!

Tusmo Waxaa lagu dhameeyay dhisideedda **90%**

**La soco** Filo Goor dhow.

---
*Waxaa lagu sameeyay si ❤️ leh*
