# Password Toggle Feature

This project provides a simple feature to toggle the visibility of a password input field using an eye icon. It allows users to view or hide the password they enter, improving the user experience for forms that require password input.

## Features
- Toggle password visibility by clicking the eye icon.
- The input field type changes dynamically between `password` and `text` based on the user's interaction.
- Uses Font Awesome icons for the eye (open/closed) toggle.
- Tailwind CSS is used for styling the input and button.

## Requirements
To run this feature, you need the following dependencies:

- **jQuery**: For DOM manipulation and event handling.
- **Font Awesome**: To use the eye icons for toggling visibility.
- **Tailwind CSS**: For styling the password input and button.

### How to Use:
**html setup**
```html
<div class="border-b-2 border-gray-300 dark:border-gray-600 focus-within:border-blue-600 transition-colors">
  <input type="password" name="new_password" id="new_password"
         class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent focus:ring-0 border-none focus:outline-none dark:text-white peer"
         placeholder=" " value="Password123" required />
  <label for="new_password"
        class="peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:start-0 rtl:peer-focus:translate-x-1/4 peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">
        Password
  </label>
  <button type="button" data-toggle="togglePassword" data-toggle-eye="new_password"
          class="absolute right-0 top-2 text-gray-500 dark:text-gray-400">
          <i data-toggle-eye-icon="new_password" class="fa-regular fa-eye"></i>
  </button>
</div>

