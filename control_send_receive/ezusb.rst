                                      1 ;--------------------------------------------------------
                                      2 ; File Created by SDCC : free open source ANSI-C Compiler
                                      3 ; Version 4.0.0 #11528 (Linux)
                                      4 ;--------------------------------------------------------
                                      5 	.module ezusb
                                      6 	.optsdcc -mmcs51 --model-small
                                      7 	
                                      8 ;--------------------------------------------------------
                                      9 ; Public variables in this module
                                     10 ;--------------------------------------------------------
                                     11 	.globl _main
                                     12 	.globl _EIPX6
                                     13 	.globl _EIPX5
                                     14 	.globl _EIPX4
                                     15 	.globl _PI2C
                                     16 	.globl _PUSB
                                     17 	.globl _EIEX6
                                     18 	.globl _EIEX5
                                     19 	.globl _EIEX4
                                     20 	.globl _EI2C
                                     21 	.globl _EUSB
                                     22 	.globl _SMOD1
                                     23 	.globl _ERESI
                                     24 	.globl _RESI
                                     25 	.globl _INT6
                                     26 	.globl _CY
                                     27 	.globl _AC
                                     28 	.globl _F0
                                     29 	.globl _RS1
                                     30 	.globl _RS0
                                     31 	.globl _OV
                                     32 	.globl _FL
                                     33 	.globl _P
                                     34 	.globl _TF2
                                     35 	.globl _EXF2
                                     36 	.globl _RCLK
                                     37 	.globl _TCLK
                                     38 	.globl _EXEN2
                                     39 	.globl _TR2
                                     40 	.globl _C_T2
                                     41 	.globl _CP_RL2
                                     42 	.globl _SM01
                                     43 	.globl _SM11
                                     44 	.globl _SM21
                                     45 	.globl _REN1
                                     46 	.globl _TB81
                                     47 	.globl _RB81
                                     48 	.globl _TI1
                                     49 	.globl _RI1
                                     50 	.globl _PS1
                                     51 	.globl _PT2
                                     52 	.globl _PS0
                                     53 	.globl _PT1
                                     54 	.globl _PX1
                                     55 	.globl _PT0
                                     56 	.globl _PX0
                                     57 	.globl _PD7
                                     58 	.globl _PD6
                                     59 	.globl _PD5
                                     60 	.globl _PD4
                                     61 	.globl _PD3
                                     62 	.globl _PD2
                                     63 	.globl _PD1
                                     64 	.globl _PD0
                                     65 	.globl _EA
                                     66 	.globl _ES1
                                     67 	.globl _ET2
                                     68 	.globl _ES0
                                     69 	.globl _ET1
                                     70 	.globl _EX1
                                     71 	.globl _ET0
                                     72 	.globl _EX0
                                     73 	.globl _PC7
                                     74 	.globl _PC6
                                     75 	.globl _PC5
                                     76 	.globl _PC4
                                     77 	.globl _PC3
                                     78 	.globl _PC2
                                     79 	.globl _PC1
                                     80 	.globl _PC0
                                     81 	.globl _SM0
                                     82 	.globl _SM1
                                     83 	.globl _SM2
                                     84 	.globl _REN
                                     85 	.globl _TB8
                                     86 	.globl _RB8
                                     87 	.globl _TI
                                     88 	.globl _RI
                                     89 	.globl _PB7
                                     90 	.globl _PB6
                                     91 	.globl _PB5
                                     92 	.globl _PB4
                                     93 	.globl _PB3
                                     94 	.globl _PB2
                                     95 	.globl _PB1
                                     96 	.globl _PB0
                                     97 	.globl _TF1
                                     98 	.globl _TR1
                                     99 	.globl _TF0
                                    100 	.globl _TR0
                                    101 	.globl _IE1
                                    102 	.globl _IT1
                                    103 	.globl _IE0
                                    104 	.globl _IT0
                                    105 	.globl _PA7
                                    106 	.globl _PA6
                                    107 	.globl _PA5
                                    108 	.globl _PA4
                                    109 	.globl _PA3
                                    110 	.globl _PA2
                                    111 	.globl _PA1
                                    112 	.globl _PA0
                                    113 	.globl _EIP
                                    114 	.globl _B
                                    115 	.globl _EIE
                                    116 	.globl _ACC
                                    117 	.globl _EICON
                                    118 	.globl _PSW
                                    119 	.globl _TH2
                                    120 	.globl _TL2
                                    121 	.globl _RCAP2H
                                    122 	.globl _RCAP2L
                                    123 	.globl _T2CON
                                    124 	.globl _SBUF1
                                    125 	.globl _SCON1
                                    126 	.globl _GPIFSGLDATLNOX
                                    127 	.globl _GPIFSGLDATLX
                                    128 	.globl _GPIFSGLDATH
                                    129 	.globl _GPIFTRIG
                                    130 	.globl _EP01STAT
                                    131 	.globl _IP
                                    132 	.globl _OEE
                                    133 	.globl _OED
                                    134 	.globl _OEC
                                    135 	.globl _OEB
                                    136 	.globl _OEA
                                    137 	.globl _IOE
                                    138 	.globl _IOD
                                    139 	.globl _AUTOPTRSETUP
                                    140 	.globl _EP68FIFOFLGS
                                    141 	.globl _EP24FIFOFLGS
                                    142 	.globl _EP2468STAT
                                    143 	.globl _IE
                                    144 	.globl _INT4CLR
                                    145 	.globl _INT2CLR
                                    146 	.globl _IOC
                                    147 	.globl _AUTOPTRL2
                                    148 	.globl _AUTOPTRH2
                                    149 	.globl _AUTOPTRL1
                                    150 	.globl _AUTOPTRH1
                                    151 	.globl _SBUF0
                                    152 	.globl _SCON0
                                    153 	.globl _MPAGE
                                    154 	.globl _EXIF
                                    155 	.globl _IOB
                                    156 	.globl _SPC_FNC
                                    157 	.globl _CKCON
                                    158 	.globl _TH1
                                    159 	.globl _TH0
                                    160 	.globl _TL1
                                    161 	.globl _TL0
                                    162 	.globl _TMOD
                                    163 	.globl _TCON
                                    164 	.globl _PCON
                                    165 	.globl _DPS
                                    166 	.globl _DPH1
                                    167 	.globl _DPL1
                                    168 	.globl _DPH
                                    169 	.globl _DPL
                                    170 	.globl _SP
                                    171 	.globl _IOA
                                    172 	.globl _GPCR2
                                    173 	.globl _ECC2B2
                                    174 	.globl _ECC2B1
                                    175 	.globl _ECC2B0
                                    176 	.globl _ECC1B2
                                    177 	.globl _ECC1B1
                                    178 	.globl _ECC1B0
                                    179 	.globl _ECCRESET
                                    180 	.globl _ECCCFG
                                    181 	.globl _EP8FIFOBUF
                                    182 	.globl _EP6FIFOBUF
                                    183 	.globl _EP4FIFOBUF
                                    184 	.globl _EP2FIFOBUF
                                    185 	.globl _EP1INBUF
                                    186 	.globl _EP1OUTBUF
                                    187 	.globl _EP0BUF
                                    188 	.globl _CT4
                                    189 	.globl _CT3
                                    190 	.globl _CT2
                                    191 	.globl _CT1
                                    192 	.globl _USBTEST
                                    193 	.globl _TESTCFG
                                    194 	.globl _DBUG
                                    195 	.globl _UDMACRCQUAL
                                    196 	.globl _UDMACRCL
                                    197 	.globl _UDMACRCH
                                    198 	.globl _GPIFHOLDAMOUNT
                                    199 	.globl _FLOWSTBHPERIOD
                                    200 	.globl _FLOWSTBEDGE
                                    201 	.globl _FLOWSTB
                                    202 	.globl _FLOWHOLDOFF
                                    203 	.globl _FLOWEQ1CTL
                                    204 	.globl _FLOWEQ0CTL
                                    205 	.globl _FLOWLOGIC
                                    206 	.globl _FLOWSTATE
                                    207 	.globl _GPIFABORT
                                    208 	.globl _GPIFREADYSTAT
                                    209 	.globl _GPIFREADYCFG
                                    210 	.globl _XGPIFSGLDATLNOX
                                    211 	.globl _XGPIFSGLDATLX
                                    212 	.globl _XGPIFSGLDATH
                                    213 	.globl _EP8GPIFTRIG
                                    214 	.globl _EP8GPIFPFSTOP
                                    215 	.globl _EP8GPIFFLGSEL
                                    216 	.globl _EP6GPIFTRIG
                                    217 	.globl _EP6GPIFPFSTOP
                                    218 	.globl _EP6GPIFFLGSEL
                                    219 	.globl _EP4GPIFTRIG
                                    220 	.globl _EP4GPIFPFSTOP
                                    221 	.globl _EP4GPIFFLGSEL
                                    222 	.globl _EP2GPIFTRIG
                                    223 	.globl _EP2GPIFPFSTOP
                                    224 	.globl _EP2GPIFFLGSEL
                                    225 	.globl _GPIFTCB0
                                    226 	.globl _GPIFTCB1
                                    227 	.globl _GPIFTCB2
                                    228 	.globl _GPIFTCB3
                                    229 	.globl _GPIFADRL
                                    230 	.globl _GPIFADRH
                                    231 	.globl _GPIFCTLCFG
                                    232 	.globl _GPIFIDLECTL
                                    233 	.globl _GPIFIDLECS
                                    234 	.globl _GPIFWFSELECT
                                    235 	.globl _SETUPDAT
                                    236 	.globl _SUDPTRCTL
                                    237 	.globl _SUDPTRL
                                    238 	.globl _SUDPTRH
                                    239 	.globl _EP8FIFOBCL
                                    240 	.globl _EP8FIFOBCH
                                    241 	.globl _EP6FIFOBCL
                                    242 	.globl _EP6FIFOBCH
                                    243 	.globl _EP4FIFOBCL
                                    244 	.globl _EP4FIFOBCH
                                    245 	.globl _EP2FIFOBCL
                                    246 	.globl _EP2FIFOBCH
                                    247 	.globl _EP8FIFOFLGS
                                    248 	.globl _EP6FIFOFLGS
                                    249 	.globl _EP4FIFOFLGS
                                    250 	.globl _EP2FIFOFLGS
                                    251 	.globl _EP8CS
                                    252 	.globl _EP6CS
                                    253 	.globl _EP4CS
                                    254 	.globl _EP2CS
                                    255 	.globl _EP1INCS
                                    256 	.globl _EP1OUTCS
                                    257 	.globl _EP0CS
                                    258 	.globl _EP8BCL
                                    259 	.globl _EP8BCH
                                    260 	.globl _EP6BCL
                                    261 	.globl _EP6BCH
                                    262 	.globl _EP4BCL
                                    263 	.globl _EP4BCH
                                    264 	.globl _EP2BCL
                                    265 	.globl _EP2BCH
                                    266 	.globl _EP1INBC
                                    267 	.globl _EP1OUTBC
                                    268 	.globl _EP0BCL
                                    269 	.globl _EP0BCH
                                    270 	.globl _FNADDR
                                    271 	.globl _MICROFRAME
                                    272 	.globl _USBFRAMEL
                                    273 	.globl _USBFRAMEH
                                    274 	.globl _TOGCTL
                                    275 	.globl _WAKEUPCS
                                    276 	.globl _SUSPEND
                                    277 	.globl _USBCS
                                    278 	.globl _XAUTODAT2
                                    279 	.globl _XAUTODAT1
                                    280 	.globl _I2CTL
                                    281 	.globl _I2DAT
                                    282 	.globl _I2CS
                                    283 	.globl _PORTECFG
                                    284 	.globl _PORTCCFG
                                    285 	.globl _PORTACFG
                                    286 	.globl _INTSETUP
                                    287 	.globl _INT4IVEC
                                    288 	.globl _INT2IVEC
                                    289 	.globl _CLRERRCNT
                                    290 	.globl _ERRCNTLIM
                                    291 	.globl _USBERRIRQ
                                    292 	.globl _USBERRIE
                                    293 	.globl _GPIFIRQ
                                    294 	.globl _GPIFIE
                                    295 	.globl _EPIRQ
                                    296 	.globl _EPIE
                                    297 	.globl _USBIRQ
                                    298 	.globl _USBIE
                                    299 	.globl _NAKIRQ
                                    300 	.globl _NAKIE
                                    301 	.globl _IBNIRQ
                                    302 	.globl _IBNIE
                                    303 	.globl _EP8FIFOIRQ
                                    304 	.globl _EP8FIFOIE
                                    305 	.globl _EP6FIFOIRQ
                                    306 	.globl _EP6FIFOIE
                                    307 	.globl _EP4FIFOIRQ
                                    308 	.globl _EP4FIFOIE
                                    309 	.globl _EP2FIFOIRQ
                                    310 	.globl _EP2FIFOIE
                                    311 	.globl _OUTPKTEND
                                    312 	.globl _INPKTEND
                                    313 	.globl _EP8ISOINPKTS
                                    314 	.globl _EP6ISOINPKTS
                                    315 	.globl _EP4ISOINPKTS
                                    316 	.globl _EP2ISOINPKTS
                                    317 	.globl _EP8FIFOPFL
                                    318 	.globl _EP8FIFOPFH
                                    319 	.globl _EP6FIFOPFL
                                    320 	.globl _EP6FIFOPFH
                                    321 	.globl _EP4FIFOPFL
                                    322 	.globl _EP4FIFOPFH
                                    323 	.globl _EP2FIFOPFL
                                    324 	.globl _EP2FIFOPFH
                                    325 	.globl _EP8AUTOINLENL
                                    326 	.globl _EP8AUTOINLENH
                                    327 	.globl _EP6AUTOINLENL
                                    328 	.globl _EP6AUTOINLENH
                                    329 	.globl _EP4AUTOINLENL
                                    330 	.globl _EP4AUTOINLENH
                                    331 	.globl _EP2AUTOINLENL
                                    332 	.globl _EP2AUTOINLENH
                                    333 	.globl _EP8FIFOCFG
                                    334 	.globl _EP6FIFOCFG
                                    335 	.globl _EP4FIFOCFG
                                    336 	.globl _EP2FIFOCFG
                                    337 	.globl _EP8CFG
                                    338 	.globl _EP6CFG
                                    339 	.globl _EP4CFG
                                    340 	.globl _EP2CFG
                                    341 	.globl _EP1INCFG
                                    342 	.globl _EP1OUTCFG
                                    343 	.globl _REVCTL
                                    344 	.globl _REVID
                                    345 	.globl _FIFOPINPOLAR
                                    346 	.globl _UART230
                                    347 	.globl _BPADDRL
                                    348 	.globl _BPADDRH
                                    349 	.globl _BREAKPT
                                    350 	.globl _FIFORESET
                                    351 	.globl _PINFLAGSCD
                                    352 	.globl _PINFLAGSAB
                                    353 	.globl _IFCONFIG
                                    354 	.globl _CPUCS
                                    355 	.globl _RES_WAVEDATA_END
                                    356 	.globl _GPIF_WAVE_DATA
                                    357 ;--------------------------------------------------------
                                    358 ; special function registers
                                    359 ;--------------------------------------------------------
                                    360 	.area RSEG    (ABS,DATA)
      000000                        361 	.org 0x0000
                           000080   362 _IOA	=	0x0080
                           000081   363 _SP	=	0x0081
                           000082   364 _DPL	=	0x0082
                           000083   365 _DPH	=	0x0083
                           000084   366 _DPL1	=	0x0084
                           000085   367 _DPH1	=	0x0085
                           000086   368 _DPS	=	0x0086
                           000087   369 _PCON	=	0x0087
                           000088   370 _TCON	=	0x0088
                           000089   371 _TMOD	=	0x0089
                           00008A   372 _TL0	=	0x008a
                           00008B   373 _TL1	=	0x008b
                           00008C   374 _TH0	=	0x008c
                           00008D   375 _TH1	=	0x008d
                           00008E   376 _CKCON	=	0x008e
                           00008F   377 _SPC_FNC	=	0x008f
                           000090   378 _IOB	=	0x0090
                           000091   379 _EXIF	=	0x0091
                           000092   380 _MPAGE	=	0x0092
                           000098   381 _SCON0	=	0x0098
                           000099   382 _SBUF0	=	0x0099
                           00009A   383 _AUTOPTRH1	=	0x009a
                           00009B   384 _AUTOPTRL1	=	0x009b
                           00009D   385 _AUTOPTRH2	=	0x009d
                           00009E   386 _AUTOPTRL2	=	0x009e
                           0000A0   387 _IOC	=	0x00a0
                           0000A1   388 _INT2CLR	=	0x00a1
                           0000A2   389 _INT4CLR	=	0x00a2
                           0000A8   390 _IE	=	0x00a8
                           0000AA   391 _EP2468STAT	=	0x00aa
                           0000AB   392 _EP24FIFOFLGS	=	0x00ab
                           0000AC   393 _EP68FIFOFLGS	=	0x00ac
                           0000AF   394 _AUTOPTRSETUP	=	0x00af
                           0000B0   395 _IOD	=	0x00b0
                           0000B1   396 _IOE	=	0x00b1
                           0000B2   397 _OEA	=	0x00b2
                           0000B3   398 _OEB	=	0x00b3
                           0000B4   399 _OEC	=	0x00b4
                           0000B5   400 _OED	=	0x00b5
                           0000B6   401 _OEE	=	0x00b6
                           0000B8   402 _IP	=	0x00b8
                           0000BA   403 _EP01STAT	=	0x00ba
                           0000BB   404 _GPIFTRIG	=	0x00bb
                           0000BD   405 _GPIFSGLDATH	=	0x00bd
                           0000BE   406 _GPIFSGLDATLX	=	0x00be
                           0000BF   407 _GPIFSGLDATLNOX	=	0x00bf
                           0000C0   408 _SCON1	=	0x00c0
                           0000C1   409 _SBUF1	=	0x00c1
                           0000C8   410 _T2CON	=	0x00c8
                           0000CA   411 _RCAP2L	=	0x00ca
                           0000CB   412 _RCAP2H	=	0x00cb
                           0000CC   413 _TL2	=	0x00cc
                           0000CD   414 _TH2	=	0x00cd
                           0000D0   415 _PSW	=	0x00d0
                           0000D8   416 _EICON	=	0x00d8
                           0000E0   417 _ACC	=	0x00e0
                           0000E8   418 _EIE	=	0x00e8
                           0000F0   419 _B	=	0x00f0
                           0000F8   420 _EIP	=	0x00f8
                                    421 ;--------------------------------------------------------
                                    422 ; special function bits
                                    423 ;--------------------------------------------------------
                                    424 	.area RSEG    (ABS,DATA)
      000000                        425 	.org 0x0000
                           000080   426 _PA0	=	0x0080
                           000081   427 _PA1	=	0x0081
                           000082   428 _PA2	=	0x0082
                           000083   429 _PA3	=	0x0083
                           000084   430 _PA4	=	0x0084
                           000085   431 _PA5	=	0x0085
                           000086   432 _PA6	=	0x0086
                           000087   433 _PA7	=	0x0087
                           000088   434 _IT0	=	0x0088
                           000089   435 _IE0	=	0x0089
                           00008A   436 _IT1	=	0x008a
                           00008B   437 _IE1	=	0x008b
                           00008C   438 _TR0	=	0x008c
                           00008D   439 _TF0	=	0x008d
                           00008E   440 _TR1	=	0x008e
                           00008F   441 _TF1	=	0x008f
                           000090   442 _PB0	=	0x0090
                           000091   443 _PB1	=	0x0091
                           000092   444 _PB2	=	0x0092
                           000093   445 _PB3	=	0x0093
                           000094   446 _PB4	=	0x0094
                           000095   447 _PB5	=	0x0095
                           000096   448 _PB6	=	0x0096
                           000097   449 _PB7	=	0x0097
                           000098   450 _RI	=	0x0098
                           000099   451 _TI	=	0x0099
                           00009A   452 _RB8	=	0x009a
                           00009B   453 _TB8	=	0x009b
                           00009C   454 _REN	=	0x009c
                           00009D   455 _SM2	=	0x009d
                           00009E   456 _SM1	=	0x009e
                           00009F   457 _SM0	=	0x009f
                           0000A0   458 _PC0	=	0x00a0
                           0000A1   459 _PC1	=	0x00a1
                           0000A2   460 _PC2	=	0x00a2
                           0000A3   461 _PC3	=	0x00a3
                           0000A4   462 _PC4	=	0x00a4
                           0000A5   463 _PC5	=	0x00a5
                           0000A6   464 _PC6	=	0x00a6
                           0000A7   465 _PC7	=	0x00a7
                           0000A8   466 _EX0	=	0x00a8
                           0000A9   467 _ET0	=	0x00a9
                           0000AA   468 _EX1	=	0x00aa
                           0000AB   469 _ET1	=	0x00ab
                           0000AC   470 _ES0	=	0x00ac
                           0000AD   471 _ET2	=	0x00ad
                           0000AE   472 _ES1	=	0x00ae
                           0000AF   473 _EA	=	0x00af
                           0000B0   474 _PD0	=	0x00b0
                           0000B1   475 _PD1	=	0x00b1
                           0000B2   476 _PD2	=	0x00b2
                           0000B3   477 _PD3	=	0x00b3
                           0000B4   478 _PD4	=	0x00b4
                           0000B5   479 _PD5	=	0x00b5
                           0000B6   480 _PD6	=	0x00b6
                           0000B7   481 _PD7	=	0x00b7
                           0000B8   482 _PX0	=	0x00b8
                           0000B9   483 _PT0	=	0x00b9
                           0000BA   484 _PX1	=	0x00ba
                           0000BB   485 _PT1	=	0x00bb
                           0000BC   486 _PS0	=	0x00bc
                           0000BD   487 _PT2	=	0x00bd
                           0000BE   488 _PS1	=	0x00be
                           0000C0   489 _RI1	=	0x00c0
                           0000C1   490 _TI1	=	0x00c1
                           0000C2   491 _RB81	=	0x00c2
                           0000C3   492 _TB81	=	0x00c3
                           0000C4   493 _REN1	=	0x00c4
                           0000C5   494 _SM21	=	0x00c5
                           0000C6   495 _SM11	=	0x00c6
                           0000C7   496 _SM01	=	0x00c7
                           0000C8   497 _CP_RL2	=	0x00c8
                           0000C9   498 _C_T2	=	0x00c9
                           0000CA   499 _TR2	=	0x00ca
                           0000CB   500 _EXEN2	=	0x00cb
                           0000CC   501 _TCLK	=	0x00cc
                           0000CD   502 _RCLK	=	0x00cd
                           0000CE   503 _EXF2	=	0x00ce
                           0000CF   504 _TF2	=	0x00cf
                           0000D0   505 _P	=	0x00d0
                           0000D1   506 _FL	=	0x00d1
                           0000D2   507 _OV	=	0x00d2
                           0000D3   508 _RS0	=	0x00d3
                           0000D4   509 _RS1	=	0x00d4
                           0000D5   510 _F0	=	0x00d5
                           0000D6   511 _AC	=	0x00d6
                           0000D7   512 _CY	=	0x00d7
                           0000DB   513 _INT6	=	0x00db
                           0000DC   514 _RESI	=	0x00dc
                           0000DD   515 _ERESI	=	0x00dd
                           0000DF   516 _SMOD1	=	0x00df
                           0000E8   517 _EUSB	=	0x00e8
                           0000E9   518 _EI2C	=	0x00e9
                           0000EA   519 _EIEX4	=	0x00ea
                           0000EB   520 _EIEX5	=	0x00eb
                           0000EC   521 _EIEX6	=	0x00ec
                           0000F8   522 _PUSB	=	0x00f8
                           0000F9   523 _PI2C	=	0x00f9
                           0000FA   524 _EIPX4	=	0x00fa
                           0000FB   525 _EIPX5	=	0x00fb
                           0000FC   526 _EIPX6	=	0x00fc
                                    527 ;--------------------------------------------------------
                                    528 ; overlayable register banks
                                    529 ;--------------------------------------------------------
                                    530 	.area REG_BANK_0	(REL,OVR,DATA)
      000000                        531 	.ds 8
                                    532 ;--------------------------------------------------------
                                    533 ; internal ram data
                                    534 ;--------------------------------------------------------
                                    535 	.area DSEG    (DATA)
                                    536 ;--------------------------------------------------------
                                    537 ; overlayable items in internal ram 
                                    538 ;--------------------------------------------------------
                                    539 	.area	OSEG    (OVR,DATA)
                                    540 	.area	OSEG    (OVR,DATA)
      000008                        541 _send_state_msg2_65536_23:
      000008                        542 	.ds 3
                                    543 ;--------------------------------------------------------
                                    544 ; Stack segment in internal ram 
                                    545 ;--------------------------------------------------------
                                    546 	.area	SSEG
      00000B                        547 __start__stack:
      00000B                        548 	.ds	1
                                    549 
                                    550 ;--------------------------------------------------------
                                    551 ; indirectly addressable internal ram data
                                    552 ;--------------------------------------------------------
                                    553 	.area ISEG    (DATA)
                                    554 ;--------------------------------------------------------
                                    555 ; absolute internal ram data
                                    556 ;--------------------------------------------------------
                                    557 	.area IABS    (ABS,DATA)
                                    558 	.area IABS    (ABS,DATA)
                                    559 ;--------------------------------------------------------
                                    560 ; bit data
                                    561 ;--------------------------------------------------------
                                    562 	.area BSEG    (BIT)
                                    563 ;--------------------------------------------------------
                                    564 ; paged external ram data
                                    565 ;--------------------------------------------------------
                                    566 	.area PSEG    (PAG,XDATA)
                                    567 ;--------------------------------------------------------
                                    568 ; external ram data
                                    569 ;--------------------------------------------------------
                                    570 	.area XSEG    (XDATA)
                           00E400   571 _GPIF_WAVE_DATA	=	0xe400
                           00E480   572 _RES_WAVEDATA_END	=	0xe480
                           00E600   573 _CPUCS	=	0xe600
                           00E601   574 _IFCONFIG	=	0xe601
                           00E602   575 _PINFLAGSAB	=	0xe602
                           00E603   576 _PINFLAGSCD	=	0xe603
                           00E604   577 _FIFORESET	=	0xe604
                           00E605   578 _BREAKPT	=	0xe605
                           00E606   579 _BPADDRH	=	0xe606
                           00E607   580 _BPADDRL	=	0xe607
                           00E608   581 _UART230	=	0xe608
                           00E609   582 _FIFOPINPOLAR	=	0xe609
                           00E60A   583 _REVID	=	0xe60a
                           00E60B   584 _REVCTL	=	0xe60b
                           00E610   585 _EP1OUTCFG	=	0xe610
                           00E611   586 _EP1INCFG	=	0xe611
                           00E612   587 _EP2CFG	=	0xe612
                           00E613   588 _EP4CFG	=	0xe613
                           00E614   589 _EP6CFG	=	0xe614
                           00E615   590 _EP8CFG	=	0xe615
                           00E618   591 _EP2FIFOCFG	=	0xe618
                           00E619   592 _EP4FIFOCFG	=	0xe619
                           00E61A   593 _EP6FIFOCFG	=	0xe61a
                           00E61B   594 _EP8FIFOCFG	=	0xe61b
                           00E620   595 _EP2AUTOINLENH	=	0xe620
                           00E621   596 _EP2AUTOINLENL	=	0xe621
                           00E622   597 _EP4AUTOINLENH	=	0xe622
                           00E623   598 _EP4AUTOINLENL	=	0xe623
                           00E624   599 _EP6AUTOINLENH	=	0xe624
                           00E625   600 _EP6AUTOINLENL	=	0xe625
                           00E626   601 _EP8AUTOINLENH	=	0xe626
                           00E627   602 _EP8AUTOINLENL	=	0xe627
                           00E630   603 _EP2FIFOPFH	=	0xe630
                           00E631   604 _EP2FIFOPFL	=	0xe631
                           00E632   605 _EP4FIFOPFH	=	0xe632
                           00E633   606 _EP4FIFOPFL	=	0xe633
                           00E634   607 _EP6FIFOPFH	=	0xe634
                           00E635   608 _EP6FIFOPFL	=	0xe635
                           00E636   609 _EP8FIFOPFH	=	0xe636
                           00E637   610 _EP8FIFOPFL	=	0xe637
                           00E640   611 _EP2ISOINPKTS	=	0xe640
                           00E641   612 _EP4ISOINPKTS	=	0xe641
                           00E642   613 _EP6ISOINPKTS	=	0xe642
                           00E643   614 _EP8ISOINPKTS	=	0xe643
                           00E648   615 _INPKTEND	=	0xe648
                           00E649   616 _OUTPKTEND	=	0xe649
                           00E650   617 _EP2FIFOIE	=	0xe650
                           00E651   618 _EP2FIFOIRQ	=	0xe651
                           00E652   619 _EP4FIFOIE	=	0xe652
                           00E653   620 _EP4FIFOIRQ	=	0xe653
                           00E654   621 _EP6FIFOIE	=	0xe654
                           00E655   622 _EP6FIFOIRQ	=	0xe655
                           00E656   623 _EP8FIFOIE	=	0xe656
                           00E657   624 _EP8FIFOIRQ	=	0xe657
                           00E658   625 _IBNIE	=	0xe658
                           00E659   626 _IBNIRQ	=	0xe659
                           00E65A   627 _NAKIE	=	0xe65a
                           00E65B   628 _NAKIRQ	=	0xe65b
                           00E65C   629 _USBIE	=	0xe65c
                           00E65D   630 _USBIRQ	=	0xe65d
                           00E65E   631 _EPIE	=	0xe65e
                           00E65F   632 _EPIRQ	=	0xe65f
                           00E660   633 _GPIFIE	=	0xe660
                           00E661   634 _GPIFIRQ	=	0xe661
                           00E662   635 _USBERRIE	=	0xe662
                           00E663   636 _USBERRIRQ	=	0xe663
                           00E664   637 _ERRCNTLIM	=	0xe664
                           00E665   638 _CLRERRCNT	=	0xe665
                           00E666   639 _INT2IVEC	=	0xe666
                           00E667   640 _INT4IVEC	=	0xe667
                           00E668   641 _INTSETUP	=	0xe668
                           00E670   642 _PORTACFG	=	0xe670
                           00E671   643 _PORTCCFG	=	0xe671
                           00E672   644 _PORTECFG	=	0xe672
                           00E678   645 _I2CS	=	0xe678
                           00E679   646 _I2DAT	=	0xe679
                           00E67A   647 _I2CTL	=	0xe67a
                           00E67B   648 _XAUTODAT1	=	0xe67b
                           00E67C   649 _XAUTODAT2	=	0xe67c
                           00E680   650 _USBCS	=	0xe680
                           00E681   651 _SUSPEND	=	0xe681
                           00E682   652 _WAKEUPCS	=	0xe682
                           00E683   653 _TOGCTL	=	0xe683
                           00E684   654 _USBFRAMEH	=	0xe684
                           00E685   655 _USBFRAMEL	=	0xe685
                           00E686   656 _MICROFRAME	=	0xe686
                           00E687   657 _FNADDR	=	0xe687
                           00E68A   658 _EP0BCH	=	0xe68a
                           00E68B   659 _EP0BCL	=	0xe68b
                           00E68D   660 _EP1OUTBC	=	0xe68d
                           00E68F   661 _EP1INBC	=	0xe68f
                           00E690   662 _EP2BCH	=	0xe690
                           00E691   663 _EP2BCL	=	0xe691
                           00E694   664 _EP4BCH	=	0xe694
                           00E695   665 _EP4BCL	=	0xe695
                           00E698   666 _EP6BCH	=	0xe698
                           00E699   667 _EP6BCL	=	0xe699
                           00E69C   668 _EP8BCH	=	0xe69c
                           00E69D   669 _EP8BCL	=	0xe69d
                           00E6A0   670 _EP0CS	=	0xe6a0
                           00E6A1   671 _EP1OUTCS	=	0xe6a1
                           00E6A2   672 _EP1INCS	=	0xe6a2
                           00E6A3   673 _EP2CS	=	0xe6a3
                           00E6A4   674 _EP4CS	=	0xe6a4
                           00E6A5   675 _EP6CS	=	0xe6a5
                           00E6A6   676 _EP8CS	=	0xe6a6
                           00E6A7   677 _EP2FIFOFLGS	=	0xe6a7
                           00E6A8   678 _EP4FIFOFLGS	=	0xe6a8
                           00E6A9   679 _EP6FIFOFLGS	=	0xe6a9
                           00E6AA   680 _EP8FIFOFLGS	=	0xe6aa
                           00E6AB   681 _EP2FIFOBCH	=	0xe6ab
                           00E6AC   682 _EP2FIFOBCL	=	0xe6ac
                           00E6AD   683 _EP4FIFOBCH	=	0xe6ad
                           00E6AE   684 _EP4FIFOBCL	=	0xe6ae
                           00E6AF   685 _EP6FIFOBCH	=	0xe6af
                           00E6B0   686 _EP6FIFOBCL	=	0xe6b0
                           00E6B1   687 _EP8FIFOBCH	=	0xe6b1
                           00E6B2   688 _EP8FIFOBCL	=	0xe6b2
                           00E6B3   689 _SUDPTRH	=	0xe6b3
                           00E6B4   690 _SUDPTRL	=	0xe6b4
                           00E6B5   691 _SUDPTRCTL	=	0xe6b5
                           00E6B8   692 _SETUPDAT	=	0xe6b8
                           00E6C0   693 _GPIFWFSELECT	=	0xe6c0
                           00E6C1   694 _GPIFIDLECS	=	0xe6c1
                           00E6C2   695 _GPIFIDLECTL	=	0xe6c2
                           00E6C3   696 _GPIFCTLCFG	=	0xe6c3
                           00E6C4   697 _GPIFADRH	=	0xe6c4
                           00E6C5   698 _GPIFADRL	=	0xe6c5
                           00E6CE   699 _GPIFTCB3	=	0xe6ce
                           00E6CF   700 _GPIFTCB2	=	0xe6cf
                           00E6D0   701 _GPIFTCB1	=	0xe6d0
                           00E6D1   702 _GPIFTCB0	=	0xe6d1
                           00E6D2   703 _EP2GPIFFLGSEL	=	0xe6d2
                           00E6D3   704 _EP2GPIFPFSTOP	=	0xe6d3
                           00E6D4   705 _EP2GPIFTRIG	=	0xe6d4
                           00E6DA   706 _EP4GPIFFLGSEL	=	0xe6da
                           00E6DB   707 _EP4GPIFPFSTOP	=	0xe6db
                           00E6DC   708 _EP4GPIFTRIG	=	0xe6dc
                           00E6E2   709 _EP6GPIFFLGSEL	=	0xe6e2
                           00E6E3   710 _EP6GPIFPFSTOP	=	0xe6e3
                           00E6E4   711 _EP6GPIFTRIG	=	0xe6e4
                           00E6EA   712 _EP8GPIFFLGSEL	=	0xe6ea
                           00E6EB   713 _EP8GPIFPFSTOP	=	0xe6eb
                           00E6EC   714 _EP8GPIFTRIG	=	0xe6ec
                           00E6F0   715 _XGPIFSGLDATH	=	0xe6f0
                           00E6F1   716 _XGPIFSGLDATLX	=	0xe6f1
                           00E6F2   717 _XGPIFSGLDATLNOX	=	0xe6f2
                           00E6F3   718 _GPIFREADYCFG	=	0xe6f3
                           00E6F4   719 _GPIFREADYSTAT	=	0xe6f4
                           00E6F5   720 _GPIFABORT	=	0xe6f5
                           00E6C6   721 _FLOWSTATE	=	0xe6c6
                           00E6C7   722 _FLOWLOGIC	=	0xe6c7
                           00E6C8   723 _FLOWEQ0CTL	=	0xe6c8
                           00E6C9   724 _FLOWEQ1CTL	=	0xe6c9
                           00E6CA   725 _FLOWHOLDOFF	=	0xe6ca
                           00E6CB   726 _FLOWSTB	=	0xe6cb
                           00E6CC   727 _FLOWSTBEDGE	=	0xe6cc
                           00E6CD   728 _FLOWSTBHPERIOD	=	0xe6cd
                           00E60C   729 _GPIFHOLDAMOUNT	=	0xe60c
                           00E67D   730 _UDMACRCH	=	0xe67d
                           00E67E   731 _UDMACRCL	=	0xe67e
                           00E67F   732 _UDMACRCQUAL	=	0xe67f
                           00E6F8   733 _DBUG	=	0xe6f8
                           00E6F9   734 _TESTCFG	=	0xe6f9
                           00E6FA   735 _USBTEST	=	0xe6fa
                           00E6FB   736 _CT1	=	0xe6fb
                           00E6FC   737 _CT2	=	0xe6fc
                           00E6FD   738 _CT3	=	0xe6fd
                           00E6FE   739 _CT4	=	0xe6fe
                           00E740   740 _EP0BUF	=	0xe740
                           00E780   741 _EP1OUTBUF	=	0xe780
                           00E7C0   742 _EP1INBUF	=	0xe7c0
                           00F000   743 _EP2FIFOBUF	=	0xf000
                           00F400   744 _EP4FIFOBUF	=	0xf400
                           00F800   745 _EP6FIFOBUF	=	0xf800
                           00FC00   746 _EP8FIFOBUF	=	0xfc00
                           00E628   747 _ECCCFG	=	0xe628
                           00E629   748 _ECCRESET	=	0xe629
                           00E62A   749 _ECC1B0	=	0xe62a
                           00E62B   750 _ECC1B1	=	0xe62b
                           00E62C   751 _ECC1B2	=	0xe62c
                           00E62D   752 _ECC2B0	=	0xe62d
                           00E62E   753 _ECC2B1	=	0xe62e
                           00E62F   754 _ECC2B2	=	0xe62f
                           00E50D   755 _GPCR2	=	0xe50d
                                    756 ;--------------------------------------------------------
                                    757 ; absolute external ram data
                                    758 ;--------------------------------------------------------
                                    759 	.area XABS    (ABS,XDATA)
                                    760 ;--------------------------------------------------------
                                    761 ; external initialized ram data
                                    762 ;--------------------------------------------------------
                                    763 	.area XISEG   (XDATA)
                                    764 	.area HOME    (CODE)
                                    765 	.area GSINIT0 (CODE)
                                    766 	.area GSINIT1 (CODE)
                                    767 	.area GSINIT2 (CODE)
                                    768 	.area GSINIT3 (CODE)
                                    769 	.area GSINIT4 (CODE)
                                    770 	.area GSINIT5 (CODE)
                                    771 	.area GSINIT  (CODE)
                                    772 	.area GSFINAL (CODE)
                                    773 	.area CSEG    (CODE)
                                    774 ;--------------------------------------------------------
                                    775 ; interrupt vector 
                                    776 ;--------------------------------------------------------
                                    777 	.area HOME    (CODE)
      000000                        778 __interrupt_vect:
      000000 02 00 06         [24]  779 	ljmp	__sdcc_gsinit_startup
                                    780 ;--------------------------------------------------------
                                    781 ; global & static initialisations
                                    782 ;--------------------------------------------------------
                                    783 	.area HOME    (CODE)
                                    784 	.area GSINIT  (CODE)
                                    785 	.area GSFINAL (CODE)
                                    786 	.area GSINIT  (CODE)
                                    787 	.globl __sdcc_gsinit_startup
                                    788 	.globl __sdcc_program_startup
                                    789 	.globl __start__stack
                                    790 	.globl __mcs51_genXINIT
                                    791 	.globl __mcs51_genXRAMCLEAR
                                    792 	.globl __mcs51_genRAMCLEAR
                                    793 	.area GSFINAL (CODE)
      00005F 02 00 03         [24]  794 	ljmp	__sdcc_program_startup
                                    795 ;--------------------------------------------------------
                                    796 ; Home
                                    797 ;--------------------------------------------------------
                                    798 	.area HOME    (CODE)
                                    799 	.area HOME    (CODE)
      000003                        800 __sdcc_program_startup:
      000003 02 01 A6         [24]  801 	ljmp	_main
                                    802 ;	return from main will return to caller
                                    803 ;--------------------------------------------------------
                                    804 ; code
                                    805 ;--------------------------------------------------------
                                    806 	.area CSEG    (CODE)
                                    807 ;------------------------------------------------------------
                                    808 ;Allocation info for local variables in function 'initialize'
                                    809 ;------------------------------------------------------------
                                    810 ;	ezusb.c:11: initialize(void) {
                                    811 ;	-----------------------------------------
                                    812 ;	 function initialize
                                    813 ;	-----------------------------------------
      000062                        814 _initialize:
                           000007   815 	ar7 = 0x07
                           000006   816 	ar6 = 0x06
                           000005   817 	ar5 = 0x05
                           000004   818 	ar4 = 0x04
                           000003   819 	ar3 = 0x03
                           000002   820 	ar2 = 0x02
                           000001   821 	ar1 = 0x01
                           000000   822 	ar0 = 0x00
                                    823 ;	ezusb.c:13: CPUCS = 0x10;		// 48 MHz, CLKOUT disabled.
      000062 90 E6 00         [24]  824 	mov	dptr,#_CPUCS
      000065 74 10            [12]  825 	mov	a,#0x10
      000067 F0               [24]  826 	movx	@dptr,a
                                    827 ;	ezusb.c:14: SYNCDELAY;		
      000068 00               [12]  828 	nop 
      000069 00               [12]  829 	nop 
      00006A 00               [12]  830 	nop 
                                    831 ;	ezusb.c:15: IFCONFIG = 0xc0;	// Internal IFCLK @ 48MHz
      00006B 90 E6 01         [24]  832 	mov	dptr,#_IFCONFIG
      00006E 74 C0            [12]  833 	mov	a,#0xc0
      000070 F0               [24]  834 	movx	@dptr,a
                                    835 ;	ezusb.c:16: SYNCDELAY;		
      000071 00               [12]  836 	nop 
      000072 00               [12]  837 	nop 
      000073 00               [12]  838 	nop 
                                    839 ;	ezusb.c:17: REVCTL = 0x03;		// Disable auto-arm + Enhanced packet handling
      000074 90 E6 0B         [24]  840 	mov	dptr,#_REVCTL
      000077 74 03            [12]  841 	mov	a,#0x03
      000079 F0               [24]  842 	movx	@dptr,a
                                    843 ;	ezusb.c:18: SYNCDELAY;		
      00007A 00               [12]  844 	nop 
      00007B 00               [12]  845 	nop 
      00007C 00               [12]  846 	nop 
                                    847 ;	ezusb.c:19: EP6CFG = 0xE2;		// 1110_0010 bulk IN, 512 bytes, double-buffered
      00007D 90 E6 14         [24]  848 	mov	dptr,#_EP6CFG
      000080 74 E2            [12]  849 	mov	a,#0xe2
      000082 F0               [24]  850 	movx	@dptr,a
                                    851 ;	ezusb.c:20: SYNCDELAY;
      000083 00               [12]  852 	nop 
      000084 00               [12]  853 	nop 
      000085 00               [12]  854 	nop 
                                    855 ;	ezusb.c:21: EP2CFG = 0xA2;		// 1010_0010 bulk OUT, 512 bytes, double-buffered
      000086 90 E6 12         [24]  856 	mov	dptr,#_EP2CFG
      000089 74 A2            [12]  857 	mov	a,#0xa2
      00008B F0               [24]  858 	movx	@dptr,a
                                    859 ;	ezusb.c:22: SYNCDELAY;
      00008C 00               [12]  860 	nop 
      00008D 00               [12]  861 	nop 
      00008E 00               [12]  862 	nop 
                                    863 ;	ezusb.c:23: FIFORESET = 0x80;	// NAK all requests from host.
      00008F 90 E6 04         [24]  864 	mov	dptr,#_FIFORESET
      000092 74 80            [12]  865 	mov	a,#0x80
      000094 F0               [24]  866 	movx	@dptr,a
                                    867 ;	ezusb.c:24: SYNCDELAY;	
      000095 00               [12]  868 	nop 
      000096 00               [12]  869 	nop 
      000097 00               [12]  870 	nop 
                                    871 ;	ezusb.c:25: FIFORESET = 0x82;	// Reset EP 2
      000098 90 E6 04         [24]  872 	mov	dptr,#_FIFORESET
      00009B 74 82            [12]  873 	mov	a,#0x82
      00009D F0               [24]  874 	movx	@dptr,a
                                    875 ;	ezusb.c:26: SYNCDELAY;	
      00009E 00               [12]  876 	nop 
      00009F 00               [12]  877 	nop 
      0000A0 00               [12]  878 	nop 
                                    879 ;	ezusb.c:27: FIFORESET = 0x84;	// Reset EP 4..
      0000A1 90 E6 04         [24]  880 	mov	dptr,#_FIFORESET
      0000A4 74 84            [12]  881 	mov	a,#0x84
      0000A6 F0               [24]  882 	movx	@dptr,a
                                    883 ;	ezusb.c:28: SYNCDELAY;
      0000A7 00               [12]  884 	nop 
      0000A8 00               [12]  885 	nop 
      0000A9 00               [12]  886 	nop 
                                    887 ;	ezusb.c:29: FIFORESET = 0x86;
      0000AA 90 E6 04         [24]  888 	mov	dptr,#_FIFORESET
      0000AD 74 86            [12]  889 	mov	a,#0x86
      0000AF F0               [24]  890 	movx	@dptr,a
                                    891 ;	ezusb.c:30: SYNCDELAY;
      0000B0 00               [12]  892 	nop 
      0000B1 00               [12]  893 	nop 
      0000B2 00               [12]  894 	nop 
                                    895 ;	ezusb.c:31: FIFORESET = 0x88;
      0000B3 90 E6 04         [24]  896 	mov	dptr,#_FIFORESET
      0000B6 74 88            [12]  897 	mov	a,#0x88
      0000B8 F0               [24]  898 	movx	@dptr,a
                                    899 ;	ezusb.c:32: SYNCDELAY;
      0000B9 00               [12]  900 	nop 
      0000BA 00               [12]  901 	nop 
      0000BB 00               [12]  902 	nop 
                                    903 ;	ezusb.c:33: FIFORESET = 0x00;	// Back to normal..
      0000BC 90 E6 04         [24]  904 	mov	dptr,#_FIFORESET
      0000BF E4               [12]  905 	clr	a
      0000C0 F0               [24]  906 	movx	@dptr,a
                                    907 ;	ezusb.c:34: SYNCDELAY;		
      0000C1 00               [12]  908 	nop 
      0000C2 00               [12]  909 	nop 
      0000C3 00               [12]  910 	nop 
                                    911 ;	ezusb.c:35: EP2FIFOCFG = 0x00;	// Disable AUTOOUT
      0000C4 90 E6 18         [24]  912 	mov	dptr,#_EP2FIFOCFG
      0000C7 E4               [12]  913 	clr	a
      0000C8 F0               [24]  914 	movx	@dptr,a
                                    915 ;	ezusb.c:36: SYNCDELAY;		
      0000C9 00               [12]  916 	nop 
      0000CA 00               [12]  917 	nop 
      0000CB 00               [12]  918 	nop 
                                    919 ;	ezusb.c:37: OUTPKTEND = 0x82;	// Clear the 1st buffer
      0000CC 90 E6 49         [24]  920 	mov	dptr,#_OUTPKTEND
      0000CF 74 82            [12]  921 	mov	a,#0x82
      0000D1 F0               [24]  922 	movx	@dptr,a
                                    923 ;	ezusb.c:38: SYNCDELAY;		
      0000D2 00               [12]  924 	nop 
      0000D3 00               [12]  925 	nop 
      0000D4 00               [12]  926 	nop 
                                    927 ;	ezusb.c:39: OUTPKTEND = 0x82;	// ..both of them
      0000D5 90 E6 49         [24]  928 	mov	dptr,#_OUTPKTEND
      0000D8 74 82            [12]  929 	mov	a,#0x82
      0000DA F0               [24]  930 	movx	@dptr,a
                                    931 ;	ezusb.c:40: SYNCDELAY;		
      0000DB 00               [12]  932 	nop 
      0000DC 00               [12]  933 	nop 
      0000DD 00               [12]  934 	nop 
                                    935 ;	ezusb.c:41: }
      0000DE 22               [24]  936 	ret
                                    937 ;------------------------------------------------------------
                                    938 ;Allocation info for local variables in function 'accept_cmd'
                                    939 ;------------------------------------------------------------
                                    940 ;src                       Allocated to registers 
                                    941 ;len                       Allocated to registers r7 r6 
                                    942 ;------------------------------------------------------------
                                    943 ;	ezusb.c:48: accept_cmd(void) {
                                    944 ;	-----------------------------------------
                                    945 ;	 function accept_cmd
                                    946 ;	-----------------------------------------
      0000DF                        947 _accept_cmd:
                                    948 ;	ezusb.c:49: __xdata const unsigned char *src = EP2FIFOBUF;
                                    949 ;	ezusb.c:50: unsigned len = ((unsigned)EP2BCH)<<8 | EP2BCL;
      0000DF 90 E6 90         [24]  950 	mov	dptr,#_EP2BCH
      0000E2 E0               [24]  951 	movx	a,@dptr
      0000E3 FE               [12]  952 	mov	r6,a
      0000E4 7F 00            [12]  953 	mov	r7,#0x00
      0000E6 90 E6 91         [24]  954 	mov	dptr,#_EP2BCL
      0000E9 E0               [24]  955 	movx	a,@dptr
      0000EA 7C 00            [12]  956 	mov	r4,#0x00
      0000EC 42 07            [12]  957 	orl	ar7,a
      0000EE EC               [12]  958 	mov	a,r4
      0000EF 42 06            [12]  959 	orl	ar6,a
                                    960 ;	ezusb.c:52: if ( len < 1 )
      0000F1 C3               [12]  961 	clr	c
      0000F2 EF               [12]  962 	mov	a,r7
      0000F3 94 01            [12]  963 	subb	a,#0x01
      0000F5 EE               [12]  964 	mov	a,r6
      0000F6 94 00            [12]  965 	subb	a,#0x00
      0000F8 50 01            [24]  966 	jnc	00102$
                                    967 ;	ezusb.c:53: return;		// Nothing to process
      0000FA 22               [24]  968 	ret
      0000FB                        969 00102$:
                                    970 ;	ezusb.c:54: PA0 = *src & 1;		// Set PA0 LED
      0000FB 90 F0 00         [24]  971 	mov	dptr,#_EP2FIFOBUF
      0000FE E0               [24]  972 	movx	a,@dptr
      0000FF FF               [12]  973 	mov	r7,a
      000100 54 01            [12]  974 	anl	a,#0x01
      000102 24 FF            [12]  975 	add	a,#0xff
      000104 92 80            [24]  976 	mov	_PA0,c
                                    977 ;	ezusb.c:55: PA1 = *src & 2;		// Set PA1 LED
      000106 EF               [12]  978 	mov	a,r7
      000107 03               [12]  979 	rr	a
      000108 54 01            [12]  980 	anl	a,#0x01
      00010A 24 FF            [12]  981 	add	a,#0xff
      00010C 92 81            [24]  982 	mov	_PA1,c
                                    983 ;	ezusb.c:56: OUTPKTEND = 0x82;	// Release buffer
      00010E 90 E6 49         [24]  984 	mov	dptr,#_OUTPKTEND
      000111 74 82            [12]  985 	mov	a,#0x82
      000113 F0               [24]  986 	movx	@dptr,a
                                    987 ;	ezusb.c:57: }
      000114 22               [24]  988 	ret
                                    989 ;------------------------------------------------------------
                                    990 ;Allocation info for local variables in function 'send_state'
                                    991 ;------------------------------------------------------------
                                    992 ;dest                      Allocated to registers 
                                    993 ;msg1                      Allocated to registers r6 r5 r7 
                                    994 ;msg2                      Allocated with name '_send_state_msg2_65536_23'
                                    995 ;len                       Allocated to registers 
                                    996 ;------------------------------------------------------------
                                    997 ;	ezusb.c:64: send_state(void) {
                                    998 ;	-----------------------------------------
                                    999 ;	 function send_state
                                   1000 ;	-----------------------------------------
      000115                       1001 _send_state:
                                   1002 ;	ezusb.c:65: __xdata unsigned char *dest = EP6FIFOBUF;
                                   1003 ;	ezusb.c:66: const char *msg1 = PA0 ? "PA0=1" : "PA0=0";
      000115 30 80 06         [24] 1004 	jnb	_PA0,00109$
      000118 7E E6            [12] 1005 	mov	r6,#___str_0
      00011A 7F 01            [12] 1006 	mov	r7,#(___str_0 >> 8)
      00011C 80 04            [24] 1007 	sjmp	00110$
      00011E                       1008 00109$:
      00011E 7E EC            [12] 1009 	mov	r6,#___str_1
      000120 7F 01            [12] 1010 	mov	r7,#(___str_1 >> 8)
      000122                       1011 00110$:
      000122 8F 05            [24] 1012 	mov	ar5,r7
      000124 7F 80            [12] 1013 	mov	r7,#0x80
                                   1014 ;	ezusb.c:67: const char *msg2 = PA1 ? "PA1=1" : "PA1=0";
      000126 30 81 06         [24] 1015 	jnb	_PA1,00111$
      000129 7B F2            [12] 1016 	mov	r3,#___str_2
      00012B 7C 01            [12] 1017 	mov	r4,#(___str_2 >> 8)
      00012D 80 04            [24] 1018 	sjmp	00112$
      00012F                       1019 00111$:
      00012F 7B F8            [12] 1020 	mov	r3,#___str_3
      000131 7C 01            [12] 1021 	mov	r4,#(___str_3 >> 8)
      000133                       1022 00112$:
      000133 8B 08            [24] 1023 	mov	_send_state_msg2_65536_23,r3
      000135 8C 09            [24] 1024 	mov	(_send_state_msg2_65536_23 + 1),r4
      000137 75 0A 80         [24] 1025 	mov	(_send_state_msg2_65536_23 + 2),#0x80
                                   1026 ;	ezusb.c:70: while ( *msg1 ) {
      00013A 78 00            [12] 1027 	mov	r0,#_EP6FIFOBUF
      00013C 79 F8            [12] 1028 	mov	r1,#(_EP6FIFOBUF >> 8)
      00013E 7C 00            [12] 1029 	mov	r4,#0x00
      000140                       1030 00101$:
      000140 8E 82            [24] 1031 	mov	dpl,r6
      000142 8D 83            [24] 1032 	mov	dph,r5
      000144 8F F0            [24] 1033 	mov	b,r7
      000146 12 01 C6         [24] 1034 	lcall	__gptrget
      000149 FB               [12] 1035 	mov	r3,a
      00014A 60 13            [24] 1036 	jz	00103$
                                   1037 ;	ezusb.c:71: *dest++ = *msg1++;
      00014C 0E               [12] 1038 	inc	r6
      00014D BE 00 01         [24] 1039 	cjne	r6,#0x00,00148$
      000150 0D               [12] 1040 	inc	r5
      000151                       1041 00148$:
      000151 88 82            [24] 1042 	mov	dpl,r0
      000153 89 83            [24] 1043 	mov	dph,r1
      000155 EB               [12] 1044 	mov	a,r3
      000156 F0               [24] 1045 	movx	@dptr,a
      000157 A3               [24] 1046 	inc	dptr
      000158 A8 82            [24] 1047 	mov	r0,dpl
      00015A A9 83            [24] 1048 	mov	r1,dph
                                   1049 ;	ezusb.c:72: ++len;  
      00015C 0C               [12] 1050 	inc	r4
      00015D 80 E1            [24] 1051 	sjmp	00101$
      00015F                       1052 00103$:
                                   1053 ;	ezusb.c:74: *dest++ = ',';
      00015F 88 82            [24] 1054 	mov	dpl,r0
      000161 89 83            [24] 1055 	mov	dph,r1
      000163 74 2C            [12] 1056 	mov	a,#0x2c
      000165 F0               [24] 1057 	movx	@dptr,a
      000166 74 01            [12] 1058 	mov	a,#0x01
      000168 28               [12] 1059 	add	a,r0
      000169 FE               [12] 1060 	mov	r6,a
      00016A E4               [12] 1061 	clr	a
      00016B 39               [12] 1062 	addc	a,r1
      00016C FF               [12] 1063 	mov	r7,a
                                   1064 ;	ezusb.c:75: ++len;
      00016D EC               [12] 1065 	mov	a,r4
      00016E 04               [12] 1066 	inc	a
      00016F FD               [12] 1067 	mov	r5,a
                                   1068 ;	ezusb.c:76: while ( *msg2 ) {
      000170 AA 08            [24] 1069 	mov	r2,_send_state_msg2_65536_23
      000172 AB 09            [24] 1070 	mov	r3,(_send_state_msg2_65536_23 + 1)
      000174 AC 0A            [24] 1071 	mov	r4,(_send_state_msg2_65536_23 + 2)
      000176                       1072 00104$:
      000176 8A 82            [24] 1073 	mov	dpl,r2
      000178 8B 83            [24] 1074 	mov	dph,r3
      00017A 8C F0            [24] 1075 	mov	b,r4
      00017C 12 01 C6         [24] 1076 	lcall	__gptrget
      00017F F9               [12] 1077 	mov	r1,a
      000180 60 13            [24] 1078 	jz	00106$
                                   1079 ;	ezusb.c:77: *dest++ = *msg2++;
      000182 0A               [12] 1080 	inc	r2
      000183 BA 00 01         [24] 1081 	cjne	r2,#0x00,00150$
      000186 0B               [12] 1082 	inc	r3
      000187                       1083 00150$:
      000187 8E 82            [24] 1084 	mov	dpl,r6
      000189 8F 83            [24] 1085 	mov	dph,r7
      00018B E9               [12] 1086 	mov	a,r1
      00018C F0               [24] 1087 	movx	@dptr,a
      00018D A3               [24] 1088 	inc	dptr
      00018E AE 82            [24] 1089 	mov	r6,dpl
      000190 AF 83            [24] 1090 	mov	r7,dph
                                   1091 ;	ezusb.c:78: ++len;
      000192 0D               [12] 1092 	inc	r5
      000193 80 E1            [24] 1093 	sjmp	00104$
      000195                       1094 00106$:
                                   1095 ;	ezusb.c:81: SYNCDELAY;  
      000195 00               [12] 1096 	nop 
      000196 00               [12] 1097 	nop 
      000197 00               [12] 1098 	nop 
                                   1099 ;	ezusb.c:82: EP6BCH=0;
      000198 90 E6 98         [24] 1100 	mov	dptr,#_EP6BCH
      00019B E4               [12] 1101 	clr	a
      00019C F0               [24] 1102 	movx	@dptr,a
                                   1103 ;	ezusb.c:83: SYNCDELAY;  
      00019D 00               [12] 1104 	nop 
      00019E 00               [12] 1105 	nop 
      00019F 00               [12] 1106 	nop 
                                   1107 ;	ezusb.c:84: EP6BCL=len;	// Arms the endpoint for transmission
      0001A0 90 E6 99         [24] 1108 	mov	dptr,#_EP6BCL
      0001A3 ED               [12] 1109 	mov	a,r5
      0001A4 F0               [24] 1110 	movx	@dptr,a
                                   1111 ;	ezusb.c:85: }
      0001A5 22               [24] 1112 	ret
                                   1113 ;------------------------------------------------------------
                                   1114 ;Allocation info for local variables in function 'main'
                                   1115 ;------------------------------------------------------------
                                   1116 ;	ezusb.c:92: main(void) {
                                   1117 ;	-----------------------------------------
                                   1118 ;	 function main
                                   1119 ;	-----------------------------------------
      0001A6                       1120 _main:
                                   1121 ;	ezusb.c:94: OEA = 0x03;	// Enable PA0 and PA1 outputs
      0001A6 75 B2 03         [24] 1122 	mov	_OEA,#0x03
                                   1123 ;	ezusb.c:95: initialize();	// Initialize USB
      0001A9 12 00 62         [24] 1124 	lcall	_initialize
                                   1125 ;	ezusb.c:97: PA0 = 1;	// Turn off LEDs..
                                   1126 ;	assignBit
      0001AC D2 80            [12] 1127 	setb	_PA0
                                   1128 ;	ezusb.c:98: PA1 = 1;
                                   1129 ;	assignBit
      0001AE D2 81            [12] 1130 	setb	_PA1
      0001B0                       1131 00106$:
                                   1132 ;	ezusb.c:101: if ( !(EP2CS & bmEPEMPTY) )
      0001B0 90 E6 A3         [24] 1133 	mov	dptr,#_EP2CS
      0001B3 E0               [24] 1134 	movx	a,@dptr
      0001B4 20 E2 03         [24] 1135 	jb	acc.2,00102$
                                   1136 ;	ezusb.c:102: accept_cmd();	// Have data in EP2
      0001B7 12 00 DF         [24] 1137 	lcall	_accept_cmd
      0001BA                       1138 00102$:
                                   1139 ;	ezusb.c:104: if ( !(EP6CS & bmEPFULL) )
      0001BA 90 E6 A5         [24] 1140 	mov	dptr,#_EP6CS
      0001BD E0               [24] 1141 	movx	a,@dptr
      0001BE 20 E3 EF         [24] 1142 	jb	acc.3,00106$
                                   1143 ;	ezusb.c:105: send_state();	// EP6 is not full
      0001C1 12 01 15         [24] 1144 	lcall	_send_state
                                   1145 ;	ezusb.c:107: }
      0001C4 80 EA            [24] 1146 	sjmp	00106$
                                   1147 	.area CSEG    (CODE)
                                   1148 	.area CONST   (CODE)
                                   1149 	.area CONST   (CODE)
      0001E6                       1150 ___str_0:
      0001E6 50 41 30 3D 31        1151 	.ascii "PA0=1"
      0001EB 00                    1152 	.db 0x00
                                   1153 	.area CSEG    (CODE)
                                   1154 	.area CONST   (CODE)
      0001EC                       1155 ___str_1:
      0001EC 50 41 30 3D 30        1156 	.ascii "PA0=0"
      0001F1 00                    1157 	.db 0x00
                                   1158 	.area CSEG    (CODE)
                                   1159 	.area CONST   (CODE)
      0001F2                       1160 ___str_2:
      0001F2 50 41 31 3D 31        1161 	.ascii "PA1=1"
      0001F7 00                    1162 	.db 0x00
                                   1163 	.area CSEG    (CODE)
                                   1164 	.area CONST   (CODE)
      0001F8                       1165 ___str_3:
      0001F8 50 41 31 3D 30        1166 	.ascii "PA1=0"
      0001FD 00                    1167 	.db 0x00
                                   1168 	.area CSEG    (CODE)
                                   1169 	.area XINIT   (CODE)
                                   1170 	.area CABS    (ABS,CODE)
