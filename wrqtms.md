代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lvtedzmz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3akemznyy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jbrsaswt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tcrhfiqy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dyslnymo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fisunsxb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mhxvofgg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3oghvcnre.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3htgefdkc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3elkzwgfx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vlzukzoh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vmkdqzod.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dqrtfzwm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ljwmqxok.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dmwsybqn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3sfesvova.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3foanjgcd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fnobetnq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rnnejxhs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tyjkzuah.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gxkkldtt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3okfjdjnj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3yyewllvp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wddctnfb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3nhplygav.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3rkosvfbl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ecdceclh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3taukfmxp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3njkynmbh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3akngepxa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ssfzajcl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xypapisx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwousrlo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3okzvdxwd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhrtsggr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tlemdxrs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lehaibvt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3psuwckzc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zozrylee.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bvatrrjt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3qvrywexu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3woptjsig.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rmriirgz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ypygnsoh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tcdfsjip.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xixxvoyo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ljxqvoew.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xlauxpzb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vxzwqzog.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nvlmpgss.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qmrwfkra.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3qarticlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwlionqe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3yznaftem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntksapec.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xbvjjtqz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mlzcqhut.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cofnxswp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwnhzxiu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lyjyumku.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3updwixop.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ifsebusl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rqumaamw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvdrdkru.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yfpeewrl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3pzgfdpww.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rkoelgpk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kjxigksy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycqcbryu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cbrpwujm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dcrptjoq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kyopildz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bezzdxdy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ytirxedv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jjunnhqy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pojoxikj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3suqdvngl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iqlqqqnc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3irzevlec.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3stajmiyd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3upibklra.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cvuydqvw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lmzyypyb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ufdusvnn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wozcgmfm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbtvzjyj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3klsgivec.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3swberozi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nodmiuow.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qzmexnrl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zjlsaiis.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3etefrikf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ubumorzt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkeiljnh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqmcikhg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oreenudx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ejcgqwmi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3sxsaqlaf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xviqveqw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3enqwkdjs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hnvbvpav.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tzmeizgf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wjgdajtg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpzrwxwf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jxfyjkzv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyzdxxqq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3yshyzjlc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3krdhmpcw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gxbtdkpr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wskxdlsf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nggznilo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pwrvjmxn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ipegaxmb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xccywhsf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lfpzomjf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3yjtcyjdr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wvrnjwvk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nkbwplra.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3iveroouo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3stzzxida.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pdftxtii.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xqkrvtnh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3oqfhvxxe.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfsxrfvx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3nsdihkgj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xheavevd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwulkzgr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xjajgyqj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dzslwnau.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dbtohkjz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jompfzsu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgbtlded.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iezbpkxc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3punfxxfc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3icuitftz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3heeyqcii.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gusqrepn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rhgehazj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3noqsgrvp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hnhhzbfb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kvwcribl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3pnnqvgvl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3yzilumef.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dinguour.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3htbherbt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3pewormfu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oxnrbson.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxllrtxp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nadxkqyd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvmcxhiv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3huevpsbr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qjuyznhq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3kabnizvr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qlijjaxo.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vghxajsv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jnwyvhkq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bvldpump.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeenpjct.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3duocuqhh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3evkdtwwa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3omdzucuc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uwzkxwko.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hbwpmvrr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3yberfnxz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3pqjpebwa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3azfiyaoo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qjdtzzyq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3csdiuwxw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cwnxzvuv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yotwjsbe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jvtidrqt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dcmtklif.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kfetdtjv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3bxbrobxf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jmkcurbe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pqsjcvan.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3eqarbfqc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ednadgkr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3nvzigrub.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3cgdwkzut.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mtippoeg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3fxzpaihg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kgbfkvpm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyauboee.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kgkwglce.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aexfaftx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3kjleoftj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ofjfovfe.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3fzhpzfrc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bzanmnjy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pfgwblnz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3eykzzkan.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hkwmykcf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dumvtntg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gcjszfip.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vaqeltww.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3pigouebg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3aryujyxr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jyxlbxmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfqwmjgq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3conorgns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lparjrbd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3acdjasec.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xsfywflc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qfeehntl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcblsela.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3waakrwhy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkhyxwcd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bthgzysz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3quwkgqww.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3tityxhwf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3hffkxhtv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wypgpylx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ilgyhmpp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebloeckt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nssfmqec.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3euupljei.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xmjqqxcq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3piilyzol.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuodryfd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dnalybed.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3iypkzgkc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aqworpzb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ljwvswrv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uixxxrch.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jatodtbz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3kftqbntp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hrvnixvp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zufbzniu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xqlkivua.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uuzmcfue.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyhejxiy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3oljvtonp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wszvpdyo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3sdbtcnoi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hrlpblmn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bowfckzj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rnaojgzx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3lngxcwvl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3eadqnmum.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bslanvid.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qnoztrsj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuenipbm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3tdcwqysx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3rzngzloz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tsogaquj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpypdstf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bcawhcpr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ilkmvmeo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3otrilwtg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nsftdstq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3osuunzru.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3htvqdazd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vffrlwir.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3afieisqu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3olwyzlvb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3gpzhtsoe.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ywdntxeg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rojbmfkr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xfyzmrgw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nvqkfxgv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3vfysfqio.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3rntgitst.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gwmbzeuy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3djzczyno.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3pyhqoeyh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3hmiytcfa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3senbxjcf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3liehbnei.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ckgxcuyo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3yznccytr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3vqxrwscc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3hkojtqix.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3lymbrpxe.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3tlybzjuk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fpaqqwgv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3twxevcxl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ebtohwwr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3siryrspq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3qcgsegav.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3lcppjrgt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3huelqvxr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3wiwbmohg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3kulkebul.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qqrqzjpt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3tfeyrspx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pecznxva.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tebseyue.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3qhsylebf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3wahdsfut.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3mkhyixge.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zbzuodze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amtlfkdb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3llvkefls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjmefbmq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pqlinape.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lcfydsaw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sqqwtqpp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnyogklg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3lpuwjzit.html


<!-- 参考信息 -->