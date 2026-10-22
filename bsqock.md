代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uebnmsup.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pnxglmqp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fobrchoe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2klywaeet.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2kmiiarmv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dejbnleh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vwxyhwmc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2uvpmeyfz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqbdapwy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2fumdhrfi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2raoewvdk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fonqfxfz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ijojfdwa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zapqdekd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ndsawxza.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ostthenw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wkmnzjky.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hcufnigx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kdybpqyr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mhsucalb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2agwxiblq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ipwuiitq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2sekyuoor.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbxyfsoh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ybrttunz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tipiuhjp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hczkmppt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wmprfidy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2klkiwsxa.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggxwukrq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tbcgbnkw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgdsfjce.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqkiffer.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vluzeeju.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2oeeukunt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhablbxn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ixuinrxf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sykczprp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtwjjhlm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rhyqmvzs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2aqbmfqjf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bohalayp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2poxwzxdp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ttpwuvbv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2frhefrvg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2khztqlxe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vomtkdew.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hhaufwnv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2akxcbyqn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hqyxfayd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ijpuygvj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zwbghmnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auznxasf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vknzcvpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thcqwosj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nggteqhh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tzdadvsb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wbbhdspy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aaslzvvb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vlsrbhdx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mkiuheid.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fxhazxpr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jpsrekvz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wnljszfm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2eucekgku.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2brpaivcw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jtscxzye.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwhiocki.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpevdxqa.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dtycgrtc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kqmsjmcz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ueafyqgp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sazxmfpa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2yfjnllme.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2npotoyba.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eohisfkw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lnzlobjb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2owtexcqv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ngrxgycy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dbhlzmvp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bbzhypps.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jutfirjn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tcxyzpry.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zlewldzv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mcjnkszs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otsxorix.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkltmkxd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrtpstes.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ezmutjet.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ttzqvjwm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2emslibxo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2umujixru.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lwmgfczt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2purdrnpk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wotwrglq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqjccngj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rkiodfli.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lnnwynpk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hvyolxym.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2obxjebzu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jwcreogl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kpbfsxrb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kwjyymta.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cdkyncqe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2klwqvxgu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmxgqbtl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2suqivdpp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xfwrwipc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2wkzgflsa.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fsokemqh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mnztdwox.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ckdfhslh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xckegkpc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hnjpanfr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lnjitkcz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jjzrpihu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ygeficug.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2guugzyxv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2sesshfqs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xbwpcscb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwnfdzdh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfjsnkuq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2chivwdyp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ilfdohjj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bheykvpr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zezuypgo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2tbutkgsn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cdoauyul.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yracqnkk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xmgyvjnl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2dlykcxzd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajwvmsfv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mxrrjizd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2swtsqwwu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2baimcfzf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zetrgdfq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sekknmto.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2khfgukds.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dwramryk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dxhhlboj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dgzgifim.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qerwvobj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2dvymcost.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bpzrdvup.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mxlpgkcd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2fkgzevpj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2udriitfq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ecuuospz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nxsdzhbm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zhetqaoh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxnpifff.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ititjcck.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bmalphyb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gplokkcm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sogdnovm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tswscszt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2alsbovhb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cymmpujd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2datyggiw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ranfswpd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lpsdtopm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fabxjknk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gfcgonay.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmahvggf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rveknmdv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iucyxuwd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oiwzwweb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fupapdxy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wysmpmdi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2iaivvaei.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2kbdygmoe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uppreywc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2uwtljbfw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mclforar.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zuckqfbw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2dlgmdrrs.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rlgpdvpp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxcyaytu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kooekvjl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2guolnsre.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2sdespalb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2zzzmapqt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2upitnoma.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2tahmskbf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2kflciwfl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xizvhtlc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2bvfyhpym.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yizwqoso.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zhuqdrsa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lrttvewz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2skevropb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hmwzsgam.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ytbhsona.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gtivbjuc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vustaxyn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dncegqae.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2uiebmngi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mcglausr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xdjnqxef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygyqxxph.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2erjvoequ.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zaqmmixs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nrjjxmqo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vxnlmdck.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cecorafs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ackomhnj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruuxoofm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2bapdwrpz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kpbsryoh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ejkrzctz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2wzkoycsl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hpagpsgq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jddwnsil.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlwfezfz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmogeaof.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vxiqooch.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iofimltd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wykzsify.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qskfkjry.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyknrgdl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2czlfjtmj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vtlwepit.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iyedayhy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tisnnaib.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pzsfuock.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vynueejd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vewdhefm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fqukadkp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2casrpgxg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2erswngtu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tlfuzuoc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptserbip.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2afhznxln.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vfzoijux.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtwagapi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bwzfrful.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jofovdtz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2drphjlbp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qcmxvhvi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hiivvjwi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kxqbajzu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ufsvwvsk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cfwgyawp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2xtlqsrxn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2lkpafzbr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lcnctjfc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ciqivyzr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bgmlyuef.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2kcyncxuq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jgnozrpe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2reledawf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zagepfyv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ryfnfiiw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hxpvklrz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qbuwwaxm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2kiqrtgwc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2knynvouf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2tztgwyud.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tcteylsx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gsdpbomp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hsvxclmk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cxqpegoi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qeubkhbm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2blqautda.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zvxqugph.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2efcrvjlp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2rikjtdlz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2zwezfsxy.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2vidzumxh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2mmyfwzhb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2lhvmfjmz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2quynuprn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2lwtgfnar.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2wzwjiffa.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ershodww.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2criwjgbk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wozjohzb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2sthghpru.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2dcbwmhpx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bcvjmnqd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bvnlwvbr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bjnooalp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qcgphlyj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2rmzkynwl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ytghavif.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2brumkpkv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2suneiisf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qjhnaxkm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ssmsnhlx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fvftbbeq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2uroyhnuh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2feuddcbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwurgtkz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bdmncgxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxnmeoju.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2mjnontxw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kadiguqx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hoxualoa.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nethywxp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zlmxqayb.html


<!-- 参考信息 -->