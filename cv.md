<h1 align="center">Khromova Maria Alekseevna</h1>
<h6 align="center"> Junior Frontend Developer</h6>

<hr>

почта: chromarija@gmail.com <br>
diskord: @Mari Rouse#0371 <br>

<hr>

<h2>About me</h2>

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
Краткая информация о себе (ваша цель и приоритеты, подчеркните свои сильные стороны, расскажите о своём опыте работы, если опыта работы нет, расскажите о своём стремлении и способности быстро учиться и узнавать новое)

<h2>work experience</h2>

  - Photofilter - приложение позволяющие редактировать изображения. Работа с изображениями происходит при помощи отрисовки через canvas.Также в ходе разработки был использован webpack, typescript, sass. За соблюдение правил при написание приложения отвечал Eslint. <br>
    ссылка на демо: https://rolling-scopes-school.github.io/chromari-JSFEPRESCHOOL/photofilter/
    
  - Vertical-sounds slider - 
    
Опыт работы. Junior Dev может указать пройденные курсы и тренинги, перечислить учебные проекты, или проекты, выполненные на фрилансе с указанием использованных навыков и ссылками на исходный код.
Образование (включая курсы, семинары, лекции, онлайн-обучение)
Английский язык (уровень английского языка, если была языковая практика, расскажите о ней)
