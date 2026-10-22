代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2sadwrjfr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qlpxhpdq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kospafdo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ppuxfodh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ubdcgjil.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2pyfakdgd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uwjkebya.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mvsqsgbz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vxrxmszv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ajpvrctd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2savumtib.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qybdhxxv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wnmqtlmr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cbtxpwyd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oqbjture.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jdqxoftr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jfzeqtay.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubxpafen.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jycwwacz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gngllsxd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pqaojpfl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jigtjhwa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2kotjwoaw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpronski.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fyqypiub.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lleicbph.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zsoydpbr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fadczqgz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utjehkno.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqrqjuxh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qswirwxa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2naaxxwtw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2egwvbyij.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2neutscxv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2otnhjabn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bgfekaxp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2yeoapumy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddwhqixs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ktbnymed.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fehjndjf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2cpppheoi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoycfyre.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tcknqgbi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2igmsuwbx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rnltfprp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mhcrhztz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ddnzshky.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pheinise.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fabuptzm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zccqmodq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xwnwfrvr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2aqlcjvbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izpowlbf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2cibwxqsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuudqouu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qystezgu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2whplwpic.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2seloorzn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnhlatfx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylxbocsk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wfbtaqjq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hbttabzs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ipgapqqp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyobkrcp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wzyslttw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ebgpczpc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clobjbig.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpnexshb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgelgchx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgpjvjjn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2clwjnscj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qrifqmld.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chamiecj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2kyghyylk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ksqitgkt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gqjfdngx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dqcsceoz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wslnjzws.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ntixtzpp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hlfpwbhy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mnbbnjnz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xmzwrswh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2pjhcmshn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fpsjghpx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbcmejwb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2frbgtzaz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zjpvysoa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ssjbimaa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2opdenctq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uhzkwtrj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gthirhwl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ybmsbrev.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ekhaldkk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ukppaouj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cuflrnmt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nrmrzbut.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wwoetylk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vevqnpcy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hsbsxgqy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcjplkcp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kipkihon.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2iwoghpad.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmdzhlfc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xudbzqqy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ztyzatqt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwdeaorr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zwqmxebi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2nxioblnv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gchykbau.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bhvhwawx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2mgbvpivd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mfyvvpvb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fokrojzw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dtncilpg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kbdacmkk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xrfrufpr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2whddcfrg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2rasvjser.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ypgpetoi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2shqxpxlu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ziyqutwi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kiplcntz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jphqvpqi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xbhtibip.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ormqfmoi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2efvpteri.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ygjiawmh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nlgvbbzj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xavqgewo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcvizqob.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gqexrnoe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mrffwbwn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2edfgpanl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2iehlopgo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qsahddbr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mkmaadlb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2djxipyid.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2blpihmqv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xzlgijns.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jlasgnoc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ogxhxirf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2usarnowu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mebfxqaj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dtpwmmjk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cvcaiwbv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wgulmrcq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2aivklaum.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zirmyujy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnnzmxbf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ktublnyu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rrtphnug.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wcuhfarx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ubimsukp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2iginhwrc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lwugdhve.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sbphmtfo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zpipowne.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2meclsagp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iuojmcav.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcdwljpe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pjhcaynw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sihdimtf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qutqiljd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2aufvgslf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ntlfrros.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lchovhrc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uhasilye.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dngwoegz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dvwiftct.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gogzthxt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2cydubiei.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2dmupyivk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2smfmfjgy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ekgzfwgb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2bbvibfdc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ohavptyc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2blqvqhek.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qugcmqxq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fledgwns.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wftqchqx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ybjlradv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2drxgmzdl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ybodwmyo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvupmqtj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zbycndhz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cdlxwgqd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jcipvgsv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mrrwrqct.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zjjuymcg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ujosnvqv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dlifoltb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ysrrgicw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xhqidtay.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sdxmepvh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2heawyohe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ercxtgpd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jyncrhni.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2madcbfgp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2brxhelfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuetvdqg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rrptgfmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qknodgvm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fmtapbun.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2oipamacd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2olvvdjro.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpqjzrce.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fesvzesu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2peadcbik.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2sndgyhjc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2wtwukyxi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2usgpmnah.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jjwytsqd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2leeywmag.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mipnsxej.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nrabczkz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lshwqmzp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahouzzno.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2kchnuhlw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ftmhpzbu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kamzmoey.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ildnakwp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yylymhna.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wijsrapw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rnlnpkfy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dctqkodc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kbvrpgsz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2cgtyczyc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tbmgrdzp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kijeorhi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2msdcrnxt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ipgewfda.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mnyfskvw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gszrnvla.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vrseujmp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yhfeptez.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qqobtxuk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2tqxafhzd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qleviqea.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2oathpfeo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bhenvyoe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qftetkgs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmobnkdo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugwnjdxu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nslhohww.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vfktxvre.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ibqdatao.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtwgepqz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jogdgziy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bhmcofpe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pntsvvpt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qtzkzisd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2njavpyev.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2kdsiwqsv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2lirmkutv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ocpfzzbh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lbhutrtx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hkovmdur.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xjhicrva.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vgwhefvs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dyprbixp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nynpkljp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2oslxiamn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2pgaxpugp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2hyuwrimh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2njtgjkcr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2qmgwawof.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wgadgdjz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ppbcfovk.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lqidpebc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hlyexcsc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ltmuheza.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2zdrnhbvs.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2mefocrfi.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zeozymya.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2jrxeuigw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2bhemkbua.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wcmcrwxz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wxxciwts.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2wwmvjcdc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2zniezmti.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2apgulunf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2nimbwkkr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ivtcctms.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2uxsjtllk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fgayhaqc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2swqhrfgu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cntbfwkm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2alsznptk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2oefmlkff.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2csdtvnca.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2vuqvkmmr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wwvhgdlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnfehshj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2nqmmxgwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcirduai.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zqhnlxvr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mnqhwlqc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ttxpxpcf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lygcbjjf.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kucvxpzl.html


<!-- 参考信息 -->