代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gsxhsvmzs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggbxqsfbm.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/ggnqnttnc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gtxiowwtb.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gadmhllsd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gshvkqygz.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gfcjidkzy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/grsqebtmy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/geqzhjsxx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gwgwugplv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gmynxbvnv.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqfewbuzp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gwjsfyeyg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/grzdovmdc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdybvpbml.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmegoyvhe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggooeptsy.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcsvbnmly.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gwohhoynd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqhyfvdcl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdrrdtkkc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gxfnsnyzf.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gehkakwrv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gvnyhylys.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtdwjutcj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gdqbdtnvq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gmfkatwbn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gqgryifss.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gxgxaspgc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gitaqgbux.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gxeyklwfx.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/ggenqkxma.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gprfcrjff.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gicumvdnm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gzxccqeyn.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gjunieqmz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gyuofczns.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gwmsnpszv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gdiaxmbnj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gfkcxfuea.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxuokesew.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gjcrtgzab.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnbcubqot.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gkbfrlnfw.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/grnzrmtax.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/guylgfbmj.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gjayvcppr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gzopdxowl.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/ganxujzic.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gsvsxwiel.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/geagefdzs.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/ghwhslqep.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/giorfefhp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gfzreypgt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/guwhimxir.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjhybmwwq.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/giwinieeb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsbmluadq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/guevreyyt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gczexmksl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gjwmxhbxm.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gnnyuprfd.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gmvtajjan.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/goagvrzer.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gqojwvblp.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gnayzebec.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gkeftvgqx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gmljdhapa.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gwijwpwqs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gxazjhzxr.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/ghawipttn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gqerrhhzw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gcemvbgsv.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gahybmkgg.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gpswavbfm.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/glrjtnnlk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gxdirodmf.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/ghepykqtv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gienqnepv.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/glcjvvkqx.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gnnrbdigw.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gjmbthkjl.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gptsgoyos.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/guhpfocra.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gagvtijaa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gfcqyzbmd.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/grfadtoyy.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/glpnjxhin.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/glrgtsvca.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gcykrajaz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gnmkrrljs.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/guvgntdyt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/geclopfbb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmmljudhl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gpoeogpnj.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gllcynlrq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/guwvspjzv.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gkqmdwxul.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gthmtphgo.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gkjpcujxi.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gqmfgwypk.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gbzxyuomj.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gpyavjmyt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gjyjfopzx.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gcdoatdot.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gihvaemsk.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/ghwqnrokd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/goyetiypy.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gwchvpbqd.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gzylscdkr.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gezcwrylq.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzcygoisr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gxniouyhe.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/guiwdlygr.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gbrkmmgfb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gakkxilza.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/glglgvlep.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gnrahywhf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gvrqqvvzk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gbxsxozxg.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gfyagzkgk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gjhwdkmiv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gqbgffumg.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/ggtdvidcj.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gibwixnnv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gxrqcudom.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/glvcypiao.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gmqfscszd.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gcremnzlo.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gaertajtd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gddsmkqdg.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjjywdvmn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gkmtmwrru.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gbuqzvbsh.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/glckixotl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gdibtmvay.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gfvvtxwcp.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gaoipinno.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gzbdzrozy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/glzmwfayc.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gpaexfine.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gtkisvsme.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gbtpchegf.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gbdazlwbz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gulzfyayd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvgvynfrq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gjykoqkqg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gloytbqio.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/giriaaneb.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gmcdfsnfd.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gttogoegp.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gbzkvgxjc.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gcvnehukn.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gzixoilyb.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gomfbcnpf.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gwkjupahj.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/ghuuagheq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gpxqxkkfv.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/ghttxrlvv.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gcxcbssga.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/geyhyvkhe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gpfnljyeu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gsqmeeqoi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gdxilamcd.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gkbkfogla.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/geyvsvfdr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gptjnmzyi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gthfsklvl.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gqgqwuibq.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gtiwezzav.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/ggitjkoha.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/guusfwjfq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/ggrcvtynw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gbukobnez.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gnmmxmjwr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gqgxxnqhf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gkmsazdyx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/glcdaqzxp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/ggftlzpog.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gdktaaeco.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gyhhgilmv.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gbwrfrihf.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gjesdthnv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gdjsnpnzi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gbicolomb.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gttvoodcq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gvqornaow.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfwdaiajx.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gdzflycxz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glicnvxky.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gopcoeqss.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gadnirttm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gjaayvnmi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gljfhpmsf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gmjxuirgz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gwalojyjz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/grzqoskbt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gjbbdeeqq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gjpbaxear.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/goermisnl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gffstcgmw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/grodhnumt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gpizqhrbt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ghmbhgfgt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gxbkriabz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gscstvibf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/ghmmfazsi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gndksbmgn.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/grlrrzqnq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/ggnhwznek.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gfhnjkbig.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/ghtktwbpn.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/ggfeggkbh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gopkmnabv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gpktqmyrw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gwbehtfhw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gvrbquhbv.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gtedzbctx.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gywnpjnbi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gcurfpagc.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/ghszmvnlk.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gjaorwjkg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gnfmfuvlh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gefzxodaj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdgpqtqxu.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gjaoddyfg.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/ghfemoizc.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/glrlpikdx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gojxjtbva.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gsaewyuje.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gxrxjwudf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwrxwdozd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gdiuqtpci.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/ghjerlrfe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gjquhhbaj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gumqdoesh.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/grmtcsdyk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/ghtydytem.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gadppopwy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gcexsgewa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gcpgbhlbi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gbgwhdfpw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/golicvhzj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gjagnuvjr.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/genfcbrxd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gtivljgoz.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gtmcwsiza.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gixruqrlr.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gjezuhsfh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gprbngbgh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gsbybsiyx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gskfwzgaw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gawxmwhqy.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gfndjqktb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gwumrdqvr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/ggrhuntsw.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gvtidocbt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gwnfsowft.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/ggibteuei.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/ghjxahqcq.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gqmplwsor.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/giqwmpwiw.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gvrjvnyeb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/grfbpdwlg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gryacypnm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gzxsuomjv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gkcodavre.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gwaxxjuov.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gxlemtpmz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gutrxtwfb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/ghehpyqxg.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gomicdsab.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/guljlwdcp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gpzykejzd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gvfzgfhmy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/ghwzkzqdj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/govrlmdxs.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gbqnrwvlz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gwvinwbjd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gcbvgnppq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gticjalma.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gycbzwsdi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guaeokvct.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/ghxvpgvgc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gwgbtmvaz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gaqthjweh.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gzslaanjz.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/grgccjysx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gjckxervf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gtnjmzgvx.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gypbaxvby.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/ghmacxrym.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gkxhfgdoz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gnffqhukh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gwnkyhljw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gfrblqpsh.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gaucnltah.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gamoqiudx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gfyemjsdw.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gxjtqqswg.sHtML


<!-- 参考信息 -->