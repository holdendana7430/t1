代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3homlqpdq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pegifxqe.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vpwovztx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ubqldmxp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fsnlhqzb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hnengllo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3glwktcfj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qfbfqzzn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3oggvuvij.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3bsofumen.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3glojdnsl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ufripkrm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxvrhhk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3squzrwgo.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3damlcwyl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xssbhcza.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3icbbgkuk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mwbqdcgh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wwoulwjn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3uzqwmybo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3kpebnfxf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gugvvldx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3opyeagdg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zcknwrtl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zfxrllzv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zoertmqq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3pxojiuql.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztqirmtz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kxfegbdu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xqnlcuhr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajcrhihg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mxzjvlaa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsmzhqvc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kzbckqzn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3paebmclu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbwqbiyf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xbajelrl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpdrtmkt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnwoeurw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqklqccz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3czvmnohg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3awebuwec.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzdsmpln.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wjfqrlqh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ibunxwkt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odldhkwh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3aqoclxfm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fwfzqwso.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xfwspvff.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3umnngzdu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pwssuapw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3yftpzuex.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xtqjmqpq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jwmmmrdz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rcgpnokv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rbehsiio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izurvayp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3nsqjstnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktqotgic.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cqqivagg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fbeijwji.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cocukdqe.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ybiqwudn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3utrdrflz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyddvcdl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ouoxnzeq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3nvkcfbll.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nsvtpwwn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ucczklsn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3kyjbcvaq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3sqzspram.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgccdgyr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fajolqvw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpvhshlq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3bfoupxdx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zqjyvlsg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yytsgtca.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rqlzjrnf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zgzyzksi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ueyowhtz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mqztysvb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sglwjjhr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3kudyvhii.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zylnwihj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qbkxwbgl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jcgdesek.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3nosxmquz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sycishnm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3imghjpqm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmatzlbt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gevvrsom.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gykauykp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ozavitkf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3oyivqazt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wzfnvtcd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rbnirehg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rrtseszd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3amnpwhxq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dgulvkyz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbmbiwdd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcanytmt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ckkzkyam.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3uvjynfwu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nqkyzdjh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3titikwug.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3sritaenm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mgagcqpp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzoxukan.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hmcyoiwe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wabwnxoq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cvaphtgo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nlicknux.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3sqapyfiq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tyhazgnc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fabdkbcl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tpehkxps.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gvcsqyaj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3esrltowc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oddmdwkc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fsdowgot.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uunuifje.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3umwttwci.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jnkydlwy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hwzbywai.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmjouytu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkjwvecq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bksxhyep.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaqpsgir.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wcfzpuor.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ffzzpuup.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdjexbyw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3iglmtxdq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3hvughaou.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vddlujip.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xgjaulbk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vngyzfww.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nnhfwgnh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ybhouzqc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3afuvenaf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzuybfsf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3uudellps.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3obwyarop.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oksckwwa.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tfxytggt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3swtnqclg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3gvfnmecy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ybdpqswz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3imfqzrzr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3phmlwchd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jvtxfghk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3autwcmbn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiuneyoi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3frpobpnn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vzrsngkt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilumbjgm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ezyfnbcx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3onoiaurx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fojnctpd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vibjghsk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3adirvnih.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmmveujw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ctckwtxu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uewldedd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3daopyiqa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bfopdtka.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mlalreat.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kfxpsdic.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3vbcmlrts.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nyxxesyg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uacqbsmw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3elynuzjv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kabtdgtp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hkrebaxk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3rvnemsoa.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3nfqjgwzz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dnwrhoyw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vzxqomyo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qrzrthbl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ovnjvlgg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ydyvtfwr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3msbgunfe.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjqrtqcc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3owftsupe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3shdigqif.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3wxfzijso.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tmxmjeit.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3trysxnue.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkbzard.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vdqqkydw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sunpvedu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ryxrkkwe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nihptfol.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zcttzfyu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yyujoqky.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3tsmfomqq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3kygeidjq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3heqqnxmi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3iqmmkeqq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nhlsgrjr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cgxttuhm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3eswmfqia.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rudlknam.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xkytiuah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnqhmpsh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ucmczhxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cllhfsgy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3odzuoeik.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bxmuvopr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yedzzucl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sebjmpzq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjrrzzes.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kofijzoq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3dvlzujct.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3akmusfpx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wqhhpgic.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3phfdgerp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gqfkkgqq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3okooxnlv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vsoofttp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3insncdir.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tksuzxwv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ytueozbo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3aofbdjnt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3afyambyf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nbrnsbze.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ktgjldrm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nnagyppw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ywlcigxd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hkbcaplv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sgqcveln.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ufdwmhke.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3suuozbzf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rhuzdkye.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3dixzmkzc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ucfuzuro.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vnrsdszd.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssfmghjl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nuiutyis.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qwsaphst.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3huorukyp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rweqcqmj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekoetsrj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3tleocgel.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3jfoiusdg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3zgqffmat.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3epbnffsj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jbqjqqit.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3mkqgkxun.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3euydbvyb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3lrkhufsz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3gmdpdgcc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3whwxwvse.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3bfqzzuug.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ceserwbt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ibqvjrip.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zbzaggsp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3oklnkumk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qgxmlmzv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3weoxoenb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hvxmciqm.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3jshvtiya.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ucbfvkml.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3moantjca.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fdjgaeux.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lwfalvfc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3zbayenbf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3otanjicg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3efebptfy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vbwkgeda.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3pfcwiuui.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3oeuxrtgo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xpffnygj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gjdlhjrj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qedzrgav.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3emxqcmzu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lmwvowtn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hdldzzsm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dnjtxndv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3aiowbamq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3lonfiaxi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ttozilvs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xicssdxz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gptlbjtc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfnnbxzo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xnjxffxa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ivvkqsmx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3oncrmusz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ybwgqebe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xieuefyt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dezpffna.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ckhdultt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mnccweix.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3llmbcqzl.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3xcrgahga.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xtaomeli.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yvqalmld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbmxuvsf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ltjbiwno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsoeuyrg.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gjggskyr.html


<!-- 参考信息 -->