---
sidebar_position: 2
---

# Layout

Learn how to use Chakra UI's essential layout components: **Container**, **Stack**, **Box**, and **Grid** for Figdu.

## Container

The `Container` component centers and constrains the content width.

```jsx title="Example: Container"
import { Container, Text } from '@chakra-ui/react';

export default function Example() {
  return (
    <Container maxW="container.md" centerContent>
      <Text fontSize="xl">This is a centered container.</Text>
    </Container>
  );
}
```

## Stack

`Stack` helps space out elements vertically or horizontally.

```jsx title="Example: Stack"
import { Stack, Button } from '@chakra-ui/react';

export default function Example() {
  return (
    <Stack spacing={4} direction="row" align="center">
      <Button colorScheme="blue">Button 1</Button>
      <Button colorScheme="green">Button 2</Button>
    </Stack>
  );
}
```

## Box

The `Box` component is a flexible container with style props.

```jsx title="Example: Box"
import { Box } from '@chakra-ui/react';

export default function Example() {
  return (
    <Box p={4} bg="gray.100" borderRadius="md">
      This is a Box component.
    </Box>
  );
}
```

## Grid

Use `Grid` to create a responsive layout.

```jsx title="Example: Grid"
import { Grid, GridItem } from '@chakra-ui/react';

export default function Example() {
  return (
    <Grid templateColumns="repeat(3, 1fr)" gap={4}>
      <GridItem w="100%" h="10" bg="blue.500" />
      <GridItem w="100%" h="10" bg="green.500" />
      <GridItem w="100%" h="10" bg="red.500" />
    </Grid>
  );
}
```