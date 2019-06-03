# GraphQL Notes

### Main Advantages

It provides an efficient communication between clients (initially the main target being mobiles where latency and network bandwidth are critical) and servers by considering the following aspects by design:
- data (consumed at least or managed at most) is organized in a graph
- ask what you need (including children or other refs)
    - thus, there is no over-fetching or under-fetching
    - avoided multiple roundtrips (for 1-N relationships)

### Features

- documentation comes by default through Schema Introspection

