---
sidebar_position: 4
---

# Alert and Dialog

The **Alert** and **Dialog** components in Chakra UI are essential for providing feedback and creating interactive modal dialogs in your application. Below are examples and usage guidelines for both components.

---

## Alert

The **Alert** component is used to display brief, contextual messages to users. It supports different statuses (`error`, `info`, `warning`, `success`) to convey the nature of the message.

### Basic Usage

Here’s how you can use the `Alert` component to display messages with different statuses:

```jsx title="Alert Example"
import { Alert, Stack } from "@chakra-ui/react";

const Demo = () => {
  return (
    <Stack gap="4" width="full">
      <Alert.Root status="error">
        <Alert.Indicator />
        <Alert.Title>There was an error processing your request</Alert.Title>
      </Alert.Root>

      <Alert.Root status="info">
        <Alert.Indicator />
        <Alert.Title>
          Chakra is going live on August 30th. Get ready!
        </Alert.Title>
      </Alert.Root>

      <Alert.Root status="warning">
        <Alert.Indicator />
        <Alert.Title>
          Seems your account is about to expire, upgrade now
        </Alert.Title>
      </Alert.Root>

      <Alert.Root status="success">
        <Alert.Indicator />
        <Alert.Title>Data uploaded to the server. Fire on!</Alert.Title>
      </Alert.Root>
    </Stack>
  );
};
```
### Key Props
- **`status`**: Defines the type of alert (`error`, `info`, `warning`, `success`).
- **`Indicator`**: A visual icon or element that represents the alert status.
- **`Title`**: The main message displayed in the alert.

---

## Dialog

The **Dialog** component is used to create modal dialogs that overlay the main content. It is ideal for confirming actions, displaying additional information, or capturing user input.

### Basic Usage

Here’s how you can create a simple dialog with a title, body, and close button:

```jsx title="Dialog Example"
import { Button } from "@chakra-ui/react";
import {
  DialogBody,
  DialogCloseTrigger,
  DialogContent,
  DialogHeader,
  DialogRoot,
  DialogTitle,
  DialogTrigger,
} from "@/components/ui/dialog";

const Demo = () => {
  return (
    <DialogRoot size="cover" placement="center" motionPreset="slide-in-bottom">
      <DialogTrigger asChild>
        <Button variant="outline" size="sm">
          Open Dialog
        </Button>
      </DialogTrigger>
      <DialogContent>
        <DialogHeader>
          <DialogTitle>Dialog Title</DialogTitle>
          <DialogCloseTrigger />
        </DialogHeader>
        <DialogBody>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </DialogBody>
      </DialogContent>
    </DialogRoot>
  );
};
```

### Key Props
- **`size`**: Controls the size of the dialog (`cover`, `sm`, `md`, `lg`, etc.).
- **`placement`**: Defines where the dialog appears on the screen (`center`, `top`, `bottom`, etc.).
- **`motionPreset`**: Adds animation when the dialog opens/closes (`slide-in-bottom`, `scale`, etc.).
- **`DialogTrigger`**: The button or element that triggers the dialog.
- **`DialogCloseTrigger`**: A button or element to close the dialog.
- **`DialogTitle`**: The title of the dialog.
- **`DialogBody`**: The main content of the dialog.

---