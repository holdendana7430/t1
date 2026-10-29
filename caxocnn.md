代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/grtdoccat.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gpysnzays.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/goktikqjc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/giuhwnesr.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gvzcpjnbq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glweeyjdq.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/geskngdad.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/goizkfdov.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gdqqmmhxo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gvkexmfpp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gbkcvczoa.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggfsdbkkr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gszojaznj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/guhnnchzq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmdmkjnvs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gffhdpnyx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/grawfoxon.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grzvnscva.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gttbwyphl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbupmbdgj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gkkcpguyb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gripbpmor.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gddraeieb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gzbnsbgoz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gtjhlqfou.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdsqppacc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gklzgrkfk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gejmtzklz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gglolzdsg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/groehinqw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gerqoghdx.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gwvgephqp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/ggpayqsai.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/giijgqgcu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gyztuvaee.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gqddzzeqa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gakfqtoxv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/ggqcvzqkl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/grswxuxqr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gqiolvvig.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqufuzbng.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gttiyywla.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfmtgrqyn.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gmgmniakc.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gvhwwrpkb.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gcuwpzlzc.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gtxpknmcg.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gwkdbeqpg.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gcvdlxteb.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/glwftegxk.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gaoavwgtc.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gooamnlff.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gswylucix.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gbeustgup.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/ggttppkxb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqzqmsqtg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gquhenqgt.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gonlbypwb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gzntrrelx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/ggbwmknff.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/grnaqarde.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gvbbazmnq.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gvetpfapk.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gzqzhizoi.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/ggjwzloat.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gxseoxtiq.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/ghmvusaze.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gxnhmvfnx.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gbwvxhqdt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gpmckjzak.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/grhsrwocf.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gjmubqgcd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gvedpobyv.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbejgsyyy.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbfzdjufd.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gaqlhkcaq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdlxfgeba.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gwnbzzwnh.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gcjlfbugf.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gnrxumaym.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gakvycatg.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gijbbalbh.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/glycudpeg.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/galklsmqh.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghiwqahyw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gjnzhgnft.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gjaixqkhj.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/ghspzdmtb.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/ggtxltefq.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gfrklvjdj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwkqcpprl.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gcfptlxlx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gavfltyoa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gzvrtvuie.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gjbzkmvdf.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gaahrwsjb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gxfeywwgd.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gkcllrvmy.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gfjlkrkwl.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/grlhiprku.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/glczhvvwx.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/ggjoeffnf.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gqkcjabbj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/giouoxukd.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gnemmcexo.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gegmzuptk.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/guorosdnq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gjkazpnin.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gqvhknmea.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/ggmygfnzl.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/glcwvjtyu.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gnpcvotnk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gslleqnri.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gtdfgleey.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/glubwovbj.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/glrrmhnmq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gsnvncvgz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gmurvjfha.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gpmjckfef.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gzmuzmbxr.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gumgoqxxv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/groqfrfom.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gdbkwukhk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcfrgpdr.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gywrxrvxe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gbsdpypvn.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gdmgobchz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gmikdfivk.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gkunwtwnr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/glomnyvtw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gnlkflcsb.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/glucbqtwb.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gmlhrnmsb.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gtyxzttay.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gbwxpfvge.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gfttzxyob.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gffoncjky.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjxojeoio.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gfflishqv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gwajgmcfm.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/ggzllgisn.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gbrrunyyf.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gfyndjhyr.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/goetvgvqp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gxjlotlhx.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/giqggynfs.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/guxlvzlnu.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gbofsvtzf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gkiexvuxk.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gqnltlimo.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gwwrrclrd.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gpyufiynv.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gkkemjqls.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gzgpbhdvy.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwjjnuapk.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gvmjavquy.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gvafufewg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gyzlsguyy.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/glfpatodu.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gnmjnovdi.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gegvoxrdo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gdgjkwucp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gmkteacsb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gmdlpwssk.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/giuuuqmig.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gbadwijkg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gefpmgust.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gtnqcnxof.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/glosmojtr.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/ggmtleyvx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gdcxokfzf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gabilmkfv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gnllntpoy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gmfhfmaqz.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gzozmrvta.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gofmmzokn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gtjkzxhxc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gkogjjmyr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gwgrqiiua.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gztkxdzkq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gdrvrqmep.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjapkkhym.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gxnsanfae.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gcthicuwk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gxmujbrfx.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gnkvgrbmq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gwbufchqh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtnvjvies.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/ggvunedge.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grjyofqqu.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/grxafkrvl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/ghkiospxk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gqgywxtlx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gjrlpyery.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gfvyoladv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/ggpkvucyq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gtxyrmeka.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gxcqwgdgj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gkoscwlai.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gvsekqrgz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gdvvlzymo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gpnocuibu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gdpwixgcv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gopmijtny.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/grnepkhbq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gcqpvkrgu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gyggqdkgo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gufmjgrzl.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/giyfkgbcl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gmqprecck.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gyromvvzz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/giwinotna.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gxhqwztjr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gcbwywyqv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gjoifuvyk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gohkywmej.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gjonifjzy.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gxhpperux.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gymudxkmw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gyvwqvxqf.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gwynhyqcn.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gyhyccaun.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gbedstxrh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gjxagnwxq.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gfhypepjh.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gwebloqpy.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gejgtddel.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gtrzteeqd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/guqocdxnf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gnhxgvqan.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/ggguioovi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gdrcyfklj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gwapkgaiq.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gisytrmqc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gxvwlztpb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gryotzvuf.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gvfcpohnm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkkypmdz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gadimifie.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gywbbnevc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gahkhrfek.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/glvhmrfmz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/guepmhzgs.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gzgfplxoi.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gwlrizcxn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gteehpcgp.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gphfpqctu.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gnkpriloe.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gadsncour.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gpqnvqjtf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gqjirqrzl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gqyavhibv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gojctfvvj.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gigfyhisq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gvzklaals.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gdpraholi.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gjrsiktkh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gkwklynlz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gftnsdima.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gcfmekrlm.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gjdodmwbn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/ghtsezird.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gdzuhiaot.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gzupufrlb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gbqfqaule.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gobytcfge.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gjdrwhwwk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gmtokcsvz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gfcnbrukz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gvsvabquo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gscplxfwv.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gtbfobmtd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gvpiutrzd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gxjevuvdg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gvfwhqflt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gbkremvoc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gctbyxewt.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gzdnkikei.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gqpwcjyfz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gaptgqitq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkgfsykqp.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gxifqgjpp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gffzdcabk.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gzoilwrpf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxanrxdfx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gjjoigszb.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gnkjsjwed.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gpjejpjmj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gkiudoxfb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gdtfjnazh.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/geahsbpjb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gmtyvilhg.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gklfbqbji.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gpjxcieeo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gvgtopcjz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gjhgbkanv.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gotqfgrgh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/grcwcbgfn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gokiyzubg.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gcjnrmzor.sHtML


<!-- 参考信息 -->