# Spring Autowiring

There are five modes of Autowiring supported:

1. `no`
    
    This is the default mode, and it means no autowiring.

2. `byName`

   Spring container tries to match beans by name.

3. `byType`

   Spring container tries to match beans by type.
4. `constructor`


   This mode behaves like `byType`, trying to match the bean with that type as being declared in the constructor's argument.

5. `autodetect`

   In this case, it tries to find a constructor match. If it doesn't find a constructor, then it uses `byType` mode.

Notes:
- Autowiring doesn't support wiring of properties whose data types are primitives (such as bool, int, float, etc).
- `@Autowired` can be used on a setter method, constructor or a field. The autowiring is using `byType` mode.

