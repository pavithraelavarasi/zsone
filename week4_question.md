# Week 4: HTML & CSS Basics
## Reverse-Engineer the Web's Structure

### Context anchor

In Week 3 you learned that HTML is the skeleton of every web page, CSS is what makes it look the way it looks, and JavaScript is what makes pages do things. You read those as vocabulary terms and placed them on your mental model.

This week you stop reading *about* HTML and CSS and start reading HTML and CSS directly. Not writing it — reading it. The way you would read a foreign-language document for the first time: slowly, figuring out what each piece means from context and observation.

You will open a real webpage, use the browser's built-in inspection tool to look beneath the surface, and document exactly what you find — the structure, the elements, the styles. Everything you document must come from what you observe, not from what you assumed or guessed.

---

### Part A: Choose a page and open the inspector

Pick **one** of the following types of pages to inspect. Do **not** use the four products from Week 1 (Instagram, YouTube, Zomato, Rapido).

- A news article page
- A Wikipedia article
- A government or public-service website
- A university or college homepage

Open the page in Chrome or Firefox. Open the browser's developer tools. Navigate to the panel that shows the page's HTML structure.

**Your Part A document must include:**
1. The page you chose and its URL
2. A screenshot showing the developer tools panel open on that page
3. Written observation: what are the first 3–4 major sections you can identify in the HTML when you look at the top-level structure? Describe what you think each section contains, based only on what you can see in the panel.

Do not describe what the page looks like visually. Describe what the HTML structure shows you.

---

### Part B: Map the HTML structure

Without writing a single line of HTML yourself, read the HTML already on the page and map its structure.

Find and document at minimum:
1. The **main heading** on the page — what tag contains it?
2. At least **3 text blocks** — what tags are they inside?
3. At least **1 image** — what tag contains it? Does it have any attributes visible in the panel? List them.
4. At least **1 link** — what tag is it? What information does the tag carry that tells the browser where to go?
5. **Nesting** — pick one section of the page and draw its structure as an indented list (no code, just indented labels showing what is inside what)

Example of what an indented structure list should look like:
```
Navigation bar
  Logo image
  Link: Home
  Link: About
  Link: Contact
Article section
  Main heading
  Author name
  Publication date
  Paragraph
  Paragraph
  Image with caption
```

This must come from the actual page you chose, not a made-up example.

---

### Part C: Map the CSS styles

When you click on an element in the HTML structure panel, a second panel shows all the CSS styles applied to that element.

Pick **3 different elements** on your chosen page and for each one document:
1. What element it is (e.g. "the main article heading", "the navigation bar", "a paragraph of body text")
2. At least **3 CSS properties** applied to it, and their current values — copy exactly what you see in the styles panel (e.g. `font-size: 24px`, `color: #1a1a1a`, `margin-bottom: 16px`)
3. What **visual effect** each property creates — describe in plain English, not CSS syntax (e.g. "makes the text 24 pixels tall", "sets the text colour to near-black", "adds 16 pixels of space below the element")

Include a screenshot of the styles panel for each element you document.

---

### Part D: Connections and observations

Write a document of minimum 200 words answering all four of these:

1. What was the most **surprising** thing you found when you looked at the HTML or CSS of the page you chose? Why did it surprise you?

2. Pick **one element** on the page. Describe what the page would look like if all CSS was removed from that element. What would visually change? What would stay the same?

3. Did you find any element whose **HTML structure** you did not expect — where what the page looks like visually is quite different from the underlying structure? Describe it.

4. Write **one question** you still have about something you saw in the inspector that you could not figure out.

---

### Deliverables

Submit exactly **3 PDFs** via SSH and SCP to the course server.

**PDF 1 — Structure**
Part A documentation + Part B structure map, with screenshots.

**PDF 2 — Styles**
Part C CSS observations with screenshots of the styles panel for each of the 3 elements.

**PDF 3 — Observations**
Part D written responses.

Place all three files in: `/home/submissions/week4/[your-name]/`

**Filename format:**
- `week4_structure_[yourname].pdf`
- `week4_styles_[yourname].pdf`
- `week4_observations_[yourname].pdf`

---

### Stuck protocol

**If you cannot find the HTML structure panel:** Research "how to open developer tools in Chrome" — there is a keyboard shortcut and a right-click option. Research specifically how to reach the panel that shows the live HTML.

**If you click an element but the styles panel shows nothing:** Make sure you are clicking the element *inside the HTML panel* (on the left), not just clicking on the page itself. The styles panel only populates when an element is selected in the HTML panel.

**If the HTML looks overwhelming and you cannot find a specific element:** Research "how to inspect a specific element on a webpage" — there is a way to right-click directly on the thing you want to inspect on the page and jump straight to it in the panel.

**If the styles panel shows hundreds of properties:** Research "computed vs declared styles" in browser DevTools. There is a way to filter what you see.

Do not ask a classmate what they found on their page — your documentation must reflect your own inspection of your own chosen page.

---

### What will not be accepted

- Use of the four Week 1 products (Instagram, YouTube, Zomato, Rapido)
- Screenshots without the HTML structure panel or styles panel visible
- CSS observations that describe visual appearance only, without the actual property-value pairs from the styles panel
- Structure maps that are not drawn from the actual page you chose
- Vague observations without reference to what you saw in DevTools (e.g. "the heading is big" without naming the CSS property making it big)
- Files submitted via email, WhatsApp, or any method other than SSH and SCP to the course server
