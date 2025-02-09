---
sidebar_position: 7
---

# Tabs and Table

The **Tabs** and **Table** components in Chakra UI are used to organize content into tabbed views and display data in a structured format, respectively. Below are examples and usage guidelines for both components.

---

## Tabs

The **Tabs** component is used to create tabbed interfaces, allowing users to switch between different views or sections of content.

### Basic Usage

Here’s how you can use the `Tabs` component to create a tabbed interface:

```jsx title="Tabs Example"
import { Link, Tabs } from "@chakra-ui/react";

const Demo = () => {
  return (
    <Tabs.Root defaultValue="members">
      <Tabs.List>
        <Tabs.Trigger value="members" asChild>
          <Link unstyled href="#members">
            Members
          </Link>
        </Tabs.Trigger>
        <Tabs.Trigger value="projects" asChild>
          <Link unstyled href="#projects">
            Projects
          </Link>
        </Tabs.Trigger>
      </Tabs.List>
      <Tabs.Content value="members">Manage your team members</Tabs.Content>
      <Tabs.Content value="projects">Manage your projects</Tabs.Content>
    </Tabs.Root>
  );
};
```

### Key Props

- **`defaultValue`**: Sets the initially active tab.
- **`Tabs.List`**: The container for the tab triggers.
- **`Tabs.Trigger`**: Represents a tab trigger (e.g., a button or link).
- **`Tabs.Content`**: The content associated with each tab.

---

## Table

The **Table** component is used to display data in a structured, tabular format. It supports features like sticky headers and scrollable areas.

### Basic Usage

Here’s how you can use the `Table` component to display data:

```jsx title="Table Example"
import { Table } from "@chakra-ui/react";

const Demo = () => {
  return (
    <Table.ScrollArea borderWidth="1px" rounded="md" height="160px">
      <Table.Root size="sm" stickyHeader>
        <Table.Header>
          <Table.Row bg="bg.subtle">
            <Table.ColumnHeader>Product</Table.ColumnHeader>
            <Table.ColumnHeader>Category</Table.ColumnHeader>
            <Table.ColumnHeader textAlign="end">Price</Table.ColumnHeader>
          </Table.Row>
        </Table.Header>

        <Table.Body>
          {items.map((item) => (
            <Table.Row key={item.id}>
              <Table.Cell>{item.name}</Table.Cell>
              <Table.Cell>{item.category}</Table.Cell>
              <Table.Cell textAlign="end">{item.price}</Table.Cell>
            </Table.Row>
          ))}
        </Table.Body>
      </Table.Root>
    </Table.ScrollArea>
  );
};

const items = [
  { id: 1, name: "Laptop", category: "Electronics", price: 999.99 },
  { id: 2, name: "Coffee Maker", category: "Home Appliances", price: 49.99 },
  { id: 3, name: "Desk Chair", category: "Furniture", price: 150.0 },
  { id: 4, name: "Smartphone", category: "Electronics", price: 799.99 },
  { id: 5, name: "Headphones", category: "Accessories", price: 199.99 },
];
```

### Key Props

- **`stickyHeader`**: Makes the table header sticky when scrolling.
- **`size`**: Controls the size of the table (`sm`, `md`, `lg`, etc.).
- **`Table.Header`**: The container for the table header row.
- **`Table.Row`**: Represents a row in the table.
- **`Table.ColumnHeader`**: Represents a column header.
- **`Table.Body`**: The container for the table rows.
- **`Table.Cell`**: Represents a cell in the table.

---
