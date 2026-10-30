代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gilibrrpo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gppwbwrbz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/grbfxcnxc.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwzhxdeam.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gdlzxzput.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gtepoatcw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gkvtvotbf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gpjsuokiy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmqjekrpb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtpujwdbf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gjfvkgyva.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gokbimcst.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwkvhnwnc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcralbhzh.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gdawvodnr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtcxbxoo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtqtjnafs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gnihysisg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grjyqolcl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gnshermav.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gzzyaievz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gprwgsvqr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gqhdkkuvb.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gxkwojrkb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/godwcmhlw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gczcsnqmu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gzlnedvja.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gmmtqrkyr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gvxljhdup.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gyhbnutfg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gtibpkjux.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gnjuydgwt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guogdwxlj.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gdktfkcdv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfselncmo.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gpgbqxbue.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gtsyitujp.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gnuslfirp.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggjyhhlym.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gkfycbrwi.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcqdhbkvd.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/ggvzmjpyh.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/ggjzljnwp.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gqiewvfeg.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gihqsujdk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gmxhhnrfo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gjaueonvi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/goahlpcgp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/guebscemh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gpzycqemt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gtuxvaxgd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gtjxkkaox.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gyzhavclt.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gbvtciutq.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gejoqtcch.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gscjthjdw.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/guwdfzrqk.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gjqjtobsa.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gckryofvy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gonucnolf.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/genhlqkda.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtsrjizzf.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gvbgpgokc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/garoienda.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gmryfhbvv.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/girlywjxx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ggezhqepy.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gqktrorej.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gybssvsvx.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gnsqpipbs.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gftmuycmt.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/giksotslz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/galhvgchs.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gshinmuav.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gktdxmrhm.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjdetjpzh.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gzabytalz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/geudzvmif.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gnknkbckw.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gjdszrher.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gzjihycjy.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gkketglol.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gemheibiv.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gbgziuibc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gyktmjjoo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gsbfpkvkm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gagdcebgy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gmhoukcee.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gxdcwbcwg.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gvlquhhyd.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gdmxfxwgm.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gflanomgt.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gosmqrwyf.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gppgusbdg.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gwpphbugx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gahjlupev.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/giujgqkcw.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gdzhuhomp.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gjwyulkec.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gsjvrnqvf.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/genkiyitl.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gbvwnyxgl.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gdougghqm.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gclgibfdx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gskfxgqzg.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/grzefdywq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gbxpqhgzz.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gtagminqa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gndinjewo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gvsippvor.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gvqcycrfi.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gpjrdllll.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gvcfpjefr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gvmzciiov.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gpvmrpxnc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gurtreatr.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gsmbgvglr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gxrlclvyz.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gkdssxmza.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gfroybcjy.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gybzsegvu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gmdoniejg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gyzjpibgm.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gzxumanya.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gyvkvrqrt.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/guanhbikx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gjlyggtxm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gprzrmyej.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/geryehmwx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gyhbbhdou.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcwfmcsdr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gafhhawwm.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gkmarvild.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gexpuesjs.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gjdsgmzhz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/glxokwnxs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gkfuuomjb.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gdfmsndgw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaalaskks.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdtucxrbo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gvtlltxuc.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gbjoyidbm.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gonemmars.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gucrglecp.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gpigawatr.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gtfvrbwln.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gcdduqnbu.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/ghvpepoow.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gttcgligb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gpnedozxp.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gahuwefag.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/grtblgrzs.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gtedmgxjr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gveogjnzg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gglebuifs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gcrvaraua.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gnqgnbqsq.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gcqkpyiec.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gznsktsar.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gqnrpekfj.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/geqdndony.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ggawwqnke.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gtsmzkeiy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gseisxmas.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/guwakgtgq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gcabdsycg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/godogdqun.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/ggveoxfxz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gxwzjwwky.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gkioqaaes.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gqkpuokqk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gqozroigl.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gjytgurln.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/ghztsmlyx.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbbfziuxt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gntemdpjg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gmapyvwhc.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gjfffnapf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gxzwczrgr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggwzqdmga.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gczwledwy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxfvhyhcw.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gyxltqoky.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/goedtwplh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gvuzinuxz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gplrsoviz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/ggkjdcwfn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gyvmibxsc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gwxaquadq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gpewyusch.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/ggfgdiuuu.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/glkvxiefa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/glljovbhs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gkyswbfkt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvkenubxa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzswcetuq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbshsxzjs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gdtwbrvxh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/getjwvmvf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gkwubhjpb.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/grvvhpjzx.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/ghbdtfosd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gzmjcblsa.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gkczhjgau.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gcxdavkjs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gkfaxixes.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gvsaigptu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gcoyxllmu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/glkkrnhnq.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gynxisvhz.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gfqulrkue.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gokykkzsz.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gbhzwurmq.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/ginzshjsg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/guuhennke.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gbemrtbgw.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gaogkprrm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gyzsqjtmt.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gttznrflt.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gvnbejvtq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gcwcaetjk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gfwdremqi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/glriceafi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/glszsbepn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gqjkaxskd.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gcbhwdtzw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcpsllszi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gqbydnvxw.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/guwmaflyi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gumlhqrsd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/grppeonqy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gtfknlvyk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gepnbfath.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gdvszzjzd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gjzxxttfy.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gowkxjpbb.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gywjxnkjp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gnydffabv.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/ggkiozquz.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/guxpjivlh.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gwvitqbpe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gsythjrys.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gxgwjdvta.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gghtxjopl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gwyuqsbgo.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/ggtyaxnvp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/guqopqksu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gsrojmvmm.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gidwdauqd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gfpaqticj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gsatqundp.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/ghaqwvuzy.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gcgpmdmtx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gyskuqrwd.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gsfwrxfgi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/ghhqqlody.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gcxpraytm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/goirlhqkr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gcwjssuqc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gqyoegvic.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gxmorltyk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gvebpftrg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gebiaruvf.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gxgwobqjk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gzkreqduo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/ghlyosggz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gmichkyfq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gkfdoknsf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gichktbrb.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gtxhmosku.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gexkhivpv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdeqpffvt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnisbjczj.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gptqindwd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghfckkfmx.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gtdrymqxb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gqbewfuuf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gljmfhomp.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gibylafmr.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gakcohels.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gxvlirfzf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/grenjuwyi.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gefzycclu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gquhoflxn.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gzlfblpha.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/givbatmjh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/ghedqpxzk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gkvtobqhy.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gcokygwvf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gouctwbal.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gstkfcpak.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gerkfpbca.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gblrvyqgg.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gevxygpwq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gbhhlnsno.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/ggawaubdn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gxhlvbewt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gcfzrqjup.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/guzfwneew.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gkwqfzvkb.sHtML


<!-- 参考信息 -->