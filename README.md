# Portakal


R version 4.1.1 (2021-08-10) -- "Kick Things"
Copyright (C) 2021 The R Foundation for Statistical Computing
Platform: x86_64-w64-mingw32/x64 (64-bit)

R is free software and comes with ABSOLUTELY NO WARRANTY.
You are welcome to redistribute it under certain conditions.
Type 'license()' or 'licence()' for distribution details.

R is a collaborative project with many contributors.
Type 'contributors()' for more information and
'citation()' on how to cite R or R packages in publications.

Type 'demo()' for some demos, 'help()' for on-line help, or
'help.start()' for an HTML browser interface to help.
Type 'q()' to quit R.

[Workspace loaded from C:/Users/buseceker/OneDrive/Desktop/.RData]

> getwd()
> setwd("C:\Users\buseceker\OneDrive\Desktop") 
> list.files()

 [1] "Arama Listesi2.xlsx"               "Belediyeler.xlsx"                 
 [3] "Broşür.docx"                       "capture-20211028-114348 (003).png"
 [5] "capture-20211028-114348.png"       "desktop.ini"                      
 [7] "Doğalgaz.xlsx"                     "e ticaret.docx"                   
 [9] "endustri 4.0.docx"                 "ermanHoca.docx"                   
[11] "Fabrikalar.xlsx"                   "Fabrikalar2.xlsx"                 
[13] "fotoro"                            "İHBAR.docx"                       
[15] "IMG_5213.jpeg"                     "kemalHoca.docx"                   
[17] "mail.docx"                         "mesafeli-sozlesme.pdf"            
[19] "Mezun Belgesi.pdf"                 "Microsoft Teams.lnk"              
[21] "photothumb.db"                     "pom"                              
[23] "pom.docx"                          "portakal.csv"                     
[25] "proasist online market.docx"       "sgk-tescil-ve-hizmet-dokumu.pdf"  
[27] "Tesis Yönetim.xlsx"                "TMS Bilgilendirme Maili.docx"     
[29] "TMS script.txt"                    "Transkript.pdf"                   
[31] "WhatsApp.lnk"                      "yeni script.txt"                  
[33] "Zoom.lnk"                         
> veri <-read.csv("portakal.csv")
> veri
    portakal
1     134.85
2     128.25
3     191.37
4     171.66
5     131.34
6     156.22
7     113.09
8     152.47
9     133.63
10    185.49
11    128.56
12    130.32
13    131.00
14    134.83
15     89.64
16    120.35
17    113.21
18    146.26
19     93.48
20    142.35
21    152.16
22     55.17
23     89.16
24    143.02
25    130.59
26    173.20
27    127.47
28    130.41
29    106.41
30    116.22
31     95.93
32    161.71
33    128.25
34    132.24
35    122.74
36    141.02
37    145.16
38     94.69
39    124.54
40    151.00
41    157.93
42    141.35
43    109.37
44    144.70
45    157.27
46    187.30
47    111.64
48    158.17
49    143.18
50    158.80
51    161.85
52    138.71
53    205.09
54    140.41
55    102.46
56    177.73
57    122.32
58    172.74
59    141.90
60     94.35
61    116.69
62     90.24
63    159.93
64    122.66
65    120.00
66    164.35
67    124.04
68    154.28
69    179.03
70    115.87
71    128.71
72    159.34
73    158.02
74    116.22
75    171.15
76    138.99
77    102.13
78    193.45
79    146.16
80    145.64
81    111.24
82    144.01
83    139.08
84    175.61
85    167.15
86    116.43
87    116.09
88    111.96
89    130.90
90    152.57
91    158.17
92    131.55
93    150.01
94    115.07
95    125.28
96    161.62
97    146.55
98    128.10
99    144.44
100   142.41
> mean(veri$portakal)
[1] 137.5187
> median(veri$portakal)
[1] 138.85
> quantile(veri$portakal, c(.32, .57, .98))
     32%      57%      98% 
126.7692 142.3758 191.4116 
> quantile(veri$portakal)
      0%      25%      50%      75%     100% 
 55.1700 120.2625 138.8500 156.4825 205.0900 
> IQR(veri$portakal)
[1] 36.22
> var(veri$portakal)
[1] 691.6942
> sd(veri$portakal)
[1] 26.30008
> skewness(veri$portakal)
Error in skewness(veri$portakal) : could not find function "skewness"
> boxplot(veri$portakal, horizontal=TRUE)

