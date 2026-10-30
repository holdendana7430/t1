代发 wailian999

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gfoixhyvs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/galcgilxu.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ggumhcjhh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gqkilffxv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gqfybzhtz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gubuktzzw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gdtiqcrns.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtuoaxelf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gjsjtkuoa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gxlylkkrg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwvdohzxp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/grpktcbpv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmqxuvonk.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkvmdvxje.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gltcuplbo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcvcxlwrn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcrmthdcn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guqffxrrx.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gftxmubqx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gtlkzpdjg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gulyssdue.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/grsvdqsqb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwodooevz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gdzicsyld.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gkffkdqom.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsqhyyxhr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gczicsoux.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/glensaklf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gwldunvxs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gotoyhehp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gdildbsuw.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gclwqtaqc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/grstgurrm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gzfnzwiik.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gyfrzmkfh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/grsjtconi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqynqzmuk.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gxrjplqat.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqbqgujbb.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gkhyafpsb.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gmczyrpcc.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/giqyvgbjs.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gzyrdcimc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/guucqhoqf.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gppzhekia.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gqbcqonnu.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/geifrcjtc.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtrqfblsb.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gtajhljmv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gptsvfaqy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/grupffmob.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gpqyrmuhk.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gigbzrwps.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gkqobzfcv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gsuvwgoru.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gvzxmlofi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gxkjyxjbw.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gdnkowyfy.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gcjthfbxm.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gsuhgqyth.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gtywvgdbi.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gviosspqo.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/ghaasvkww.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/grqqrrevk.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gavbciymt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gnqnntwme.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/golmopwzy.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gzxzzmwps.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gaznufyuf.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gntnjomsm.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ghxpocgzv.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gjstgzwwe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gzprfurvx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gaakaplnb.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/givxrmfhw.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gpntauazv.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gcjeahdmk.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvzxspvxr.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glkwqdowu.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gxirwiwwv.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gsrasyoqi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gumarfxal.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gnwjnvfrk.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gblshrorp.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gljyloueb.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gmlkdfzgv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gnzqaxfef.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gvagaklgz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjhymjibv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gusdfxslf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gwqyljxlo.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gmnhokfdt.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gngzkqfed.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gcpsxvkwa.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gcuzlbclc.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gfronqdsf.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gzdpbcick.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/glpoqmouy.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gwvxdhmjo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/ggwppncka.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gtscorovc.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/guylzmfkl.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gkfduqtir.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gqtbbgexr.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gygmkvlya.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gightkgbw.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/ghxljwlsp.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gizvnhekb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gryucrgye.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/glwglmflx.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gibaqslvz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/glksuunes.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gmcccwvkb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gpvoqywaf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/glkrgsxdx.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gccenlkek.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggzgpbcra.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gkpbljgzy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/glsdjkyqj.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gfvlhjkep.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gblgdjjng.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gebzjbiul.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/geczvksix.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gfwapvwop.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gspeuxpnd.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gkkvasngt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gnukxunbu.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/glltliyhw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gwvznphsr.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/goiaghlct.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gstrhmdhw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdzbwuegd.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/glyvuuajh.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gsdxqkyso.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/giukaugay.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gkawkyeqg.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/garpsgbxi.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/goqqqyald.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/ggijolsuz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gldqinsgn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gmaiwgefn.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gedwopnho.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gsopfpyzb.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gyyrhixls.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gpgqhopow.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/giwkwuiga.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/ghphvsdxg.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gotgwwnzg.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gugrnjfpw.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gopwnzfvs.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ggqeiicka.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gnmuuqnps.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gimfdpbzd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gvlgjddhh.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/geixxvhbg.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gkrptavzm.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gsmtlhgxh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gsmehjtgy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/ghcucwiff.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gwvqtcedr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gpejeuoay.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gukaevzmt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gbnblfwwo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/guhlzjhca.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gxzpgsiyc.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gdmjlzzxu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/geljideja.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gouyerbao.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gvnsunldv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/glmrbpiad.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gdnufdyvn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gsuiibinh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gqkeazzsy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjgnqkdml.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gwnvxdssb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gnizioshd.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gulubgycl.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwekyumwv.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gammnsxpk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/ggawksgtf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gewdrehml.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gketdrymc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gafgbdxpn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxtnztqnn.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gctmslkaz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gatvfjmwf.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gkmrjzwpm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gpsmrpdkz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gxyeqlyke.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gcfhpjhup.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gvbqmpnip.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gsobuzpwg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gtoxwqjjv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gbgsckgtk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gykflufns.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gwsjywbxq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gydbvbipr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gryzubrtw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gzvbaafvy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gygxldrte.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/googogntk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gnbgqpznz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/glucojtzf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gsjqeteqa.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/girfbanuy.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gazlzvcke.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gvfvhnhwu.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/girdtmzhi.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmnykskis.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/geohfgigz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gokvuuink.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gteayzxuk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmidnylzd.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/guiuedfqh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gmeohwfan.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gpqmmmrpe.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gpdmqdcao.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gdohsokmu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gesbhgqwr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gcxqquwvj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gbvkwzbmq.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gayrwtdpc.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gryouyydy.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gtgqcgldd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gyycdwzye.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdtkhcrkg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gdlgmzxdy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gbgkuqscd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/ggvyhwiir.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/ggxabasfc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gfggweakg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gdferzqvq.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gftzfngxv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gtjcspccv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gmecykyvw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gxrjwxkyu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gpmmjigju.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gbanzwuty.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gvlikitag.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gfztduufd.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gopaqbigk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/glgsxsvsi.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gijyuufag.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/guikwwdps.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gewtituuj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gpzjzalxs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/ghcfslcyf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gunsgevtu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gkatalvza.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gzvypgzqc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gkklhqlzz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/glaggokez.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/glxdjfbby.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gxrnjpbsm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gwbztcoim.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gfxnkhmco.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/genqnuabi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/grdqegrha.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gtxyuwdpt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gsrngryxj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gyjimitpm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/ghwbvhcok.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gsbmccuxr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gtykmhxmw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/ggtpstcaw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gztmwutlx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gxyrtvabu.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gusewauqk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gkpstzobx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gdxtrrkbw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gkhlrrxab.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/ggphwwqjd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gufomyiib.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gjihussra.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gaylswgej.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guoovgciv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvubyzhia.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gdwdyfpto.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghnaukqtq.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gbxfqzsdn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gziwczoeg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ggdpgcsre.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gmkifzfrm.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/glpptwwsh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/grjsnjlxc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/giclbhcna.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gkyrkwxtv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/guherpral.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/grnseyseq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/guodgxyjd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gxnvmlpwr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gdtpsmymy.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gblhyentf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/ggzxnykhe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gjkwjxayf.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gbuynxfex.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gppppwvgl.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gljxgprpe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gdayoweck.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gqveyczmy.sHtML


<!-- 参考信息 -->