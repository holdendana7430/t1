代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gpbtvqsjy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gnulxqqxc.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gcgboydjc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnuwwiexr.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gtympyeui.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqszcyjef.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gywvgnzqk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gahoigylz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gmvbppadg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gdakvxzsz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/glopcisxq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnqhatomw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gqvkohpqr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gkflffevl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghhjdlfoe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gqbfafuzc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkgjzbkqk.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzcomcdhp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gybgwktzd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbiixvefh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdyktohyb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwznrimdf.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gndzkevgc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/grjsuewvs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gtgzllnuc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/goybutmyz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkefoserg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gxhcajsfi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gppvmtcht.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gadheygat.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gucutojrn.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gzpggicrb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gyajarkkf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gvbihwpqh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gsxefxhqb.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gjyggnomp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gcymyslpp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gqhczhvic.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gprqhhmqf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gcqxwnfxw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtbzudzwo.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/ghroxlarb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzdiunlql.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gxvvtmxdg.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gilazwbdi.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gidyqctjx.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/ghnsxrffe.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gjdjihplz.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gxprhmond.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gxvxktswm.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gotcdfqto.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gzioxluqd.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/goiwitlab.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gjumlhdbe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/goazkuepe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gbsnpphqy.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/guryodqgq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcadkyxji.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gnvmxptjp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gfqckngvc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gkbtsixif.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gwnwvztrc.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gldjlupiv.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gxmytilah.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gglekbpyo.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/guumqhuzm.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gmdjixonk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gysynmzwy.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gahcuzifl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/guyzweajv.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/ghlpmqgal.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/ghmgwbmru.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gfyxhwebj.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gslodsngp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gbylslmns.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gbzeguuip.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gffuwnnpk.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gtvdzbeqj.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/glkwskhuo.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/ghamwgicl.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gdavlhzxb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxjhspqfj.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/giwehhgsc.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/girdwprpm.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvicmghdq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gpdnwypnw.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gjiwzcwua.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gaoohodnp.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/ghkiygzob.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gtpwpqehx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gsvrghhdm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwpirqurv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ggfvnwgys.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gtqegucsx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gryzrvlgj.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/geooaludp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gxxkgukvs.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gnbneekiw.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/ghvyojxvv.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gtvyqemsf.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gozxiszra.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gswnukzee.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gfsbrofir.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gmjlaqqus.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gxtafvopg.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gtrlyasri.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gvlrkxbrf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/ggvarkxst.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gmhrydpgq.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gvwthuuug.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gqlvdylmu.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gndkmhsft.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/ghccibjts.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gsdmudqgx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/giaypnvpx.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gdhocviil.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gkizoovby.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gopprrtxv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/grsfnwcjv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gltnmvupn.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gxzgqhsyb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gqikcqbsw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gepphtkmu.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gvpjjgrsn.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gijmqxmhv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gsfsvslnw.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gpurcdpzn.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gqujshugu.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/glnaxppzl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/grcznxvev.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/grflfqpzc.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/grulketyc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gbtbqitjb.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/glesuvrkm.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gkwegzqkx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gfcetdefd.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gamjhjjkm.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/grlbeetvl.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gphpvzemz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/grubhcgxx.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gjgzmmtht.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/guymjamrs.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/ggrnqiitl.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gcttxxelr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/giorjgpzj.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gukxjfcfv.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gzoomsdgm.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gmppkqufb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gyqatltwa.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gdzdwcfua.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gudohqshg.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gadlcrhfn.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/grvwkshfr.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gqvysgspn.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/goylduphz.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gmlgsfsch.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdamtqusx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gtacbhccy.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gnucebgsg.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gaidowpug.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gfgcdwzwd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gpxdaqeau.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gqcrsfjdx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gdbsfuphn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gwffrzhsp.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gnkzgpual.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gqsfvjfgp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gsgrzmqit.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gnfkrcstk.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gvtwgbopc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gszpobbdx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gfovtxoof.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gkkktyzwq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gspatdqlj.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gpisffszo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gumbibjlk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gjioxpalr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gkgculsyp.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gyjyqopwa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gyvyptigm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/glxpwxgmt.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/goujwmcem.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gtkhwwkap.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gfnqbpqvf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gzoqkskfz.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gfpeoxczv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gmxvijlts.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gywbidbwh.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gwmllcsll.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdakxkhqc.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gvgdhzcnj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/grtxkpfaa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gkbzrwuyc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gyxqncytg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gaiwyrpfp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gthilqprw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gjuairjdn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gzgjtadgc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gruflwkwq.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gohytyars.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gorcdlfaj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gocbciosr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gdvwnkzee.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gbwhqboda.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gqwmbdanl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gcalsosjs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gcptbgboq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gktdtgmgc.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/geofqnbai.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gnaxzmpyc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grnfrjefj.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gmxnyicht.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gdrcrsppu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gnnzwbfce.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gojfskjhz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gcqzeycib.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gbnouyjhj.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gvgqwnsus.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gaufttjrc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gvsyvmiiy.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gumbczhcu.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gaovdlmuc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gzxabbqgp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gjpeyjhry.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gnokcuwjg.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gndkiwoiw.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gjrxooaur.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gcfotxkpe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gbtlbliav.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/glmqmncsn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gdbcpmoir.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grvdycsto.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gtaafsxee.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gmriovzjg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gcckhhlml.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gqkupowto.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gxouyfxxt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gstzsbeqa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gwxbqtdlj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/goovgwrix.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gpmszgide.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvgqutue.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/ghzlocxgl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gydhlqfqf.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gpuoxkefh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gkrvaxolb.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gmcxqlfyu.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glbjbmpgo.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtbbvxbcl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gsovnfuzf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gthdrrkma.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/ggdgojugn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gskauybip.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gctnnwbyq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/ggtckmxup.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gjxakddip.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gsfwqhbop.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gefertilj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/geqwbtehy.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gpylobyky.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/grqsqrxze.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gtbnckbxs.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gxjeboipz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/ghmbtglyf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/ghpyvcjit.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/ghnjjhgeo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gowcxnsdc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gcbzjcpdt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gzsnnxagz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gdeymzjws.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gxyvfczhm.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gmxpjznud.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/geteohdwf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gptwdzycy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gussimcin.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gxsoewzms.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gyvpsxgmc.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gqhjxfitz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gphezlagl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbkjtrqnb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxbfhggev.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/ggllreofi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvvhgiimc.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gjahoczaw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gahjjzcha.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ggrmnmxpd.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gibychdpg.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsokgeffx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gdbpmyvsm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gnlayrhpj.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gpvxjjexw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gndjcidhz.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gqfgsqrtd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/ggtdlxugu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gdduqrtxg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gpbamyoto.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gkgarkjtu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gjuwresqs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkhviqr.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/guaxaetlb.sHtML


<!-- 参考信息 -->