# Step by step instructions on how to setup Django environment

The instructions are based on the `shell` files in this repository.
Each sub-section is based on one file from the shell files and some additional info if needed.

This is for making it easy to copy the instructions provided in the shell files.

## 1. Create a directory

First, create a directory where your Django project will reside.

```bash
mkdir Foldername
```

## 2. Change directory

Navigate into the directory you just created.

```bash
cd Foldername
```

## 3. Install Virtualenvironemt

Install `virtualenv`, a tool to create isolated Python environments.

- Using `pip`:

    ```bash
    pip install virtualenv
    ```
- If you are in a externally managed environment like in Arch Linux then you can try

    ```bash
    pacman -S python-virtualenv
    ```
- If it fails you can try

    ```bash
    pip install virtualenv --break-system-packages
    ```

- **Note:** If it fails again, then you are using Linux, we trust in you.

## 4. Create virtualenv

Create a virtual environment to isolate your project dependencies.

```bash
python -m virtualenv name
```

## 5. Activate virtualenv

Activate the virtual environment.

```bash
name/scripts/activate
```

If the script is not there, then look it maybe in `bin` or somewhere, you know what you are doing right?

## 6. Install Django

Once the virtual environment is activated, install Django.

```bash
pip install django
```

## 7. Start Django Project

Create a new Django project using `django-admin`.

```bash
django-admin startproject (Projectname)
```

## 8. Change Directory

Navigate into your new project directory.

```bash
cd (Projectname)
```

## 9. Run the Django Development Server

Start the development server to ensure everything is set up correctly.

```bash
python manage.py runserver
```

## Aftermath

Edit your files and enjoy the development process. Good Luck!
