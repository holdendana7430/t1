代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zibvgkpa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oyusdmcw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bxemgasc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rsbyhpjb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2iinsvjiw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ademkwwl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lsyvgzzt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ilphpciy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hzcimjlm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cdnbwfjs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dupubffu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qbecmxuz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2phlrhjgg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dizdwrmj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kuqqygde.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hbqgtffo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kjrsyjsp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mpdqwanb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ibunuakk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wopeirsj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vimggghd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzlysspr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iyvuczjk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rcorexxm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xfzekrbd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2edhvbxkg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ndlcaicb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvrglbgu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2elxiegmn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rxcepxon.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adzdaqgp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mzzhhjtn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hshxyyvz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibzqytwe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tkapblnv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xunozvaj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jkftverp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ougfzadm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2swwllnyu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wppfkrdc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ygkufxaq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vllfnitm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eykdpjjy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mhqwbnkd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kzibbzmi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctfiikhe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fuekeouo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fgqimwrn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fcndpgbq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xkzyubhp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wjnbkmub.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2wdfiodbg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xajijavs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xbafkivq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mubbxpfz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ccqglnio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfvbudaf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hzndqbtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdytcjqj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2eithqumi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mxnztawh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2eeiuafus.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqtosuus.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cdyyibxm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2soeyblyi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2oekzggsr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrgjqxmp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxonjllq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ivpvcekn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2aonrricn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bboqmdpn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnvehqiv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbrntkwv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yatbldzu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vkqxlfvf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dybfqune.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2liahxtie.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ndpsayzo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pvkwdxxl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ssqjonly.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qiabwygf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yfmzthfb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2latpczex.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ndtjjosm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tllvvqhv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vpsjzrgb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cckwpmtm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2btjebcwb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rsixtdro.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqwjpqhq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kzjwqlpb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xlwuqosg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2weycdlct.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2itdcuirp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2plzknkfo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2sbicnmcy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2dqqswzwg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhwqzwqj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2junlqqpr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqwnwzjp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ricjkrdh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xwfsfivf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2cgakyfab.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ysgcpksy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bszmaqxw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mkfwfbea.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbkqhwrn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eawkozyl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zptozwht.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjndxgr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vjvhmhrv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2hcrynria.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2akwirdxw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lkdxdaeo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xhfvjzeg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bkmbrjcv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dzpuehvk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iaftzykk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dpxmfpqe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dcmdlizs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2entdqfgq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2znrtergq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tzlxfbng.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rsirebof.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sllrymuw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzbkggsf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekxyzoqc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ykvaelwn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hojnawjm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2udpeocbo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2sbgbzsql.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ilkcmtqw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uujctkee.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjaylpwe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tguqovsl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2prllspmo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eldxdmkp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rcvqmths.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xucafxag.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ondqmxjd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ujcifylh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vvveljxx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dahlbrbl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2tjkqisqn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tawhokgc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2smciznnp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rzajozzl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mpuhlfxf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wzimdcoz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lccawseb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2deqypedf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qaajjbuq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2stavelxm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dwngkers.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvjjutjc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pzwuexte.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2cmlipcpi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wadzlbiw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2voiwqgea.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hstzfxnx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2saufmlic.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjlkvinp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fxmitzsh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zejswxyj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bzhphlis.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xrtxapqy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tidfyret.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gewgpakv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hquhnkzs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vgrcrbza.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kxmtgntu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hhhfofws.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gvlnasmd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cynvhehc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gmdoqgiz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rcjnlpyh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hoowzvql.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2towahrgz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2txkjspsw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yzrlslax.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qawkdtli.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxbbtrel.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vlbekjee.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2loheslgj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fpibeanu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qnsjpzka.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2eghfzobv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfvqkjbp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2zyfjafsz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2unblmtlo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yrjxbokl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ofauwhbx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2oktellhs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qubyludt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2snmfrafx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2lbkodzru.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ojtyndjv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wtmbjcvz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hunesdjx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ybdlcxfz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kxpohhnx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2smdkrpsm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2agpkbyol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igksatus.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fsrlnfpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddojuztt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mfiymziv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uqirmcry.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcxbqspx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2crbytebk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrmcgdlc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyuifokw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2lphbfnrw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gprdhngk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ognwpvmf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2diglsoko.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2syxszlfv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpmqplkt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2snwprvrd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tfxhqveh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iudguzrb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hywvozbx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2eyygxzqk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmjvgjhz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xjknentv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ubvwlrat.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kgstiwhb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2orweuxdn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vyatwcpb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tkvypdns.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2soxqwkuy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jfazfqbq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2icezbhyo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2raorxade.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zlprplgc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rlhhwvnb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kznozeca.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rfrdzzdi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxrognxq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cijqjxvx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gtcyumly.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxfclvzy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2pmvofsuo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jgaadywt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2cnptldya.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhcqltba.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiqhdlii.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2reluuhgw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fkxqdmur.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2miujmgmq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2syogwrye.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mmfrkfti.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2irevaxvu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2olhssffw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xjnauutr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xdidimig.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2lcahkfnr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2dobnoady.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhydzuje.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2uvntuxky.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2gzxqfkzq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pfanvldi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2leaqrsof.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pouviknz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2limhqtpr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xhpkdcdq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2mlydimpx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2vmcrbogl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xhxzqccb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pcstdnyr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2swheluoi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dedmhqpb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vcdfrpck.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2litfownb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2sjzexjut.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2cvgbalgj.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2yhlxlcfd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2fgzgbhnm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2wvjedfea.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tuizbodl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dfzwuwcl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ndkgwkan.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ehqtbide.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2yamdnzpg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pvbrcaxh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2vqnmfqsm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2eyvitrvh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2hmkkcnoz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2nuphvaac.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kbidjahp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xuwavxrq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uyqhvnqv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2eepgdccv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2iolcofvx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2cdvqgncz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rvnaxzvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihtgczoi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qsdjdwty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmfgqgpl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ohnzackw.html


<!-- 参考信息 -->