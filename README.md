# Skidbar Table

**Skidbar Table** is a simple Lua/Luau table format for storing and exposing scripts as commands/actions.

Each entry contains a name, description, and callback. The callback receives a `pass` object and uses the stored function to execute the selected script.

## Table Format

```lua
{
	name = "Example",
	description = "Lorem ipsum",
    callback = function(pass)
  		runcallbackviatable(pass.owner,pass.args[1],function(p)
  				v.func(p.Name)
    end)
	end,
}
```
## License

MIT, see `LICENSE`.
