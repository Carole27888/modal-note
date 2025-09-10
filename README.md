This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.

# Add Note Modal

A React/Next.js modal component for adding notes with user mentions, styled dropdown, and dynamic highlighting.

## Features

- Add notes with a textarea input
- Mention users by typing `@` followed by their name
- Dropdown appears for user selection when typing `@`
- Select users from dropdown with mouse or keyboard
- Insert mention tokens into the note
- Mentions are tracked and can be submitted
- Responsive and accessible UI

## Usage

1. Import and use the `AddNoteModal` component in your Next.js app:

   ```tsx
   import AddNoteModal from "@/components/AddNoteModal";
   // ...
   <AddNoteModal users={usersArray} />
   ```

2. Type `@` in the note textarea to trigger the mention dropdown.
3. Select a user to insert a mention (e.g., `@Carole Mutemi`).
4. Submit the note using the button.

## File Structure

- `src/components/AddNoteModal.tsx`: Main modal component
- `src/components/ui/`: UI primitives (Button, Textarea, etc.)
- `public/`: Static assets

## Customization

- Pass a custom `users` array to the modal for mentionable users.
- Style the modal and dropdown using Tailwind or your own CSS.

## Requirements

- React
- Next.js
- Tailwind CSS (or compatible styling)

## Example User Object

```ts
{
  id: "1",
  name: "Carole Mutemi",
  email: "",
  phoneNumber: "",
  role: "",
  status: ""
}
```


