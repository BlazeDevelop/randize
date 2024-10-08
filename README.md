# 🌟 Randize: The Ultimate Python Randomizer Library 🌟

Welcome to **Randize** — your all-in-one solution for generating random data in Python! This library offers a wide variety of functions to produce random numbers, strings, names, emails, colors, coordinates, and much more. Perfect for testing, simulations, and fun projects! 🎉

## 📚 Table of Contents

- [Features](#-features)
- [Installation](#-installation)
- [Usage](#-usage)
  - [Basic Randomization](#basic-randomization)
  - [Advanced Randomization](#advanced-randomization)
- [Examples](#-examples)
- [To-Do](#-to-do)
- [Contributing](#-contributing)
- [License](#-license)

## ✨ Features

- **Random Number Generation**: Generate random integers, floats, dates, times, and UUIDs.
- **Random String Utilities**: Create random strings, passwords, and emails.
- **Data Structure Generators**: Generate random dictionaries, JSON objects, and more.
- **Web Testing Utilities**: Random user agents, URLs, and HTTP request data.
- **Custom Data Mocks**: Random color palettes, coordinates, weather conditions, and more!
- **Flexible API**: Easy-to-use static methods to integrate with your code.

## 🔧 Installation

Install **Randize** via pip:

```bash
pip install randize
```

Or, clone the repository and install manually:

```bash
git clone https://github.com/BlazeDevelop/randize.git
cd randize
pip install -r requirements.txt
```

## 🚀 Usage

### Basic Randomization
First, import the library in your Python script:

```python
from randize import Randize
```

#### Generate a Random Number

```python
random_number = Randize.number(1, 100)  # Returns a random number between 1 and 100
print(random_number)
```

#### Generate a Random Password

```python
password = Randize.password(length=16, include_digits=True, include_punctuation=True)
print(password)  # Example: 'aB3$dEfGhI8!K@Lm'
```

#### Generate a Random UUID

```python
unique_id = Randize.uuid()
print(unique_id)  # Example: '123e4567-e89b-12d3-a456-426614174000'
```

#### Generate a Random Email

```python
email = Randize.email(domain='example.com')
print(email)  # Example: 'john@example.com'
```

#### Generate a Random Name

```python
name = Randize.name()
print(name)  # Example: 'John Doe'
```

#### Generate a Random Date

```python
random_date = Randize.date(start_year=2000, end_year=2023)
print(random_date)  # Example: '2015-06-21'
```

#### Generate a Random Time

```python
random_time = Randize.time()
print(random_time)  # Example: '14:30:45'
```

### Advanced Randomization

#### Create a Random User Profile

```python
user_profile = Randize.struct({
    'name': 'name',
    'email': 'email',
    'birthdate': 'date',
    'address': 'random_coordinate'
})
print(user_profile)
```

#### Generate a Random Payment Card

```python
payment_card = Randize.payment_card()
print(payment_card)
```

#### Generate Random IPv4 Address

```python
ipv4 = Randize.ipv4()
print(ipv4)  # Example: '192.168.1.1'
```

#### Generate Random IPv6 Address

```python
ipv6 = Randize.ipv6()
print(ipv6)  # Example: '2001:0db8:85a3:0000:0000:8a2e:0370:7334'
```

#### Generate Random Color Palette

```python
color_palette = Randize.random_color_palette(n=5)
print(color_palette)  # Example: ['#e91e63', '#9c27b0', '#673ab7', '#3f51b5', '#2196f3']
```

#### Generate Random Geographic Coordinates

```python
coordinates = Randize.random_coordinate()
print(coordinates)  # Example: {'latitude': 40.7128, 'longitude': -74.0060}
```

#### Generate Random Emoji Pair

```python
emoji_pair = Randize.random_emoji_pair()
print(emoji_pair)  # Example: ('😀', '🚀')
```

#### Generate Random Weather Conditions

```python
weather = Randize.random_weather()
print(weather)  # Example: {'condition': 'Sunny', 'temperature': 25, 'humidity': 60}
```

#### Generate Random MAC Address

```python
mac_address = Randize.random_mac_address()
print(mac_address)  # Example: '00:14:22:01:23:45'
```

#### Generate a Random URL

```python
url = Randize.random_url()
print(url)  # Example: 'https://www.example.com/about'
```

#### Generate Random Text with Translation

```python
text = Randize.random_text(language='italian', word_count=10)
print(text)  # Example: Random text in Italian
```

#### Generate Random User-Agent String

```python
user_agent = Randize.random_user_agent()
print(user_agent)  # Example: 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36'
```

## 📋 Examples

Here's a quick example of how you can use **Randize** to generate random data:

```python
# Generate a random color palette
color_palette = Randize.random_color_palette(n=5)
print(f"🎨 Color Palette: {color_palette}")

# Generate a random date between 2000 and 2023
random_date = Randize.date(start_year=2000, end_year=2023)
print(f"📅 Random Date: {random_date}")
```

## 📋 To-Do

- [x] Implement a function to generate random texts.
- [x] Update documentation with examples of using new functions.
- [x] Optimize performance of random data generators.
- [x] Replace random lib to secrets

## 🤝 Contributing

Contributions are welcome! If you have ideas for new features or have found a bug, feel free to [open an issue](https://github.com/BlazeDevelop/randize/issues) or submit a pull request. Please read our [contributing guide](CONTRIBUTING.md) first.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

✨ Happy Randomizing! ✨
