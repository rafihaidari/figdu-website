---
sidebar_position: 5
---

# Menu and Popover

The **Menu** and **Popover** components in Chakra UI are used to create dropdown menus and contextual overlays, respectively. Below are examples and usage guidelines for both components.

---

## Menu

The **Menu** component is used to create dropdown menus that allow users to select from a list of options.

### Basic Usage

Here’s how you can use the `Menu` component to create a dropdown menu:

```jsx title="Menu Example"
import { Button } from "@chakra-ui/react";
import {
  MenuContent,
  MenuItem,
  MenuRoot,
  MenuTrigger,
} from "@/components/ui/menu";

const Demo = () => {
  return (
    <MenuRoot>
      <MenuTrigger asChild>
        <Button variant="outline" size="sm">
          Open
        </Button>
      </MenuTrigger>
      <MenuContent>
        <MenuItem value="new-txt">New Text File</MenuItem>
        <MenuItem value="new-file">New File...</MenuItem>
        <MenuItem value="new-win">New Window</MenuItem>
        <MenuItem value="open-file">Open File...</MenuItem>
        <MenuItem value="export">Export</MenuItem>
      </MenuContent>
    </MenuRoot>
  );
};
```

### Key Props

- **`MenuTrigger`**: The button or element that triggers the menu.
- **`MenuContent`**: The container for the menu items.
- **`MenuItem`**: Represents an individual option in the menu.
- **`value`**: The value associated with each menu item.

---

## Popover

The **Popover** component is used to create contextual overlays that appear when interacting with an element (e.g., a button).

### Basic Usage

Here’s how you can use the `Popover` component to create a contextual overlay:

```jsx title="Popover Example"
import { Button, Input, Text } from "@chakra-ui/react";
import {
  PopoverArrow,
  PopoverBody,
  PopoverContent,
  PopoverRoot,
  PopoverTitle,
  PopoverTrigger,
} from "@/components/ui/popover";

const Demo = () => {
  return (
    <PopoverRoot>
      <PopoverTrigger asChild>
        <Button size="sm" variant="outline">
          Click me
        </Button>
      </PopoverTrigger>
      <PopoverContent>
        <PopoverArrow />
        <PopoverBody>
          <PopoverTitle fontWeight="medium">Naruto Form</PopoverTitle>
          <Text my="4">
            Naruto is a Japanese manga series written and illustrated by Masashi
            Kishimoto.
          </Text>
          <Input placeholder="Your fav. character" size="sm" />
        </PopoverBody>
      </PopoverContent>
    </PopoverRoot>
  );
};
```

### Key Props

- **`PopoverTrigger`**: The button or element that triggers the popover.
- **`PopoverContent`**: The container for the popover content.
- **`PopoverArrow`**: Adds an arrow to the popover for better visual context.
- **`PopoverTitle`**: The title of the popover.
- **`PopoverBody`**: The main content of the popover.

---