# Oasis User Commands

This will explain the new User Commands which where introduced in version 3.0 of the Oasis Selfbot.

Requirements

- C# 5.0.
- Basic Knowledge of C# is good.

1. Create a new classlib
   - If you use Visual Studio you create a new class library.
   - If you use other IDE's you can create one using `dotnet new classlib -o Oasis` in the Terminal.
2. Namespace and Class names
   - The Namespace should be named `Oasis`
   - The Class should be named `Commands`
   - Thats the only class where commands will be registered
3. Creating first own Command

   ```cs
   public async Task Example(dynamic ctx)
   {
      // See more
      //https://dsharpplus.github.io/api/DSharpPlus.CommandsNext.CommandContext.html

      await ctx.RespondAsync("This is response")
      await ctx.ModifyAsync("This will edit the message")
   }
   ```

   - async is fully supported
   - You can use parameters of type `int, float, ulong, bool, string`

4. Now build the lib with `dotnet build -c release`
5. Put the output dll into the `Data` folder and use the `creload` command
6. Done! You should be able to use these commands just like normal commands.


Your code should look something like this
```cs
using System;

namespace Oasis
{
    public class Commands
    {
        public async Task Example(dynamic ctx)
        {
            // See more https://dsharpplus.github.io/api/DSharpPlus.CommandsNext.CommandContext.html
            await ctx.RespondAsync("This is response")
            await ctx.ModifyAsync("This will edit the message")
        }
    }
}

``` 
