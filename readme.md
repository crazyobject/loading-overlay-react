# LoadingOverlay Component

The `LoadingOverlay` is a customizable react loading overlay component for React applications that enhances user experience with seamless loading indicators. Multiple props which you can set for in detailed customization.

## LiveDemo

[Click here to see it in action](https://stackblitz.com/edit/react-obverlay-loading?file=index.html,src%2FApp.jsx)

## Props

- **`show`** (boolean): Controls the visibility of the overlay.
- **`icon`** (ReactNode): A custom icon to display in the overlay.
- **`text`** (string): Loading message to show.
- **`backgroundColor`** (string): Background color of the overlay (default: `rgba(0, 0, 0, 0.5)`).
- **`zIndex`** (string | number): z-index of the overlay (default: `9999`).
- **`style`** (object): Additional styles to apply to the icon and text.

## Example Usage : with configuration options

```jsx
<LoadingOverlay
  show={loading}
  icon={<i className="fa-solid fa-car-side fa-2x"></i>}
  text="Adding your ride to the pool..."
  backgroundColor="rgba(0, 0, 0, 0.6)"
  zIndex="10000000"
  style={{
    color: "white",
    fontSize: "1.0rem",
    fontWeight: "bold",
  }}
/>
```

## Example Usage : Default/ no configurations

If you don't mention any configurations just like below options then the component will show a default loading icon with text "Loading...".

```jsx
<LoadingOverlay show={loading} />
```
