# ---> 04 WHITESPACE

## - Spacing system (px)

2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128 /
128 / 132 / 136 / 140 / 144 / 148 / 152 / 156 / 160 /
164 / 168 / 172 / 176 / 180 / 184 / 188 / 192 / 196 / 200

# ---> 01 TYPOGRAPHY SYSTEM

## - Font sizes (px)

10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98

## - Font weights

Default: 400
Medium: 500
Semi-bold: 600
Bold: 700

## - Line heights

Default: 1
Small: 1.05
Medium: 1.2
Paragraph default: 1.6

## - Letter spacing

L1 = -0.5px
L2 = 0.75px

## - System px to rem

html {
/_ font-size: 10px; _/
/_ 10px / 16px = 0.625 = 62.5% _/
/_ Percentage of user's browser font-size setting _/
font-size: 62.5%;
}

# --- 02 COLORS

## COLORS

- Primary:
- Tints:
- Shades
- Accents:
- Greys:
  #555;

# ---> 03 SHADOWS

## SHADOWS

0 2.4rem 4.8rem rgba(0, 0, 0, 0.075);

# ---> 03 BORDER-RADIUS

## BORDER-RADIUS

Default: 9px
Medium: 11px

# ---> 05 CSS Template and Rules

## - links

Put transition on original "state"
transition: background-color 0.3s;

.btn,
.btn:link,
.btn:visited {
display: inline-block;
text-decoration: none;
font-size: 2rem;
font-weight: 600;
padding: 1.6rem 3.2rem;
border-radius: 9px;
border: none;
cursor: pointer;
font-family: inherit;
transition: all 0.3s;
}

.btn--1:link,
.btn--1:visited {
background-color: #e67e22;
color: #fff;
}

.btn--1:hover,
.btn--1:active {
background-color: #cf711f;
}

## - Ul li Css

.ul {
list-style: none;
display: flex;
align-items: center;
gap: 3.2rem;
}
li a{
display: inline-block;
text-decoration: none;
color: #333;
font-weight: 500;
font-size: 1.8rem;
transition: all 0.3s;
}

## - Padding Margin Rule

(padding || margin): top | right | bottom | left ;
(padding || margin): top and bottom | left and right ;
(padding || margin): top | left and right | bottom ;

## - Grid System

.container {
/_ 1140px _/
max-width: 120rem;
padding: 0 3.2rem;
margin: 0 auto;
}

.grid {
display: grid;
column-gap: 6.4rem;
row-gap: 9.6rem;

}

.grid--2-cols {
grid-template-columns: repeat(2, 1fr);
}

.grid--3-cols {
grid-template-columns: repeat(3, 1fr);
}

.grid--4-cols {
grid-template-columns: repeat(4, 1fr);
}

.grid--5-cols {
grid-template-columns: repeat(5, 1fr);
}

.grid--center-v {
align-items: center;
}

## - To add illustrations

.parent{
position: relative;
}
.child{
position: absolute;
}

## - Css for icons

.icon{
color: #e67e22;
height: 3.2rem;
width: 3.2rem;
background-color: #fdf2e9;
margin-bottom: 3.2rem;
padding: 1.6rem;
border-radius: 50%;
}

## - Input css

.input-group {
display: flex;
align-items: center;
background-color: var(--background);
padding: 1.6rem;
border-radius: 0.9rem;
gap: 1.2rem;
}
.input-group i {
font-size: 1.8rem;
color: var(--grey);
}
.search {
outline: none;
border: none;
background-color: transparent;
}

## - Scroll css

#style-4::-webkit-scrollbar-track {
-webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
background-color: #f5f5f5;
}

#style-4::-webkit-scrollbar {
width: 0.2rem;
background-color: #f5f5f5;
}

#style-4::-webkit-scrollbar-thumb {
background-color: var(--color-background);
}

# Progress bar

progress {
display: block; /_ default: inline-block _/
width: 100px;
margin: 2em auto;
background: #444;
height: 12px;
}

/_ webkit _/

progress::-webkit-progress-bar {
background: transparent;
}  
progress::-webkit-progress-value {  
 background: #FFF;

}
