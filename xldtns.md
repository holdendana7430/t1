代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bkfsohfw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3sxtxnfor.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wrlttwul.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3yzvzchij.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rxbynprr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brkqnttl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ctvibwgn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cfkjcneg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tusyjqez.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lujwgwat.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rfktqvkk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdtiyezv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3utojibkg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dsadokdk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pttolvfg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pradoudj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eglvttqr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxmvmwod.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3aomlnsfq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qkjeuriy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouppsdps.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krfclfxq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3djlcjhxp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qoidmunw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3pmrjspxy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3drjuifeb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mavbzguq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zqbwmpxv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vleiskyg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3stxgadxz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rlzktwiy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ljrlnxde.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3siuaczje.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fiawrwxk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lknegvdb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xldbmmiy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ynztygrt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jaeeuxsi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wdfzeofz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bnnroxkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqigtpfg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dihighxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nggtrgka.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bhmislbo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hyuggxus.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jyammoxn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lqdadrmt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksdujdxi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxfwaxie.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3lmilrpmo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fxjaqeje.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jtlxkgtp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rquwtrtd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qkwzldam.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbdtwlha.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbwydyk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chtddoze.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qjdzithq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3lwyskets.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ftbkjfwg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iufxupcw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3xmkwktwb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bsiwwhag.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fungtvcd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ujgebcab.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wlmqpqeg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mesuzpaj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mdoaertu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nyvnpqnt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bsvabfmi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3keradury.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3diqiufdy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gsinlgnu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ydykdmjb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cklaepeu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jpemziqv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3grlskqzu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xftxxllu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3huynguup.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3oajbcjvg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3smnyiypg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uusrbtjw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkzpirhl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fomqquvb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vntbpicf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3puosjxte.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3olxlsbcn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivqlkowm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3plsmymmg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ymhfeyuo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdnwhoaj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuvtjgdf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3twjlpnib.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yapensfs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3trxbjyla.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sropnpxc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kklxjrko.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3buujzfog.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jewbuftc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gxcgvbpr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ebtrcozk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mvfkrotz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wznkrzup.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wmlpgkfz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nswubaoi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cooiyriv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ljtbhjjv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gtifasds.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fbsjyljd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcakckoz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xylcvrgp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zuelqcgo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3majrjgda.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gwivkcii.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nqbosdmw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wmhgcbpz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3skkglpla.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyqqtuxo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fthtwcti.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lxinjylu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fxkbljqj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3aezjcqco.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3lotzxjkb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqkenyuu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3viuosyzw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nzcsopmp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sifirgsd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hbwrtxfe.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3redtyvrn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lthhrvew.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3atbwkhrp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vuwalosy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3onlyztwh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3onuwylzm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3otnnqlcg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ypgtrspn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hifxehya.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dzzcixuj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqnhfhuh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3slutttmj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ujyiuyca.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoxqlfxo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xnpdfltz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ljnvttga.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ijncknrx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zatmvllk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoyjmtwu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oarltltg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xsrlwxih.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gnhefvyc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dudrfctk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bmywsxjm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xurkhvuy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ocgjwafo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fwnjgqdv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vgbqriha.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cbbtktra.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3unbmjgcj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3oouryljn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wxwdrnzo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3shkmxmft.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3difdgjvi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3axlkquou.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3gibhavho.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vlddzzmg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmthxiog.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ivlwcyqx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nyelnqdt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kjhpjwmw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xzcuopub.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xkgbnlyb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3znlznxrn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kompuoju.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qqpsndcy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vsjspiwx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3bszkqtpd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ttzgjocg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sfbuhhjt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3othbaarw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3aoqagvgy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3dwlasjkt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hnyintty.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cnphkndv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ppsniuxq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vsapsmlg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3nraeivtp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vngsynut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjcfpzkq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mnxmiwcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wymqcood.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3poihatxu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3veltzjlc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wywtzamn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wboyzyxo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcwkjbuw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3oscvztmk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zfrnpgiq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3uyhotzgx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3clpjrpnr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xjlkoywe.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3pnvlipcd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mumkoqbj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qzjdltha.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dbjilflz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ysimfset.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ourrmaxx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gzrvrzxv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctswlrzg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rwmteeox.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ntlpzkmu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pplpkbxg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wumbdlwt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hburqqjz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3igjyloin.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rzmmxiyi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pnfjjuqq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qjaohsbp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3shetttmm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uxqoibit.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3emsvcoha.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ommnupko.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyuqcogs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3titabzuk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3uhpgyqdq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3axstfxte.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncggpjzs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zvznqwez.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hxztxixc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3cpiqdqlp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmpzugob.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vooigjth.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajlxxmkq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3gzykidau.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3mbhqjptf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3otzgbnyf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wvoxmlua.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ltqepivx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gpcebpdk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bmhuignp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hfhontpn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jgdqcwqe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3vqyihodv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3yjrzoxsg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3trtcifuh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3kkqxwivv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hwtqehwa.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fpkfzaqn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lhlalqzk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zktxtouf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3tkuyracj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3aaijqrnh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3rinzzpqf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wwksprxh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3dkgektmv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3usawwsmb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3fotysaho.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jfdawzjn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3cdzapubs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3cygtfdmy.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3cicadcmq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hthcoawm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3sobndkkp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3therkyfm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3gjlhjawl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3jikozumo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3shodzxuh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ryjgvfjx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcqnjmqs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3yowzgxwp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3joclctfr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3eoqywnrr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3draphvfr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pbktnmva.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3lbfpdcbl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hqwgrehu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dfyfazpt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3bbcthnpt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3tmpjbxdd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3wgngagqu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fqgherku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxxnsyit.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3mmuhfeqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khguzhhi.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3syfwlcyw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mjhzksjx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3idgbdbik.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ftgykcga.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lldpyiym.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3pafxdbdh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aijrurwk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wwvjzvvt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xynhqqne.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kiadyesp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qhdcxurn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zeghhydj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3hfcekcvv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3vnqchsag.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ryndqtfq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgonlfmv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3smpifkee.html


<!-- 参考信息 -->