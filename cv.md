# RSSchool CV
# Grigorii Kurdzheli
## My Contact Info
- E-mail: pappoy256@yandex.ru
- GitHub: [pappoy256](https://github.com/Pappoy256)
- Telegram: [ternoho](https://t.me/Ternoho)
## About me
I'm 25 years old, and programming, as a symbiosis of creative and technical fields, has always been of interest to me. However, this interest was more of a background one, and I had never actively pursued a career in this field. That was the case. 

Now, I have some free time and, more importantly, a desire to develop a new skill. I've always found it challenging to choose something specific from a vast selection, so this time, I decided to make a quick decision without delving into thoughts or comparisons. My choice was frontend development. 

I believe that this will be at least an interesting adventure, and although I have no expectations, who knows what it will lead to? Great things often start with small steps. Among the aspects of my personality that I consider strong, I am known for my perseverance, attention to detail, and love for challenging and engaging tasks that I enjoy completing.
## Skills
- HTML on a very basic level
- CSS on a basic level too
- Git and GitHub
- C language
- VSCode as an editor
## Code example
Fragment from my realization of [magma cipher](https://www.ietf.org/rfc/rfc8891.pdf)
```
void magma_t_algorithm(const uint32_t in_data_block_half, uint32_t *out_data_block_half)

{
    uint8_t data_part[4];

    // Разбиваем 32 битный блок на 4 блока по 8 бит;
    data_part[0] = in_data_block_half & 0x000000ff;
    data_part[1] = (in_data_block_half & 0x0000ff00) >> 8;
    data_part[2] = (in_data_block_half & 0x00ff0000) >> 16;
    data_part[3] = (in_data_block_half & 0xff000000) >> 24;
  
    uint8_t byte_first_half, byte_second_half;

    for (int i = 0; i < 4; i++)
    {
        byte_first_half = s_box[i * 2][data_part[i] & 0x0f]; // Младший полубайт
        byte_second_half = s_box[i * 2 + 1][(data_part[i] & 0xf0) >> 4]; // Старший полубайт

        *out_data_block_half |= (byte_first_half | (byte_second_half << 4)) << (i * 8);

    };
};
```
## Education
### [freecodecamp.org](https://www.freecodecamp.org/)
- HTML/CSS course (in progress)