# BabyCAT
Website for the coronagraph demo bench "BabyCAT".

The BabyCAT website is built using the Jekyll framework. Jekyll is a static site generator that allows for easy creation and management of websites.

## Local setup for development

To run the BabyCAT website locally, follow these steps:

1. **Install Jekyll and Bundler**:
   ```sh
   gem install jekyll bundler
   ```

2. **Clone the repository**:
   ```sh
   git clone https://github.com/ivalaginja/babycat.git
   cd babycat
   ```

3. **Install dependencies**:
   ```sh
   bundle install
   ```
## Running the Website Locally

4. **Build the site and make it available on a local server**:
   ```sh
   bundle exec jekyll serve
   ```

5. **Open your web browser and navigate to**:
   ```
   http://localhost:4000
   ```

You should now see the BabyCAT website running locally on your machine.

## Note on Jekyll Version

The Jekyll version 4.2.0 listed in the Gemfile only supports Ruby 3.0.x. The latest version of Ruby 3.0.x is 3.0.7.
