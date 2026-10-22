代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kkktyeea.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hwllycyn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qkdfdauv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kubuxadf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xeklwrsz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dvhhsaev.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xwypmwdb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2toodxilx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fjxeqwkc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2sznthhkl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vhefgbzm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wthdgzgx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2yctqdipe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vdkvtaue.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jfrqdbbx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oizvxqsm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eiahougl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2uojgjhnh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2puiaxdmf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2klxorwsa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vhyjgrqo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gztdluiv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nqgwbnmn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yrnwnkjz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bdkmrelj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vxwingbv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2msiohdei.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ocmfntqu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uzldmnyd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2aacgzmaz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhjetmdm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dtwagpjd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjsvelgj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2przxytnw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tckbtjoc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2narncmis.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqzuxfhl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnlslcxx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezvnbjyj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2muhztspf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zzcljzxq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjphkmsf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kphlyjxk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2umzvpuiq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2dcxckpmw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kkbuvcjd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jcpanhdk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2bquwpuya.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qeqoxqkt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qiwxjmph.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xzpfhaek.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fvaziwcr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2uhspgrvc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dfqcafbb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tyhyfrdi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2gillbosv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcdrmdrb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vjcitpdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfvawkzo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gggxceqd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vcgvtgmf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2yfjxachw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jlgfmtih.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2beojlaow.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tmbhykhx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tcikyzyj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vhpuaxip.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vyarqowo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2peteehfo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bfzphlnx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhxazztu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nfgjgiln.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uoncldye.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mreowtlk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2otasaykm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2iyqqeibo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytanktnr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2khajkref.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2adfysqkm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hqiupplu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2koponeza.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tlctyudy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2shteqnji.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ymnqzqgf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xqvdhylm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tqcvfogj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2yyfcbbsp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mnneplmu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gbpzfale.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sbsijhea.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbtbwdrm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2anprayzg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pwmvpzaj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2eusxmosl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uzqukmdp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2woxduqdy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jipfpxej.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kkaxlmav.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2budfrtwp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2euawbduv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhjitywx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wwjohiwu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lfyarfgp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rwqrnxnv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2sbpwvpbu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2naxbgptj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zojpdcrf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxgycnyl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dwxmzlls.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2irswhnib.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zaaaztil.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kjrdwkoc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2wtrsavdz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2oyjxdrfu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2euyhculx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2tjvgfhry.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rskknuhi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vgumgxjj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vsaimzlz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2bkixiirj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bdzibwdw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xciivevq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2nhkqpdtg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gwfltwvr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rysafqqg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnaucghs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncxoeggf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmdriyzv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2yodfcbow.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mzwuxxrq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2blnctxqb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2waqlrmkj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sqkwdneq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jglqmjpo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vgyfkybw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzmogqro.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dhqvtgwv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2jpucqjon.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ntxivvmc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zdnquyzu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2iujqtwsy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zpcyrhml.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yqljwluy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pbqthkfn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pfmleqht.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bvqpckcv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2woczfrju.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ajleahbi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mghzcuto.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2walrdvcb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2paeztkmj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuaytcgp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epbdqfzg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qovrrxbp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2udcccdpx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vasdvpqc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2thkmhjcr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qrixdzod.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cixoxxlf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2etkqwqhu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aoovzwug.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2azmvxmtk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kgtmbzvp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eqsndpud.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gbleuyyu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2twwqgozy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ntlppphe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jtdiufim.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tlqgffxb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kwfpbfxz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2whhtcwin.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cfprymno.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2marfvvgs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2stnsrvrc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2azitkitg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hxuboqmg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fjnktzvy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mhetdwkg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2exrvsdmt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nzolxwpr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xstyyobq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdhoxycz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ezstkjmd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nihbkuhj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2daltpnhe.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kiltgwzd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qlzrbstl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2egpzqnda.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jkshfymq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pmakwegy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2bytveuyh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qcmxqfwp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uolfvyuz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wpvaynda.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ksqssiqw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dzsiwfsi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xwzcitum.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kvazfxsv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jngaehyw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2brzkbmyi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xnyvbddg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jphcexte.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ozvlvnoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxszozeg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gqtsaqdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucqxwpmk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2svjlewie.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zazwqhjp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2woqsjgmr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sfzxiolx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uundezno.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2czcvfgyh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vhuptuwu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ymljkvow.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vglkyoxw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ryrtfvnm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2erfjdtvv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xtexsgjk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2arbhhaie.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vczppawe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ivkamgwh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lolpqqjj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2uckeznyn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbfzrsjh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fcijuniw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2njfxmhvq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fgkxhkrn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ifveclbb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ojopftuk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dfsiyodh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzxvhnr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zeugprit.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rlhcmxih.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2htisybvz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2chltjdqt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kseyldhb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qntbxiji.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hkkataxd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wywkhxlm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nwhrmadc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2cwjnarxq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzmcgekt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2csahlxaw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2btgfcbla.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2urnptpur.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhaaqmoj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zuwmzdjv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2jxripaii.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xlvyyrus.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2mijxlcwa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcnjhzxt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2wcqfnkdb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2aptlgsak.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2slqtznkn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zdmukcmk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tfuyvbxl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2cdjhablo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2nurrswco.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2uggwqcwk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cdwzoirn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2zuzzpmxv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xvgbkwes.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hpxfzmbz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2anbmazol.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2munyyyfj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vocisogd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jmnuqjym.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2cqpcqohc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lhrnoygr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2vhvfcjzy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2mkkgydme.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rlwdfnef.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lsyricrd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ktbhilzy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ixlhylef.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ztaefwic.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kfkhmczl.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2asdmigsc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2lffgsicj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2htavgwml.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2veetfziy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2uykaembo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zqlhcyuo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2irjeqbga.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ccjvdbeg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2waptqncj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2nyqzzukk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2atupkklt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2kkhnfpfj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zaiwqsss.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bypjeuso.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tljeqkwy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2bwqocbwa.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ztwowdbk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2sjrjscdd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lmpjcfof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzraiyhd.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2whnzsigy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brukrbnv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wlurqlcm.html


<!-- 参考信息 -->