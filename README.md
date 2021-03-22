# 💰 Surprise

## Código fonte do artigo: https://khalidabuhakmeh.com/html-buttons-are-under-appreciated-in-asp-dot-net-core

![Surprise game](https://d33wubrfki0l68.cloudfront.net/952d2b5350da86b3b44b3bdeae2741f7785041ac/bc902/assets/images/posts/html-buttons/html-button-playing.gif)

> HTML buttons are one of the most under-appreciated components of modern web forms. ASP.NET Core developers see the button as a way to submit a form of input elements like text boxes, selects, and radio buttons. I’m here to tell you that buttons are so much more versatile. In this short post, I’ll write a simple yet fun guessing game using ASP.NET Core Razor Pages, HTML, and CSS.

> HTML buttons can hold and transmit data like any other HTML form input. Think text boxes, selects, and radio buttons.

```html
<form asp-page="Index" method="post">
    <div class="parent">
        @for (int i = 1; i < 10; i++)
        {
            <div class="box @($"box{i}")">
                <button 
                    type="submit" 
                    name="box" 
                    value="@(i)"
                >
                    🎁
                </button>
            </div>
        }
    </div>
</form>
```
