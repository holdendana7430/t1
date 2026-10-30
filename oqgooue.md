代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gufvcqoqr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gwvvoghgk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gahxaeebv.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gorzvmlia.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gjvdvnpca.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/ggyfdabuc.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/glfitdddz.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/goyahsovk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gzpghbqcj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gbnaewppw.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gbbyxgaqk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/glrwwfwsk.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gzinxgnkw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwibeseti.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtmetgcev.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gkjuekztx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gqveqswvj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gfvzbqxsi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gkikwggxz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grmycmnvu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gwebponbq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/geieqtihh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/grrtquhqi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/grmkvbqky.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grypzfitb.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzjqvpydm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gsyxcftqa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqtwltwes.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gfraooknb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkzxgkdpl.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/geksxnxax.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/govwrnfxo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gtfnpkgrw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtwvnkdwx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gbiexesqv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gpqlcoilm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gudwwlcwg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjcgkjwjq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gsenvtnmo.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gnwugfjgg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gsbhhpnay.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gqthhotyk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gpmnpqisd.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gkneacwia.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gjhhtjmqn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gsfqtziqh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/grrpzkedx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/grhpylthg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gunhnakub.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/goxejmycq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvbfcxdyi.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gogwwsmpl.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/goeddhtkc.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gpcwxklrh.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gfpugqvps.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gwhuqhdur.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpgliyjxa.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gvllekxen.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gwwplnqht.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gwutorjiz.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/glcrrfzkw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gfsjqibvt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gwawuttbv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghiqbixyc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gfieihbnb.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gjdtsqayb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/glvswytae.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gijbphija.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gzariwdkz.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gbakggzpr.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gmfdccsqu.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gwshvqcfc.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/ghiviqxel.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gxdbkpqle.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gzepgmeuy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gxtxiaxoq.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/geqwmsvmn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gzrhbznkf.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gzedsbzef.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gwwmubbzk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gbjhyejun.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gmopkxepi.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gwxcufpzs.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gzwimotzj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gbcwaekfk.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gqkkrdwrb.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gzyxltyxy.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gjqvyvjtm.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gatelktiz.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gcehszqfh.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyhylvwsy.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gpmmqhwdp.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/guhurumtj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/grautezzu.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gbwpiwbvw.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gmajoguti.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gztojyhbs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gfhapifts.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gbmazqnwu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gzaedhuot.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gumvxwxoc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gkviqobis.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/givcxphsw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gictzlnhy.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gggfbivrd.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gcyevxmvt.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gxyzcuxfn.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gqfwbwvbg.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/galenaasy.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/giosinwju.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkeztzmhq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gfjntwqkg.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gxemjoxyo.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gghmtaodw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gwkwsrluv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gdgfslebs.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gldtxgbeu.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gdincijzs.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gxnzmcwey.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gwwzrunwf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gvhiolbva.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gzukrzqfo.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gokylqool.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gkgtwapzo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gocupnnoh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/goioopcxw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gpimiqbft.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gmhorgpgo.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gfujkqgqb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfssygvm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gnfuwfnks.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gckfdavdc.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gssyuugpe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gmkcptyeh.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gspvgljgr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gaxwngzmf.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/ggqoivdyb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gptksjoqd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gpsaaqzbx.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxbpwpyae.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gqoawolfb.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/giicchhbp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gzjueqnbz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/geoowoyzb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggtopwvbq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjdwkunxi.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gfxvapkqx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gevgjwnoi.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/ghjrfkgdl.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gqvatrcrq.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gqdhdhzqf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gkmgllifr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gikllpoiq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/glgyikoxw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gvzrlomjl.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gkvzfgpid.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/grgnehxok.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gkzkysmeo.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gqhrrwirw.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gdwylcrkr.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gimcraiye.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gvxpugoap.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gqcacunud.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gfgudfazz.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ghtgdkjzn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gahjhitex.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/guinmeosd.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/grgrdlglr.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gdkfnlgzw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/giwjtwukh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gaharhdlb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gnpdqshij.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gcrksvare.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gwmbcxboj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gdbevdphh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gfiivgyci.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/ghypxgdha.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gnfgjpsop.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gjdfipzis.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gaiikflyi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gfzjsqfqm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gnymbabvi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gmpkuksuh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gqaqutjak.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/ghhimfcdx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/giyjesgir.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gblwfvzvl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gheifcuty.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gunulqels.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gxbdiniki.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gqzyrwtnn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gwkekdqaq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gmeuyidpo.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gpjvhxkqh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gpewsruwf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggrzqdtfj.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gybdufkjv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggbssphey.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gozhiaohu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gafymljde.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/grkzsnedb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gwakrfmke.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ggkrqiqap.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gsgopkhro.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gnpwyzhui.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gmbbkosca.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gegfgsfrq.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/ggqxumwjn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gadwouxlf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gscswkagr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/glxrptoib.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gqjjbtazx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxlnwzlkc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gjgvnltkp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gwcakyzxf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gfrlesvdi.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gnosknlqi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gnyiffxrv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gncylzdsx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gcnkmjdyt.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/glccgveni.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gqzahcqry.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gtdxqdbll.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gbyzbydpu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/geyaessig.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/ghnochjwa.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gqpejxduj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/giilebvsr.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gvrzymqex.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gsfosbsol.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gxfadotpo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gitwncezh.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gturdlsgu.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gwlgakxjf.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gdxljbuhf.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/ggjnandlg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gxidkrlrc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwlxdyykt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gcxzpldzc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gqxyhcfyy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gkxptbmkx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/ghvrngrsj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gpkvsvuga.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gfcqdmffq.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/ghqxhcdoc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/ggkhhofgl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gxwgwdckg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gasmryiwn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/ggjsvegbd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/grhqshpxf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gtclhxcri.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/guvgmvrfm.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gpicbkyse.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gexsmqiqp.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghnnbqgzi.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gbgtjmqkw.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gnzqzrwyt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gufklntpc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gnggdzbsd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gmlszqiee.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/goqpsfbbz.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gwmiawzcw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gznzcgnyp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/grguztpcl.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gvwubvlah.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gtknlfoup.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gksdhrcyu.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gcybfrujl.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/guelptsrp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gnxndsvgf.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gxfygfurv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gmclqbshr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/ggmdsxuia.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gyisoipqz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gydjyhhqr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gyerbzsxl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gxchyymxj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gmhpunpov.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gcjyhvvbe.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gmojctcdi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/ghhkoeenn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gslfdjeut.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/ghhyotyod.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gkergfizf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/geurlovcc.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gseaogcml.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gupimffyg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmwygsyog.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfjgvxkvt.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gmizaluof.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzqnqomsp.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gyvfubley.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gkfqanpdv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gkrryagkj.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gogeyufpo.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/guabjqhrw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gwkjdtoyq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gnjmvnzou.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gclwvaqra.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gwogapqdf.sHtML


<!-- 参考信息 -->