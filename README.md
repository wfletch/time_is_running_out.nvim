# Time Is Running Out ⏳

Simple Reminder that just being alive is not living.

I guess you could also use this as a reminder to any specific date.

---

## ✨ Features

- Runs on Neovim startup
- Optional **once-per-day** notification
- Optional integration with `nvim-notify`

---

## 📦 Requirements

- Neovim 0.9+
- Python 3.8+
- (Optional) [`rcarriga/nvim-notify`](https://github.com/rcarriga/nvim-notify)

---

## 🔧 Installation (Lazy.nvim)

### From GitHub

```lua
return {
    "wfletch/time_is_running_out.nvim",
    event = "VimEnter",
    config = function()
        require("time_is_running_out").run({
        end_date = "2070-12-31 23:59:59",
        delta = "days",
        only_once_per_day = true
    })
end,
}
