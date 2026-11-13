# Auréllia Beauty

Auréllia Beauty is a responsive, multi-page website for a beauty and personal-care brand based in Accra, Ghana. The project presents the brand's identity, showcases skincare, makeup, fragrances, and haircare collections, and provides a simple way for visitors to make enquiries.

The site uses the tagline **"The Art of Beautiful Living"** to communicate a focus on confidence, elegance, self-care, and personal expression.

## Project Overview

This project is a front-end showcase for Auréllia Beauty. It is built as a lightweight static website, so it can be opened locally, hosted on a static hosting service, or expanded later with JavaScript and a backend service.

### Main Features

- A shared, responsive design across all four pages
- Brand-focused home page with an introductory hero area
- Product-category previews for skincare, makeup, perfumes, and haircare
- Shop page featuring product collections and promotional videos
- About page explaining the brand's purpose and values
- Contact form with labelled fields and basic browser-side validation
- Consistent header, navigation, footer, colors, typography, and spacing
- Accessible foundations, including page language, image alternative text, and form labels
- Lightweight implementation using only HTML and CSS

## Pages

### `index.html` — Home

The home page introduces the brand with a logo, hero message, and call-to-action link. It also introduces the company's self-care philosophy, previews the main product categories, and encourages visitors to learn more or make contact.

### `shop.html` — Shop

The shop page displays three featured collections:

- Skincare Essentials
- Makeup Collection
- Luxury Fragrances

Each collection includes an image, a short description, and a **Shop Now** link. Because this is currently a static website, those links direct visitors to the contact page so they can enquire about the products. The page also includes two autoplaying, looping promotional videos with playback controls.

### `about.html` — About Us

The About Us page presents the Auréllia Beauty story and explains the brand's mission: bringing together quality beauty products, personal care, and inspiring experiences that help customers celebrate their own beauty.

### `contact.html` — Contact

The contact page provides a simple enquiry form for a visitor's name, email address, and message. The fields use explicit labels and the `required` attribute for basic validation. The form currently uses placeholder processing settings, so a server-side or third-party form endpoint must be connected before messages can be delivered.

## Technology

- **HTML5** for page structure and content
- **CSS3** for layout, colors, typography, responsive grids, and interactive states
- **No JavaScript dependencies** are currently required
- **No build step or package installation** is needed

## Project Structure

```text
First-project/
├── index.html          # Home page
├── about.html          # About Us page
├── shop.html           # Shop and product collections
├── contact.html        # Contact form
├── css/
│   └── styles.css      # Shared styling for all pages
├── images/
│   ├── Aurellia Beauty logo.png
│   ├── favicon.ico
│   ├── product1.png
│   ├── product2.png
│   └── product3.png
├── video/
│   ├── video_1.mp4     # First promotional shop video
│   └── video_2.mp4     # Second promotional shop video
└── README.md
```

## Getting Started

Because the site uses relative paths for its stylesheet, images, video, and page links, it is best to run it through a local web server.

### Prerequisites

- A modern web browser
- [Python 3](https://www.python.org/) (optional, but recommended for running a local server)

### Run Locally with Python

From the project directory, start Python's built-in HTTP server:

```bash
python3 -m http.server 8000
```

Then open the following address in your browser:

```text
http://localhost:8000
```

You can also open `index.html` directly in a browser, but a local server more accurately represents how the site will behave when hosted.

## Customization

### Change Colors and Fonts

The site's shared visual styles are defined in `css/styles.css`. Common brand colors appear in variables such as:

- `#f8e5df` — light header background
- `#f4dcd6` — hero background
- `#a66c50` — primary button and heading color
- `#704b3d` — navigation text and hover state
- `#68483e` — footer background

The main font family is also selected in `styles.css` and can be changed there.

### Update Page Content

- Edit `index.html` for the home-page content.
- Edit `shop.html` to add or update product collections.
- Edit `about.html` to revise the brand story.
- Edit `contact.html` to change the enquiry fields.
- Update the shared footer and navigation separately in each HTML file, as this project does not currently use a templating system.

### Add a Product

1. Add the product image to `images/`.
2. Add a new `<li class="grid-item">` inside the product list in `shop.html`.
3. Include useful `alt` text that describes the image.
4. Point the product's link to the contact page or, in a future version, a dedicated product page.

### Connect the Contact Form

Replace the placeholder `action` and `method` values in `contact.html` with the endpoint provided by your chosen form service or backend. Include a success or confirmation message so visitors know that their enquiry was received.

## Assets

- The main logo is stored at `images/Aurellia Beauty logo.png`.
- Product images are stored as `product1.png`, `product2.png`, and `product3.png`.
- The promotional videos are stored as `video/video_1.mp4` and `video/video_2.mp4`.
- The browser-tab icon is stored as `images/favicon.ico`.

Keep asset filenames and paths consistent with those referenced in the HTML, or update the corresponding `src` and `href` attributes when renaming files.

## Accessibility and Browser Support

The website is designed for modern browsers and includes several accessibility improvements:

- English is declared with the `lang` attribute.
- Images include descriptive alternative text.
- Form controls have associated labels.
- Required fields are identified for browsers and assistive technology.

- Semantic elements such as `header`, `nav`, `main`, `section`, and `footer` are used throughout the pages.

If more pages are added, keep heading levels in a logical order and ensure every interactive element can be reached and understood with a keyboard.

## Current Limitations

- This is a static front-end project with no database or backend.
- The contact form is not connected to a service that delivers messages.
- Product links currently lead to the contact page rather than individual product pages.
- The shared header and footer are repeated across pages rather than generated by a component or template.
- There is currently no automated test setup or build pipeline.

## Contact

**Auréllia Beauty**
Accra, Ghana
Email: `aurelliabeauty@gmail.com`

## License

This project is intended for the Auréllia Beauty website. All rights are reserved unless a different license is added by the project owner.
