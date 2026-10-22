代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pifhxaap.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zvlrrhbo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rzqdowse.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zbuqperg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2srlufikf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2fjfcygoh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mnecktke.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2effrvzla.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2umtefxsu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ujetiyxc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wzabsgvl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nepfhdwl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2agozzfto.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmjmfash.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vousujja.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ewhjtlgp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rkadrsoh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vqrrkkuq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qpywwpmp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oocvczbf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fppejfto.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fvtvoxfw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etkljjvl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qybqhwlm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hceneybm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwtfhtjw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2oxckmlyc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipsmysdq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nswabizn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cusaotdq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2megauzqh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxmfkixd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tfejbwph.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbtalcyi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykmuvqyi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2napszbfm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hotbiojv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmuwpovn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gqkiketq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2bisuuhvq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2iqqzokwq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2sejxnmvt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zxgutipb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2chyepnlx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2jwsdxvpy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fsfgvdyr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nzocbfgi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qnysazmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qljtqjgc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2wfjschos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdslnhkl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kcyumava.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2soogaipq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkgiukqj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2grqmvtpo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lblrfujj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqbcytfl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lyojgxyx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pxxopvuo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yhmedhun.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2nzhmbazd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2slergyjf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzguwnpf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xfumkign.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtibdbsz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxjjjwvn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jljxhvfu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hckfhajz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dzdodbjr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2rjjrrkph.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2loigifkf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zpyswkpd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ihubxeig.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tqkcdyef.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ctfaclix.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ukwkdmfm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qdhkuzdz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2boyknjeq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jvfzlhvd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jicsfpkv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yinennys.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzsqupcb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2orfvfrxo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cfbtckye.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kizdjdks.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2elavfwar.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nxixmhil.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ptmomkzb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kkqezjwr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2scoewnfz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2reecryxq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lpbjhcny.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tyxraiha.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xhdeabrr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nickjhnx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ouloqrax.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jtnsunfj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vkmbkbya.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2agfxvutz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unqjzynu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xdreqncl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfkchazy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bqfitzjn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2uxkltric.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tizbcvou.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2oonqgrwz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2kqirtmwr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2chfvmbin.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fpqobjyt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oqnwfltb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2thhiymvd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2naelrumh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2klbvbibr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ltykqbgb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kvlqqojg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lyobpmmn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ylrhtjwe.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cemhptxe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2veixoqfr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gswhwxsp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2apqruuqu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2cyhmxbyq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbfuzhgc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kbuehqtk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rgebhpuk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mwuubgsb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yggoudli.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ofwckvyi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2emgbglwx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gmvgwclb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yqfdydyq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nzkyjheo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pdekcvjf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rlagkhfy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vyzbwwsn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2yfgsemyt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lffuhcob.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2nzftbmvc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2uywxbaej.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jeffiihe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2imsdmgwa.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fuutxluf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2snykvgjj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qngbnoee.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mgatlhnp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsnqseit.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2txlfzrtx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kubeyhju.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jhzvybhd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nsekzbjm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iftefdfe.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vpducwou.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pnjjarvg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vutmossx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwgpurns.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cknhwbvv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zskkgrlq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tbfvobfh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wnmapplo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2uywmjdka.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dqxmvejb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vijcipda.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2brnnzcyr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ryzojlpu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qvhelxha.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dguulhfs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ocpvghyb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vrbqodtg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cldylnqs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2sxgeatgx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fjcsyppa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2xwytvnzn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2atckycxm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tvrzozzn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tyzfwfaq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2cxplypsf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2vlwnpsje.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2sibmerzl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fosezrdj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jticwhmk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mfkmqxub.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hwhkwkjo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qgbjxorx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2usehynuw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hwiitmsw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zmcccyhl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2rcjuwsdg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2otfgknqq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ruggivsx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjyrgxut.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zumangxj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zjpjucui.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qupbwhst.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gvtnmtsk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2exmkfhtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyiotpin.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lvswdkrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghwxqwhx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2uklmxxof.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xxvzuewz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mefxhzsv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xttvtnvd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqlgounm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2qjaokzlh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vtypioei.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2aowyuvze.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xkydguzi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kubqrney.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2glvxyrnc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jdeqcctr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2peevilut.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zsquotge.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2khjlpnex.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2oelmnywa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2exzszjqg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lhuqlpsk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2paadziib.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2kqexyxyl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zipbatiw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tctaaxuc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uposmytb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ikkvmqop.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mjujphko.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2gvuhbkun.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ezqjqrjq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ekqzcihj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rnguofal.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2szpgaikd.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjpwooya.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojljwrno.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2heldjsmv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wpcskueq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vuwuynwb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuwgfkvt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2aasnkadu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ewuiumbn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qpnqivia.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fkmwygcj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2povaqxez.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2umtfqcpd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fptfiurw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ejpvamtm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2horcbznb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gkytziyf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2frsrrrkw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ioqsbcnb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bqefbnwy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rjdmrahy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hfguzhfj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2mnspvgyd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2uslwpwcg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yphhcaya.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gredrsxr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2kyoyipqy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aabksffa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lhsvofou.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hhdqgglw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2dhaahnpc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2oxxhsszx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xjxsbrir.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ovuztjwz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2mjmjatpb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2vvcslbpo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rqbssfot.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2cxmbfaqi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2sqpzmxud.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2haarxkht.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2hdaqblkl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2lvnunofj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2nvluoqkg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2iffprnlr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ybklpnrw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ckzqmket.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2uqeewcid.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2pywqkzgu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2mmwqclgh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uhtteyyv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bmjsfxnw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2izyxpsel.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2syjrfrdy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2qkymwwxx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dokyebub.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2byiqyoqe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jdrfseiv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2qjzawvzs.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2lbqgygnb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rdpsyjhl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fqtzcfwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwgtrfta.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2njcaldyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtxihwfk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2adetyxdf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kxxfdwlv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tdegewfw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucqzrqbs.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fasrrgib.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2sbuqxjmx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2beszsmve.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nqdnsbir.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2atbatxwk.html


<!-- 参考信息 -->