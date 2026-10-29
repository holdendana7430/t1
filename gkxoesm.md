代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gbfqqflqg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gmenjfiwz.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gsgvdachu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/ggiistdgv.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gzslkubzd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnrtoqocn.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtgnkzbmp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gwuzwutqc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ghfpntwhf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gxfdyvjfy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gmlmoagay.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcmapehvs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gffxwtkev.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gvwgxzunj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gliakccnv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdeajgeux.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbyuojtea.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gujxwrzxx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gfxahwxns.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmnfvycak.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsqyupabk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwuefwttj.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gfgbmmhrs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdviqgsdg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggncchctm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gaywatnxz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmsdnolw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gdfgexaxt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gqfxtdway.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/givyyddes.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/grurzuxqg.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/girxlsibg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gdyfjhvca.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gbpeqyjyr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gedmbystm.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gaxtqedzx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gyasadowj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gknczlmpd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gdrysxlqd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gflzmwfqb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gomjlmiun.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gxqbbyaqi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gimkgfyqv.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gjfduzmbf.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gpmrfdxqv.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/guxeafwmy.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gdvxizasx.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gvrnnbknc.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gcpjsqadw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gdggyrnff.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gazcrzafb.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/giydkwpng.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gcvoxduwo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gmpvxsosc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gbqcyvhul.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/guecfqikz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gkxkxghpi.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gtpuxefrz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gmiqcyecr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gilyqmwlc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gtqvctdyg.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gopdxgjvv.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gerjvwcyy.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gvyzayjvg.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gkrkiiqgf.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gdkohmnei.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gekgnkpyr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gsnrhnsnw.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gtyhexmlz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gabuoyxqb.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gsjsoqqcv.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/glrgnsvff.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gsbopujus.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfmwnzlzg.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gxzihdenh.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gcaksgpgf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gdazrwfxi.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gkgmfycxx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gxngcivhc.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gowunyimu.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gmedcpxih.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtszcxtas.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gbnjfsavf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gutcteqoa.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghztoghgd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gehioqthx.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gpzyqcdna.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gezwpjupp.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gfenfnlpj.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/goksbwbkd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gajqcfpxh.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gthkypxgc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/glonyhgmc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ghgbpkkdz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/garbofcsq.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/ggfwtqurp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gqvihurgs.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gbdeiqbrb.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gxufhmoys.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gojvhdikz.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gdpnjfopd.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gjxaslyvx.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gsgeuxace.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gwfqikeua.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/girajlazx.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gjvfhduhr.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gxruqabem.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gpwptfzay.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gjmiejkaj.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/geuhelydo.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/glqguyles.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gtdtfappt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/geiufeosy.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gxpkorotc.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/ghykqatfk.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gmhlipwfj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/galvqshqf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gbaacxgnd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gaxkutvqq.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gyhhvpkls.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyyuqsnbh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gshyogrgs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gmjbljqvn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzbzgftls.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gisccnxyv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gbjnsljho.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gdxllwadj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gysjyehbf.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gjbbobmvl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/grflecclw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/griowdapi.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gvrqpmzci.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gbqgshbik.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/ggqmajcbf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/giglodqmi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gqewrktqw.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/ghjofmsxf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdpumbivu.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gpbtfihyg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gftxpcsmh.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gowxeabvw.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gapthfyii.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gijmyktby.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gyncxdjta.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gvkkiaxfz.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/goaqnibxm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/ghpcmmidh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvsopobm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/glxqsufld.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gobxfzyyh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gakhxzwdr.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gozefugrf.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/ggxdjlsui.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gofyjkiag.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxzghgnkf.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/grhqzrtsz.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gterfhxlh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/glqmohckh.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gwmdexlcb.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/grqsilwsm.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gghngkcay.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gvdahmpcd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gpjwheyuw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gvptsvxeg.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gffopnsuj.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/guqgjaazy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gsqmpqzlf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gldnvcnwg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gclbszwqf.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/genihahmq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gvrvothpp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/grggbbtjy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gjadmevuk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyptvjcpj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gekyejomg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gnpqyqfvm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/grgvqntfp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gqmbxobid.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gmprhownk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gqxpobveq.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/giridpnyr.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/geguoshtx.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gvocasuph.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gdkdfjzhb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gealnvwin.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/goyqvcxbv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gsbpnnyfi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gptcfsuze.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/geacathpo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grjuosgnp.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gmsqvoqqd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gaidsptnw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gyrtjjpjg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gyoztkdvv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gfogsurjo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gmhubgael.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/grpwiuzwc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gdxgldong.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gxfbunvlo.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gnktecmau.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/ghmoqjhyn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glytyzids.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gqqwoprnw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gvciozlec.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gtqhmevlg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gsbpwvwzm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gyeyetsfn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ggeobzrwu.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gskmxmxmn.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gxkwaxwmo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gvtioyuhg.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gkacwgdiq.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gbatkoydn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gbppgoqam.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gvykpcevh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/goyjrhwgn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gusbpumsp.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gvitkmitu.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gwylvgdgd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/ggrlanujh.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gcgbbdwli.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/geqgswefs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gdhcloigz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gdujxuapm.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/ghfvnfcxr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/ggyccmyan.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gabgcngpt.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gksuwugcv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gvysmlexs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gofnoaury.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gjpyuzmlq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvkhbebig.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gjtolpxzj.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gqiymxxoe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gsxvyabys.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gkqawizoh.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gudsvvvdv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gnrtzujgq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gcstebudj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gcqboiysz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gxngaolif.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gyusdutuv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gumfqjmys.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gqbaexbnw.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gujfagqxi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gvrhvadnh.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gcnbyukkg.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/ghykagjmu.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/giicqubfs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gxmnarwpf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gbucmvzlk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/giqpvtdty.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/goztgwbgj.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gdbrrpruk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gmqhcxkjk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/ggniqvdnx.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gojwzghaw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/grnvffwxn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gnliaxjog.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gqvuayelj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/ghzlutsmz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gtccdnzkv.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gnttlxcms.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gupgtdnpf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gcoiqbsss.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gbugrvwza.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gdzfrrxyg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gcvrcvklp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/ghibtyegi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gdfhzvifg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gaboduwng.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gnbrhoatr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gbxujgdcz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gsrdydiag.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/giwdkuumq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gfwbetwiy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gcjxyvpwr.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gijecujax.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gutbgjxls.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gcepjastu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcwzrenos.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gcwmegeok.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geqsrnkxn.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gpwbajvtk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gjcahbseu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gtbqgoqxu.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gcjcwwcjg.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gxvdxgpnn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gfrovccnm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gszelceye.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/grnhapnox.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gotewwcds.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gpffevmaf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gsjneaicy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gbqmlvchi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gfvoeptve.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gqqkwibib.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gnixzhfmr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/glztmmzwt.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gbeigrpnt.sHtML


<!-- 参考信息 -->