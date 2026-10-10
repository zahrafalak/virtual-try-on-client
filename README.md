# Virtual Try-On for Google Shopping

A front-end prototype built in a weekend at a **BrainStation × Google hackathon** (April 2024).

## The challenge

Google asked teams to solve a real problem with one of its products, and named **data privacy and security** as a key concern. Projects were presented to and evaluated by Google representatives.

Our team of developers, UX designers and data scientists chose **Google Shopping's virtual try-on**: helping shoppers see how a dress would look on a body like theirs.

## The idea: privacy by design

- The shopper takes a photo and enters their measurements.
- The feature builds a **silhouette** from the photo and measurements, then **discards the photo**. It stays on the shopper's phone and never reaches Google's servers.
- The silhouette is matched to the **closest model in Google's existing lineup**, so the shopper sees the dress on a similar body shape and size.

While working on the matching, we noticed the model lineup lacked diversity in height, size and ethnicity. We recommended Google broaden it, which would also make the matches more accurate.

## What's in this repo

A clickable React prototype of the shopper's flow, built from our designers' Figma mockups:

1. A short tutorial
2. **Taking a photo**, with an animated "silhouette in creation" preview
3. Entering height and measurements
4. Seeing the dress on the matched model, with the option to proceed to purchase

The silhouette building and model matching were the concept we presented; they aren't implemented here. The chosen photo isn't uploaded or stored anywhere.

**Built with:** React, React Router, SCSS, Material UI, Create React App.

## My part

I proposed the silhouette approach, which the team adopted. I built the photo flow in React and SCSS:

- [#1 Photo upload component](https://github.com/mayteles/virtual-try-on-client/pull/1): the photo step with the animated silhouette preview
- [#7 Photo upload](https://github.com/mayteles/virtual-try-on-client/pull/7): the upload page, camera icon and routing
- [#8 Primary call-to-action styling](https://github.com/mayteles/virtual-try-on-client/pull/8)

**Team developers:** [@mayteles](https://github.com/mayteles), [@BeccaVin](https://github.com/BeccaVin), [@laur-af](https://github.com/laur-af) and me, working with our UX designers and data scientists.

This is my fork of the team repository, [mayteles/virtual-try-on-client](https://github.com/mayteles/virtual-try-on-client).

## Running it locally

```bash
npm install
npm start
```

Then open http://localhost:3000.
