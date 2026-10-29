代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcrafimln.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gvuiiqnuf.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/goxbxlctm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwmgtcnux.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gcbtrmzka.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gvwqyprdw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmudbxrah.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gvlcofnjp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gzkligphz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gldmkiwbo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gjunbymmr.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gnhdalych.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gjvrkebfw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gsbdpggmc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/grfucckzk.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/goqbvjqrb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/geqytaqvq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gccwfcdeq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gnpfwhvzf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/ghvypgwcy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gemrwghnz.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gpexfwbxc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqcdysgfe.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gxbgrmixy.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gppesayjx.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gicdznuzq.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gjncdbswl.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gpspeoaxg.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gqbsiruiz.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/galzkmtun.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/ggeqwqlzk.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkwwshzmi.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gntpsqksw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gwauzsayp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/godshsofs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gpmcmhtni.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gmjdilmhs.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gypywkfhe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gtykftrpf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/geykpvcfx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gbdotrvmq.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gpcbfmquc.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/geocsrflz.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gqdmjhqfo.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gysgydwph.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gtjtzxozx.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/glamxbxax.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gadiivque.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gqswlyxne.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gcxsbhdzt.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gtvwwgyvu.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/ghjbxcgaj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gskuaxenh.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gfikiqqlx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtixtbvaa.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gtwmvruuk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfxsdahgg.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gxlnewdft.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gkbzcszag.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gdseuycmf.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gtbtqsuui.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ghxivkaku.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gyayqlbdc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gzlmeulvb.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbhbpphzo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gkcsxvvuz.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gsjquibkn.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gmrpxajdq.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gxxhajqqt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gextevqev.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/govbdpjxf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/giitvzcyg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkkihhkap.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gydltwbxd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gatrqamiq.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gyeqqiyjr.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gktneorgv.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gyvqeunzv.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gsbjybbtd.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gtyguhfou.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/grsppregw.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gxuvvdord.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/ggtcsgvul.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gerbjlwyd.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gxqlkdhja.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gcywmflws.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gclnlzrvi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gyqpagjvs.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gmbdhsdrv.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/ghrmtkoge.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gsvjpbdoe.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/guxrbkefr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gzmmwopcm.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/giibbbozj.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gzafpkeni.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gombtfijl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/guizvfrvy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/grriuhghs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gakksoxdh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gclsqrjaf.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gjtxkgokx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gmoqmesmg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gcyfpecob.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gazpcyqmj.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gyadtdmpc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gzzitvzvn.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gpazxvygm.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gduvckeem.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gqecspsxs.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/ghstukffo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gsgnmvxqy.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gigwxunyf.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gpsayamfl.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gsiujwicq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gtjvfpmcv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gldmyoubi.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gesiwozvi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gjshlolpm.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gdbnteiny.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gvybnlswn.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gbbvzvyec.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gioqjnjpr.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvvchtglh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/ghpwwlfno.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gwoppgrtq.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gxyzcajgh.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gojjjmrpz.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gnkjltinf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gubhspwfh.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/guhtjxdai.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gtgscyiiy.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/glsqtwwyr.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gpdqzofyx.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gbfkyqkbb.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gqbyutqfh.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gnxixdsgj.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gukapvudl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gtbycqerv.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gnwtqmpie.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gztcgsdvr.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gizymnmzj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/ghkgunqbf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gtibvbwhv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gpeolapvb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/giygsomox.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/glmyheoxn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gwgsitrxh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gduaxufwz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gqspxpixq.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gnuchifku.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gctwyjwqe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gltjyjuye.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gtzbcdlsu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjixbaqs.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gxivzopia.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gbvvwsfqh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gsqnquccl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gewycxtso.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gozcmbspg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/grxhykuqy.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/ghcypqloo.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gxfhqiyyv.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ghgvycmro.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/grnrqayeu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/giuhzhzns.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gultacyrw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/ghelpnqnr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gufpbosyj.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gqesrjkcd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gixhlutkh.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gpefailir.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gwlxxiueq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gtfktbqrg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gahtaauqc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gscozumwy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gqhmkctkq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gyhvmpqip.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gxtrhhpso.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gjjbphxjk.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/grfmifrlg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gcqkjqjxx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxbbtwiht.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gihdtgtvq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/govbmjzvw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqegdjwfv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/ghjouogfm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gxrzrdagl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gourwynws.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/ghyuuuqrn.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/giuhbzdxv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnhjznzad.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ggnzqtfcj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gefqklzmv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gyefejabx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gidmvfhrc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/grucwsqib.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gddoxfmcm.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/ghvphstuh.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/goeqdyhgy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/godzlofxh.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gfcjyrslz.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gbrnucnjf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gaaqqpprd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gcsusaowk.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gtcbmtdex.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/guvtydzug.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/ghtyunljm.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gguivmulx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gpqwkrxvv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gzvlwumrl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gridskcww.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gidggymgr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gwieospcq.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gotwdyxbb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/goryysoje.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gzctdsqsf.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gneiixbzo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/ggjofgvul.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gffssxykw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gfbgcybme.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gjdfcaysq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gscznzqlr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/glbqwacuv.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gnvhvzgqb.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gdcdupdit.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gusiyppqt.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/ggsvoqmtv.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/guevgvcgo.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gtodllnok.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gospxspen.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gbwusasqk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gvxodwzow.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gorwgidxe.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/ggewgznsa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gkoqgqggy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gcdcdirjs.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gmimmxioz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gxblvirii.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gwgxzksqm.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/ggaezeibh.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gitdnmesu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/glomjexhj.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/galrjcuim.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gdxpnixqu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gxwtydrgt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gdppijlmr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gdvdhsgsd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gibccjsxr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gyxxiqlwy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gwedmqxim.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gpyygxtta.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gzlmtvnxx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/goxgbadeh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gdrtohmaz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gxdyjqnpr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gbmxfqrdh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/geojvmgsa.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gisqlssvb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gsbyunmwg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gemhsvqcx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxnsewpji.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/glwczoaos.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gycbjroua.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/geypesqqx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gfqhedlos.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gvyxugvdx.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/ghnyljdnr.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gipbfwixk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gvblvgkfj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gwyxlzabe.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gadtjzoks.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gcraduvtz.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gtsgtwxsr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/guxviyzem.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gcuilmhfi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gfsuzxpzj.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/ggtgeltak.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gqumtujsb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gdpmxgzjw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gbdlsqegn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gwwewwchj.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gyufobwvm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gtthmcbic.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gqjeagvlb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gfqzpifcj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/giioioris.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gcpnwgqxr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gphxpljvo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/ghkcxcdxy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/goyofatvu.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gqhdjfyqa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gcwfxwdwd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gbpvhxteg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gimsyevbz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gamkprvop.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gixycwhpc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gkviayeph.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gtdzzmmeq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gjqwgijfd.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gjalblopb.sHtML


<!-- 参考信息 -->