代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2smwyucbp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2czdmmyyk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jvazkxgy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rsjxbeyr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2smjloyam.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2akylsldd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eloybhnu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ncifivnm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hxepjnpr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opzxaysa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2csfbqomt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nyaybcky.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kikubsfw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rricmrmm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rgmvmkde.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxtbxuis.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2evstumnx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tkbnlnij.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yoizcjws.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nlnfbjkw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rllieycx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zewovtax.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2twmrddgr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dyieqgqj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jivzfcvu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2awllzmhh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hsmaordg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqtxnzwt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ipwknpiq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skwbhxph.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gyltrehy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tlzmbcgc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2fktvpkov.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sujqykbq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2yfohgldv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2apmrwbtk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mycdibuk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hbfygrpk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2maagikma.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lwlrgvet.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2smoyysjp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ywljgplc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ydnmnogg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bhjvrpnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czmdayrz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2gyfawrmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnfigjdc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2evnzixga.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mdbfezdg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gklwdslv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mzbghhfi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2eujnlagg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2npjkgqhz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yzdjpexo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zvvhkoan.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdimvzmt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvwmgpct.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2fjsdmkfs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejsdjehp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhyginph.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2urifdvic.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2enhikise.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ccytotno.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qncorqju.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wykxkxpb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pnazvrrc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jitkdvyd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2edgedftk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ksjdpwee.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dqdzjgkv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wyaawbtk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ajfmggin.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nhiwgbjh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ahwpvxdv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2iseqoxtz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xuzphhft.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzcukyvg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfdvdaoj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjrdmmjm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbjywoxk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lxhieqrs.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xyadqbzi.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jllmmbot.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ihhaqakg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vxghfwpv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2olvrbjhj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujwctnim.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieqyzvyf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aicvlgbt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vvyhqzea.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2obniehqk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2biipcyzp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2okqadveg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lujsnkha.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2txkrnypb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2evjbkovv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fmkhrwof.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fatyxsjx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ilqlolgi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lvmegihg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zyrnevpt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fziorxkj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qbrvdvbb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mufjtblg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ssjjobgp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2frjewecq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aymzvvqw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gvrkmqct.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2uarqxrds.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wfpydgpe.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2iivjxmid.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lcddyeym.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahtzunum.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ighkhtkc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2scbcyvfr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bunzoqnu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bwqlsmaa.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ymhvpvon.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlqktkjb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qntrnnqw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vwynekwd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ahlcgjle.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2latffifa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrnoooxy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbnwwpom.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nmeuyhbn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2iyjlbqhl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2imrxctbj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2acjqdwoo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qahsmllj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wyouyzhi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2fgzisklx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zoxmnkwy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2krkrgkhs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tcxmeshb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ivbcjiqv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2iekuxhqp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2poosulee.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wszfbweu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ykitjwds.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjfjnxqo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mhnktoec.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcjzvcfl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zljusyqg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ntwwamxn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvgssacu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2aogjifbt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wbzmmchf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xaiayscb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikqwwohk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wjkkocmb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2niusefkf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ykhhvfsn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qwjvdnef.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nbotjqim.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pmghmqxy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2mczsomtr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pnylwbqj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jmmnvxsh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2olkenluo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cmpaogjc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2oqmarcdf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tgqwnjsh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jvefdsyu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ssytnpxp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2nagwnenx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jitjised.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ziutmyzl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2bsttsyao.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utkgabzb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2aoqffigj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nexihmbr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2alziwucp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ajdehnzo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2aysnqxps.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ohhyoesd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vfhfqidu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kdjafsye.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wcindgrv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbkzeey.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2biyafial.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gnxlbkgm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xbqfictv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2rtmqyolm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zpmhbxpy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bzmifatb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2asdaypdm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2bqjmqnev.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qbtjsnks.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ztgzcdmy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2inxtvbrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmalvsbj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wyrgcete.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxzlmfdj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tplwejoa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jjgfzbxf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmzbxqwd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2arehedxi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwybysvk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbluntyp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xwjgayxt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pqaurwtu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2stmafzcl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2loyyombv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2olftcllt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ekzimbtd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2loqqljta.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxemthfc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2magwgneo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2bbbicppe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2mvanhsqr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlueqnop.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2aduahwou.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ipxpqyms.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sggrynkv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bbdqaoao.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eteohgav.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rnzsphpu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ghvgsekp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qxtljexr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2otqbpvoz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2tudsmnzc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kudlibpj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mzsvynmd.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2szldhhqw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fexcoujz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cfjxzuaf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2trqzpwwp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ixysnjfi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ojtryfcc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2mcmlnlbn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kzfjloii.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2zunkougj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2flzikrga.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ojnlpclo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2xhsqjnru.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ctwqlozd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2tpsdsoty.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wllfjvcl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2prqfbaam.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2zmaksxtp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pouztjcx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2yuapufbg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xbeapblb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2tywdjdnh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2tatexlha.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vhswmbtr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2njokvgaq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xfptidzk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2rmfnfbzw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ilqsevnd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2phtgudkb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bhunwqrw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nmmnolbl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hbkxtjub.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ferzjbhq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wivpnnvy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nynchyqc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2umormjny.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dwkeakfl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2gunkxryc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lgsvvuqx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ydzwslqc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2leihwtna.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bebtaqbe.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jrwrqvsf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xjffucuq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2japsdnrl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fzoyexwq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2bgblleke.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2dxiycfdr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2yxbfjdab.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uvwsuqlo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2dxnwxwjm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2mtvzogiv.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2gfskhchc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2cjnwfhuv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2daqtfeex.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ksmfhnls.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uwbjdnit.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fbmpphor.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2awygaorg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qryzlsgb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2psskadjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnfrogbi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2dizngzjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iohimuaf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ddegixob.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2czjudmrx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ajgchuqg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2aywsvdbj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpojhegb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2vvcgkluv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2axnfwise.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tcholeky.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2urowkida.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2vykzehko.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dccgyoby.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2xrdkurfx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2broyycmu.html


<!-- 参考信息 -->