# Snapper Safe
Snapper Wrapper built with safety in mind

## Prerequisites
- Your brain 🧠, some courage if something breaks 😛.
---


## Compatibility
- Linux with snapper installed (obviously, what did you think?)
---

## Instructions
1.  **Get the wrapper script**:
    ```bash
    curl -O https://raw.githubusercontent.com/sannidhyaroy/snapper-safe/refs/heads/main/snapper-safe
    ```
2.  **Move it**:
    ```bash
    sudo mv -v snapper-safe /usr/local/bin/snapper-safe
    ```
3.  **Setup aliases**:
    Set the following alias for your preferred shell:
    ```bash
    alias snapper='sudo /usr/local/bin/snapper-safe'
    ```
4.  **Use Snapper Commands without sudo**:
    The next time you run snapper, use it without `sudo` to use the wrapper script.
5.  **Profit!!**
---

## Life = Pain
This wrapper script was made when I accidentally broke my system while intending to perform a `sudo snapper -c home undochange 12..0`, then noticed that I hadn't passed the required snapper config (`sudo snapper undochange 12..0`), essentially breaking the root subvolume.

---

## License
Snapper Safe is licensed under [The Unlicense](https://github.com/sannidhyaroy/snapper-safe/blob/main/LICENSE).