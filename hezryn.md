代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3deysdlai.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qxvogaky.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tlgsxudl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hwhefogg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kjgjcjsi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3petfbrql.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3aruceatp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3whjcpvav.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bzwqslfb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmryhnga.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yghtdahd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lcfjtrdg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3taesqksy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vdimxxhd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qaczcghv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3igcmaoon.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3valchksg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejhxpujb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nezyoknd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3unbagybs.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3buslcmgu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bhpgfuxo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wkefanag.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gzcsxkmr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3aynqdpgk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dqfbwnju.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifiijlrh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3opcgmamn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltunssap.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dohrbhfo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3stsvgysm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxypjrnc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nsxtdkdb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stewmvts.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqgygxmn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dkxfygdu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kappbtak.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmuumlob.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnlpwalo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vlgoqdrt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3uppqlitg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cplgnahi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3sxdchslw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xkudzdjv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3swbcybkc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cefmwdzb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3nxylvkfl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tdoniybt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3eghcklfl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vzikzfjh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hromffdt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xsssqrju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upnggeuh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3syuefzcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omrcmtlx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zjmknwam.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3eowsbduq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmlnhrwb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfdfvsai.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3urfytrvi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3aythiwfq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3itubqeln.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wmvjgnxi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttihgzrd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ixebdgmt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zfqzazcw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vjgskooj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zcshlkpu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmgkrwqm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pighlszu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xsqimkot.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3kskhcvng.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkjvvyil.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3twkovjxc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zgtcgbhr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3eglhbkzu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yrlyvhej.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3pgprdovt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qjkjzxqn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rlomtose.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3iqlymbsm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3snubmqhs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rwaaxogk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xjrkudsv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3embmbosz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvclnupd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3doouyqhx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qvbcufre.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vngozrve.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yxlwikrm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ajyklamm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3iavdtdqt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ecioydtd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtnyjgyq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3riabtrzm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3itjccpiq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3upnmfnbc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fkerktfb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hilrvsie.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvxnhftq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kquhyxoy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3nijcrcbr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3akyxstvm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxnyycad.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nybqqrnw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtglhbur.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3chapybgq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3leepunay.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ndpvkqyc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pdnekasn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3yhigkisg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hcqaqbfu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wntxezsq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sfflwcaw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fsxntriu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3nhmazhwy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3auywkgbo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qmcajsye.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xczsykmb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hejcwwwg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxriaymz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzqxfpmj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjcipbco.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcavsvua.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rjpwocry.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cwrmfwqh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3oxgbwoxd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ookldkfb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3yybomrgr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vwhqbblw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3perbyirl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3glkmwxwt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3bwvdprre.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hacfaxch.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zvmpwqia.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pkjgusub.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ajgukcej.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wmkuswnj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eqpblqic.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mtilpufp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fnueekdt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tfhtlyzc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ngtechmv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xpidiesn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3nthmjmbt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3pxqlqsxs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3urqnioby.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqhmmedl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3satcyivu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3emdlwjml.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eypyblas.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ueumymzm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3eqccvumm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhghlunl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mjrfoxhz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nrcgqlxo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqmkzfsj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cziqlgej.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgrnclgx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3quqiqrlg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3merbmapz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bdirzakk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3meyjynvb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jdmfzruw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3smbvbebs.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tuysnydb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3leribkfi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ckhqdqcw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cwvdlidp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ymnqwqra.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kyiacqal.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zdgbbxkm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xuxpmmjq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3yqwwqqeo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xfdqctgh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hritelto.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nmliitmg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snavhcws.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3nmewgrdk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tgdowqho.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dkutzdme.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dtzndmib.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3muyrhooc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3xzcplmcf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nmxsptgd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bytfgqsv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gdrndzcy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3glswkrqb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rusythfh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bqtytoyp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bsbcibyh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3grytktbk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zgxqnljd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3axapaoim.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yhjfghcg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3radgrgvf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3kdqneber.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ubyspjbu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ijdmdotl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lryfhthu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ydjrtspt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xckntlup.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3sspvsuha.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3eqebjccs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vugnwlvr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3anmvkotm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnjhfdsi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3htphvctn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kibzkrbk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xzczptbe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qibzsblq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3xhgofcjs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3nevkmdmk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kaobgggi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxwtqtct.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pourypcy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3modeuezw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3lwnfpogx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3czqmlaiv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcjarcen.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3snqvyvpy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wagcowrp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eyzcxcmx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3slegguui.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rmhlegdc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pujphlzn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bzprauzc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vtpxozlq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jnovstzx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3mourtqmq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ppzktezs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jupjpahx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmtfnisd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgdkzlab.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wmkxsqml.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ffpwqmqw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3psvymwlv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftewsaek.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3lgrdoigp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3psktuedb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3toallbaq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvwdeimd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vqcojacn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3tjzicpsv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3hsegorbw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vepyjnjl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3cxfurohk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3eqjeztmw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ussodmkv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jusymdwi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3awctkjgj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yfljyqpk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3dtwntvdt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3olnqbdyx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hyktwgdt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tydoinsk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3offoirfg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3wiqkcpsv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rjzzrbap.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3onhqwlsl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3phyieiex.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3cxrjpjjp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3buejervl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3nsabipbx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3egwztycz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3rnmztaqp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3hcpniube.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rykdhuzd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3nlosilxd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kxjtgohi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pgnfzhaz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ivjuclri.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3meofqhpk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3pifvcahb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3zqpwgoqu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ocaqsspo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3thmoohew.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uuwevrwj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3knquwhae.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3qalgziax.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3pljmgqoq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3htttwuoc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3omdpcyid.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3fjyeohzs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3fvwfwvmt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3eywtmbub.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3eldvwsat.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kzffmvxt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3mkgugpsy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3myvevzwi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3pckfpflp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3strqhwyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psdboqpx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3nkfdgbzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqvgdpkn.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3rfyweika.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtepbdrm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mjkzvwjs.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3cezwlrgi.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tfxxpwzf.html


<!-- 参考信息 -->