## 📌 What is JSX, and why is it used?

**উত্তর:**

- JSX মানে হলো JavaScript XML। এটি React-এর মধ্যে ব্যবহৃত একটি syntax extension, যা JavaScript কোডের মধ্যে HTML-এর মতো structure লিখতে দেয়।

### 1) `What is JSX?`

- JSX হলো এমন একটি syntax যা দেখতে অনেকটা HTML-এর মতো, কিন্তু এটি JavaScript-এর মধ্যেই লেখা হয়। এই কোডটি আসলে JavaScript-এর React.createElement() ফাংশনের একটি shorthand। JSX ব্যবহার করলে কোড লেখা সহজ হয় এবং UI structure পরিষ্কারভাবে বোঝা যায়।

### 2) `why is it used?`

- HTML-এর মতো syntax ব্যবহার করে UI component গুলো সহজে বোঝা যায়। JSX-এর মধ্যে JavaScript expression ব্যবহার করা যায় {} এর মাধ্যমে। JSX component তৈরি ও nested structure handle করতে সহজ করে তোলে।

---

## 📌 2. What is the difference between State and Props?

**উত্তর:**

- React-এ State এবং Props দুইটি component-এর data handle করার জন্য ব্যবহৃত করা হয়।

### 1) `Props`

- Props হলো component-এর বাইরে থেকে পাঠানো data। এগুলো parent component থেকে child component-এ পাঠানো হয়। Component এ props পরিবর্তনযোগ্য নয় (immutable)। Parent → Child data flow — উপর থেকে নিচের দিকে component-এ data পাঠায়। একই component বিভিন্ন props ব্যবহার করা যায়।

### 2) `State`

- State হলো component-এর নিজস্ব data, যা component নিজেই পরিবর্তন করতে পারে। Component এ ‍state পরিবর্তনযোগ্য (mutable)। এর ভিতরে declare করা যায় এবং UI পরিবর্তনের জন্য ব্যবহৃত হয়। User interaction বা event-এর মাধ্যমে পরিবর্তন করা যায়

---

## 📌 3. What is the useState hook, and how does it work?

**উত্তর:**

- useState হলো React-এর একটি Hook, যা functional component-এর ভিতরে state ব্যবহারের করা যায়।

### 1) `What is the useState hook`

- useState ব্যবহার করে component-এর ভিতরে এমন data রাখা যাবে যা পরে পরিবর্তিত করা যাবে — যেমন: button click করলে counter বাড়ানো, input field-এর মান পরিবর্তন ইত্যাদি।

### 2) `how does it work`

- Component-এর ভিতরে dynamic data handle করা যায়। UI update করতে user interaction অনুযায়ী মান পরিবর্তন করা যায়।

## 📌 4. How can you share state between components in React?

**উত্তর:**

- React-এ component গুলোর মধ্যে state শেয়ার করার কয়েকটি উপায় আছে, যেগুলো নির্ভর করে তোমার application-এর জটিলতা ও structure-এর উপর। যখন দুই sibling component-এর মধ্যে state শেয়ার করতে হয়, তখন state-কে তাদের common parent component-এ নিয়ে যাওয়া হয়। যখন অনেক nested component-এর মধ্যে state শেয়ার করতে হয়, তখন Context API ব্যবহার করা হয়। এবং Context API ব্যবহার করলে prop drilling এড়ানো যায়।

---

## 📌 5. How is event handling done in React?

**উত্তর:**

- React-এ event handling মানে হলো ইউজারের interaction (যেমন: click, input, mouse move ইত্যাদি) ধরার জন্য function ব্যবহার করা। এটি HTML-এর মতোই কাজ করে, কিন্তু React-এ কিছু পার্থক্য আছে। Event attribute গুলো camelCase হয়। Function reference দেওয়া হয়, string নয়। React এ Arrow function ব্যবহার করলে this binding নিয়ে চিন্তা করতে হয় না। Prevent default behavior করতে চাইলে e.preventDefault() ব্যবহার করলেই হয়। Multiple event handler চাইলে function-এর ভিতরে logic ভাগ করা যায়।
