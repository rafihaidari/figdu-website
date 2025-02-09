---
sidebar_position: 3
---

# Accordion and Collapsible

# Accordion

The **Accordion** component from Chakra UI allows you to display collapsible sections of content, improving both user experience and accessibility. This component is perfect for organizing large amounts of content in a compact format.

## Basic Usage

Chakra UI’s Accordion consists of four main components:

- **AccordionRoot**: The container that holds all Accordion items.
- **AccordionItem**: Represents each individual collapsible section.
- **AccordionItemTrigger**: The clickable title that toggles the section’s visibility.
- **AccordionItemContent**: The content that gets revealed or hidden when the item is toggled.

Here’s how you can set up a basic Accordion in your app:

```jsx title="Basic Accordion Example"
import {
  AccordionItem,
  AccordionItemContent,
  AccordionItemTrigger,
  AccordionRoot,
  Box,
} from "@chakra-ui/react";

const Demo = () => {
  return (
    <AccordionRoot multiple defaultValue={["b"]}>
      {items.map((item, index) => (
        <AccordionItem key={index} value={item.value}>
          <AccordionItemTrigger
            _expanded={{ bg: "blue.500", color: "white" }}
            padding={"10px"}
          >
            {item.title}
          </AccordionItemTrigger>
          <AccordionItemContent>
            <Box p={4}>{item.text}</Box>
          </AccordionItemContent>
        </AccordionItem>
      ))}
    </AccordionRoot>
  );
};

const items = [
  { value: "a", title: "First Item", text: "First section..." },
  { value: "b", title: "Second Item", text: "Second section..." },
  { value: "c", title: "Third Item", text: "Third section..." },
];
```

## Collapsible

The **Collapsible** component is useful when you want to toggle the visibility of a single section of content. It also supports unmounting the content when collapsed, which can be beneficial for performance.

### Basic Usage

Here’s how you can set up a basic Collapsible component in your app:

```jsx title="Basic Collapsible Example"
import { Box, Collapsible } from "@chakra-ui/react";

export const CollapsibleLazyMounted = () => (
  <Collapsible.Root unmountOnExit>
    <Collapsible.Trigger paddingY="3">
      Toggle Collapse (Unmount on exit)
    </Collapsible.Trigger>
    <Collapsible.Content>
      <Box padding="4" borderWidth="1px">
        If you inspect the DOM, you'll notice that the content is unmounted when
        collapsed. This is useful for performance reasons when you have a lot of
        collapsible content.
      </Box>
    </Collapsible.Content>
  </Collapsible.Root>
);
```