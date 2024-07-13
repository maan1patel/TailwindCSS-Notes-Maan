Tailwind CSS notes by ~ Maan Patel

* `To setup Tailwind CSS, run these commands on your terminal:`
1) "npm install -D tailwindcss postcss autoprefixer" // install required packages
2) "npx talwindcss init"
3) "npx tailwindcss init -p"
4) "npm install vite" (to run the server)
5) Create a "index.html" file
6) Create a css file "input.css", add it to your html and edit it with this content:
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
7) Add this scipt line: "<script src="https://cdn.tailwindcss.com"></script>" in the <head></head> tag (because to see the suggestions for classes in the html file while coding which makes your work easier)
8) In your tailwind.config.js file replace content: [], with content: ["*"],
9) Add "scripts": {"start": "vite"} to your scripts in package.json
10) Run npm run start command to start a dev server

* `Advantages of using Talwind CSS: `
1) No reinventing of class names required
2) Your CSS doesn't grow with your HTML and Designs 
3) When you make a change, no risk of breaking existing templates 
4) If you try to make a website by using Pure CSS you will get answers to a lot of questions you have about Talwind
5) Will this make your site slow?-NO Will it increase bundle size?-NO 
6) What about responsiveness? Yes it is responsive

* `Classes:`
1) SPACE-X-3 (for giving space in text. Eg: Navbar)
2) PX-3 (for giving paddin in X-axis)
3) PY-2(padding in Y-axis)
4) FLEX (to display the text in flexbox)
5) BG-PURPLE-200 (to add color for the background with dark or light colour by setting it between 0-900)
6) TEXT-RED-900 (to add color to the text)
7) MX-2 (for giving margin in X-axis)
8) MY-3 (margin in Y-axis)
9) PT-2 (padding from top)
10) PB-4 (padding from bottom)
11) PL-6 (padding from left)
12) PR-3 (padding from right)
13) H-14 (height)
14) W-2 or W-1/3 (width)
15) ROUNDED-2XL (to keep a div or a image round)
16) JUSTIFY-END (to start the content from thr end)
17) JUSTIFY-BETWEEN (giving space evenly or space between the text)
18) TEXT-6XL (large text)
19) HOVER-BG-PURPLE-100 (to change the colour or anything while hovering the mouse)
20) ITEMS-CENTER (to keep the items in center)
21) JUSTIFY-CENTER (to keep the content in center)
22) TEXT-LG (To make text large)
23) ORDER-1/2/... (to give the elements order while making the website responsive)
24) INSET-0 (top,bottom,right,left all get 0)
25) ABSOLUTE 
26) STATIC

* `Flex I.M.P classes`
1) FLEX-COL (to make the classes of column in vertical direction)
2) FLEX-COL-REVERSE (to make the classes of column in horizontal direction from vertical)
3) FLEX ROW

* `Width and Height IMP Classes`
1) W-[33rem]
2) H-[23rem]

* `to hide tag in tailwind for responsive devices`
1) max-sm:hidden

* `Fonts and Sizing: `
1) FONT-SANS (Properties: font-family: ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol",  "Noto Color Emoji";)
2) FONT-SERIF (Properties: font-family: ui-serif, Georgia, Cambria, "Times New Roman", Times, serif;)
3) FONT-MONO (Properties: font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;)
4) FONT-BOLD (to make font bold)
5) ITALIC/NON-ITALIC (to make font italic or non intalic)

* `Margin, Padding, Space Between, and Border` 
1) MX-0,... (margin from x-axis)
2) MY-0,... (margin from y-axis)
3) ML-0,... (margin from left)
4) MR-0,... (margin from right)
5) MT-0,... (margin from top)
6) MB-0,... (margin from bottom)
7) SPACE-X-0 (space between elements in X-axis)
8) SPCAE-Y-0 (space between elements in Y-axis)
9) BORDER-SOLID/DOTTED/NONE (giving border with different styles)
10) BORDER-BG-RED-700 (to give color to the border)
11) PX/Y/T/B/L/R-2 (to give padding from all the different sides/ to give padding in the content in the div box)

* `Square Bracket Notation:`
1) mx-[69px] (to give the large sizes to any class or an element. For Eg: w-[])

* `Responsive Designs:` 
1) SM:BG-RED-900 (Minimum width)
2) MD (Medium width)
3) LG (Large width)
4) XLG (Extra Large Width)
5) 2XL (2 Extra Large Width)

* `Buttons: `
1) FOCUS (to change somethng while pressing the tab button or pressing the button or when the cursor is on the button)
2) ACTIVE (to change the properties while pressing button so the user can feel that it is a button)

* `Apply Directive:`
1) @apply (to apply the all classes in one and then applying them to the style.css file and then giving them a name and then applying into HTML classes)

* `Layer Directive:` 
1) @layer (Eg: @layer components) (to make a part of a specific class like components or utilities. To check in the CSS by using inspect option and then checking)

* `When to use @apply and @layer directives: `
~ I personally suggest that use this directives when you need not much then there will be no reason to use talwind css because if you are going to define a lot of classes in style.css then it is going to be a large file and there is no point for talwind css. 

* `Customise your own config file: `
1) npx tailwindcss init maan
~ If you want to access the full file just type in 
2) npx tailwindcss init maan --full

* `Deploying Tailwind Website to Production `: 
1) Add this tag into package.json file into scripts tag: 
    "build": "vite build"
2) npm run build 

