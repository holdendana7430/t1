代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3duqkcwwy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zqhxioys.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lzpluqcr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3apmaqdlg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3mfgoayoj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvteeixl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3muuhimir.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cfxatrmc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3febxflpm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zatotxiq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nwmeeqdv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jztrnlrx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wilajoub.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igfndfio.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3okhulzum.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kaylmcjq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fmsiyxoj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ligoaavw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3eilexqnk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yapmcwjl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mrqsirtx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3uuzvxsmp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3htdodkvx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wydnxmtn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3puwoywob.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emhhcyni.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3tbvnbhwz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ismihzps.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3naivtwlu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ndpllxcp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nywubnes.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnepvwbu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zznmnljo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmgnqtux.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzlkgvtd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gfzksbgh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jmaqspqk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmlnjitd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3aetsrvmb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wvpdoocc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xovjfehv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jnwwwmux.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3pcjpdlly.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3smqdhcfn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ljoekqef.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hnpadatv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rnvhfayc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3paybznls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gszxnguk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xkrxmoff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjvefiqt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3teuvayof.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3yoavihfr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ekwwbidp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3igdazgsg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntwrnlwy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkjxnhaq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ibqxyxnr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3slvtuvin.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bqzmypyd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3lgyydhif.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3uxlwtknw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkavokse.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dupywucc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygdpqbya.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeczugth.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3drtcihjo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3bnojmljh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqalgjov.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bdawkhck.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ghkvksjc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ueqgkkfx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rongejjm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3cddyatur.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3tnwqvmpe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xiodeoga.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dznksban.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cqgqspqo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yxehtrrt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bqvtgyex.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qilkpyth.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jwomfvcg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3axucmkaw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rinxsrlr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wfpcwrrs.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rforxgsg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jfxqvzxr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cgftxstp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jhwxefev.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ntbnrkhj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vqpoymun.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zuevhzcj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwetodab.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mslpqwvo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xzuyxhvi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3trmajohm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3imhgnczr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kljbiiwj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3angpiwsq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3psqabxbc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yjygndnu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlgimcmn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3olkqutvn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3yqdrhjax.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3olubkajc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3agksxgwc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ctewvnom.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mkvjemwi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3njaakpvk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vhdyahuw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nannrqjq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3troyfahd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uvfiltic.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fsivqqhx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3tvmhjjli.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kyrbymlv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3avfipehe.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhxjgrhf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3igsmlmse.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebweeuks.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wgxydmbv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fbzvvbwd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3lrzdxqyq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ghpfhmpb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vmhpsmcl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3uwmxwzto.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dwkhuqza.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3okkubckp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cyemmnrr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fytsrtvq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3orneswgg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3krmloedn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mngnnbxi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3edhmytxm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mbdggkko.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3tnrhxviu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3elkhsjjt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3vxcdoawa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qvnbbplc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3thsfqtua.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zztsbaer.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gcclwsck.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3iutgrust.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ksucixai.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfzvfztf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsowwgsp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3azmfjvwr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rpsbcvns.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xvxjtzpw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3krcyzjno.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xwlssywc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sxpbrywi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yabrasgv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dllampdz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsgzulej.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mcjwjmqa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vxltdcou.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uhfssghr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3civppogh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ycbcfodr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3pbqczsgi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hmtrnmdu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ttdfipmq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ogxzngml.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kgqqkcdp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3umfcwjeu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yavwbfbb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3zafparsa.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3isyjfqxk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cxdgzvac.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ehvsrvpj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ukypftvr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3bdieblve.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3aethwyzs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qbgqxfvf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qjntrxlv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3zljcbprq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ckzpaepz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fakehmcd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ihstpelf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3iapmplln.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hxvmnxdh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zdrtynhs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mfgmpond.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3sdaigzkh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qxgdgtyu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3jnfklqid.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jficutre.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gqmcpcrx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fcijykmr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ogktdwke.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hpknnbot.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ndwznejf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vdkrzeri.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fgbgumzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpkyhtfr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3acobdkpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmakpakv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rizphykd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3aktfbdgl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkqzqzcq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bouwqwib.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sednydzf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcchxotv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3sxbggjbz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ueamqryn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwmlkhtc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3jyjbwfrv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hrsaejbv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpdcbsan.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pxtsgknm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3edpuhcvx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lwtrwbro.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3epmojcnt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3owkjsyvc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrikhjnj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zmwixdkc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bcmruzoa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sormfgrb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jhgpykpd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3chulhycx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oevqdepu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3szteemnh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xepgdbiu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aledxyzl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3pxfpysca.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3uimzlzmm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nexmqfji.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jqpzzgtp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3uocepnfp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3utwxwjav.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3belbmtho.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3irlkjvdk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvvffike.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zmokfxbr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mjxofcnb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3oecoxdnd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofzvmdbq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crpmdzic.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcbxtovy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zojcmoxx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3pjzocanl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ldrczovk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3uphsbgob.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3reioxxrm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mnuajjox.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lsohidrp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fmlqpqsw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkoriak.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3amildesp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3zynjlpft.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rywmjlsr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3yvoamalz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3phjxramy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lqnhixks.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3owxuwxic.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lruqcwyq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3wtplkzds.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3nsrxtuad.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3xxkzujyl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vbdreqkq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3efmbzucr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3uzxsqdsr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ecoydogq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3vqasaloy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zdvpyezx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jlxujywv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rhqqhofl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3hqcjugbm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3rllasotf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3gzwhaflr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3wuzyknqx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ncodteau.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3dkmmlhhp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3owzkewbq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dnrjjzjc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3rodeckni.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3owlrmise.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3woqblfmk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3cbogpedm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3lecopeoh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3whiwcdql.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pglhbujr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3elkbhqno.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jnjjadke.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3lwlgwkxq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ahlaaxjd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fyurhhrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzjbrxfe.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3nuholium.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdmsclic.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3slkllsoq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3leaqysld.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dqddfeaj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rydnjosl.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvqqcjit.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ocdkvqcv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pnronhfi.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jhponolp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3aobuhicn.html


<!-- 参考信息 -->