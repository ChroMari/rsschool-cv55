<h1 align="center">Khromova Maria Alekseevna</h1>
<h6 align="center"> Junior Frontend Developer</h6>

<hr>

mail: chromarija@gmail.com <br>
diskord: @Mari Rouse#0371 <br>

<hr>

<h2>About me</h2>

I love to work and I love the dynamics in my development. I am a person who loves aesthetics, so I try to do my work not only internally at good quality, but also externally reflect the beauty and elegance of the project. I like to code, by trial and error, I realized that this is what I want to do for 10 years.
<br>
I try to help other people by explaining and guiding them. I have a small vocation for pedagogy; I bring up even the most complex and confusing material for others.
<br>
I want to bring benefit and beauty to people with my work, so that when they see the project, they forget about the bad and gray in their lives and realize that there is a place for everyone in life.
<br>
I know how to build my own personal learning plan and like to study topics in depth, not dwelling on the superficial knowledge that is needed to solve a problem and create a project.
<br>

<h2>Skills</h2>

 - **HTML5** - <font style="vertical-align: inherit;">✅</font> <font style="vertical-align: inherit;">✅</font> <font style="vertical-align: inherit;">✅</font> <font style="vertical-align: inherit;">✅</font> 
 - **CSS (SASS)** - <font style="vertical-align: inherit;">✅</font> <font style="vertical-align: inherit;">✅</font> <font style="vertical-align: inherit;">✅</font> <font style="vertical-align: inherit;">✅</font>
 - **VAVASCRIPT** - <font style="vertical-align: inherit;">✅</font> <font style="vertical-align: inherit;">✅</font> <font style="vertical-align: inherit;">✅</font> <font style="vertical-align: inherit;">✅</font>
 - **TYPESCRIPT** - <font style="vertical-align: inherit;">✅</font> <font style="vertical-align: inherit;">✅</font>
 - **REACT** - <font style="vertical-align: inherit;">✅</font>

<h2>Example code</h2>

```typescript 
  class CanvasWrapper {
  canvas: HTMLCanvasElement;

  ctx: CanvasRenderingContext2D | null;

  img: HTMLImageElement;

  filtersCanvas: IfilterCanvas;

  resultFiltersCanvas: string;

  constructor() {
    this.canvas = document.createElement('canvas');
    this.ctx = this.canvas.getContext('2d');

    this.img = new Image();
    this.filtersCanvas = filtersCanvas;
    this.resultFiltersCanvas = '';
  }

  filtering = (titleFilter: string, valueFilter: string, unitFilter: string): void => {
    const title = titleFilter.toLowerCase().replace(' ', '_');
    this.filtersCanvas[title] = `(${valueFilter}${unitFilter})`;
    this.resultFiltersCanvas = '';
    const keys = Object.keys(this.filtersCanvas);
    keys.map((key) => {
      this.resultFiltersCanvas += `${key.replace('_', '-')}${this.filtersCanvas[key]} `;
      return key;
    });

    this.resultFiltersCanvas = this.resultFiltersCanvas.trim();
    if (this.ctx) this.ctx.filter = this.resultFiltersCanvas;
    this.ctx?.clearRect(0, 0, this.canvas.width, this.canvas.height);
    this.ctx?.drawImage(this.img, 0, 0);
  };

  save = (): void => {
    const a = document.createElement('a');
    a.href = this.canvas.toDataURL();
    a.download = 'image.png';
    a.click();
  };

  drawing = (img: HTMLImageElement): void => {
    this.img.setAttribute('crossorigin', 'anonymous');
    this.img.src = img.src;
    this.img.onload = () => {
      this.canvas.width = img.width;
      this.canvas.height = img.height;

      this.ctx?.clearRect(0, 0, this.canvas.width, this.canvas.height);
      if (this.resultFiltersCanvas.length !== 0 && this.ctx)
        this.ctx.filter = this.resultFiltersCanvas;
      this.ctx?.drawImage(this.img, 0, 0);
    };
  };

  render = (): HTMLCanvasElement => this.canvas;
}
```

<h2>work experience</h2>

  - Photofilter - application allowing you to edit images. Working with images is done using canvas rendering. Also during development, webpack, typescript, sass were used. Eslint was responsible for following the rules when writing the application <br>
    demo link: https://rolling-scopes-school.github.io/chromari-JSFEPRESCHOOL/photofilter/
 
<h2>Education</h2> 

Period of study | Institution name
------------ | -------------
2004-2015 | MOU Lyceum (with a physical and mathematical bias)
2015-2019 | Vladimir State University A.G. and N.G. Stoletovs (Information Security)
2020 | Coursera (Moscow Institute of Physics and Technology, Yandex, Interface Development: Layout and JavaScript)
2020 | Coursera (Hong Kong University of Science and Technology, Full-Stack Web Development with React)
2021 | RS school pre-school javascript
    
<h2>language</h2>

 - English A1+
 - Japan N5
