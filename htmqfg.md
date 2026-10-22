代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zabvlvwb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gyekrkoo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ifuaajes.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iemnmsys.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2meqzjyhx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ketdgzie.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xtyxeuhi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2znffujnt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnmpdwaz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojirmcnp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2edzblxol.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcakoeer.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zuixecva.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lvymrmdj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ttwvryqq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jfulyidl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nozxwjcj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yhkqsjei.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2idipyxfs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2umxhvwsa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2slhhjdxc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mjzpdixw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zktfxqhg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hnrlgisq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mjvimhhz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tbxrkoju.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dnnbmwfh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jirgqcey.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mahnvhhv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vhzsbuch.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xvhxclwv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zlgrxqkv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gzmrwpfw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oddcatya.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2prbaqqqk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pvqjrwsn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pnjgltji.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iihougcp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ycgmiths.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llbwntyv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2httoxhkg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2kxbjgdvu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zsbseiet.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kahydrif.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmvussek.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tcsafgpu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cbhuilxz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yausddjw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pktbsqbp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdcabmxz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2phbgcejx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsxsmqku.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jmlhkcoj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdnvdhch.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gpbnfxbx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2egnhgqah.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ucxttopq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcifhiel.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2oxrjrzvp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kbrrlccd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2sjmkicqk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qgqauvql.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fsphbgen.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2wcjvcdnd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lnpakboi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bvlvggml.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2adytsmcf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rxpqltjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljrjdcjk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wicztigr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdxmvmvd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2unvbpyrh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mroadvjd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wnqhpyad.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2etqxjklu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmvnjpsp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hlhtjwbv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vsszbeew.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dwkrbffl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ginzasdv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mrduxgqs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nztmtrvp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ixrqoteh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ormfobnz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfmfpqsf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rwlenzbg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ovmyinzu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ifktkuxd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znjrkvqr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mhximbel.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gcqynqwc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wtwcotpv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ypjuiioj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2uokrmiwh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dhbgklvo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ometycmn.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pceuouct.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kwgrayci.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2uukluzup.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bfpkeyza.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ezbthyxu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvirkjix.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bshtsiie.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojkajccl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nzxyxdxn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tfqsioxz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2llavmhnb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wpypldar.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nglycxyt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibnnanai.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2koeukrva.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2aibmklus.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jvvunfjq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2sftpytbx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2epxkecmg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljtlcoce.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mpitjibr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ixrtnxpe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2abkbtral.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2poczjfdd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kdofpqfa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixignsbc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zfaqwuxg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xpdoyrwo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ukvwrlxv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2oewzzfiw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wvozkdiv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kwqtresr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zijczvpp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ratntvke.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2erxqcoxl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dtxodlsk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xsderboq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2usgenvma.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2kixvcrfa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2phlamgop.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qbkniocu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxmjienu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qsgylzez.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lnfrtazt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2yhbxdacx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hweguykc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cwcraxfw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2csjtujol.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mfzliegb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkhhrjke.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qoarukxs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnxgyzfw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vxkyqnjv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ihzawcyy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vfoqeixm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rlavxtca.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jcczjffm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ljzgniqd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vqlxnmou.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2twtpmwbq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rxrhkdcs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pszhknia.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wcndffye.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mqnqnkne.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ifihofpp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hbjorhir.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jdojpoeu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jaigoeea.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fllnjmpf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2auukdcql.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pqzgnpxb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hzllqofd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gabbtoui.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2eejxtvae.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bakvueau.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ytaymumx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umqdqhos.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2blxhdyoz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2niedqxlq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2krhfirzs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vmplkkpt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ggmhwbuu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fpghpipp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hhhjnkai.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tuwygfxw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ycdpmmtx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fmjeiyhz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2syusagfi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bjoimope.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zohgtbif.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2webcdhgq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jfbosptt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hutpivcp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xtkqmpzo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ckogocyy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2fmkgwiir.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2axqtximo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wvrjydqa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qztrdxav.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vfikgxtr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2yddcsxkq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qwrgodbp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hivhcfbx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fccupoou.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2koovklxt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dmghjtzu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2guwdnoth.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2eltgokja.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2atauuvuo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kmhsqfpf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rjyqyjya.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vzhmhcte.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ivpezsny.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jecxfctr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2alsadphz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2kgsdeuvl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hghbvhnm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dtajenyr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2groepjwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yacualcv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2sxycrcsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umlxdslh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bbngiaxm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hojbfjqd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2pczjjgjz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fvjwpmpa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xlgevllu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkmpabpb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2hmqtzpql.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2rneigcjv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2pehpecbo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2yabzkmdk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2hrzjcxbg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zrjxqdtw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ttlkekik.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbdfeked.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjnebchg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nyblbcjw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hgpbjhlb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqjzfqry.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dswnqyga.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vssfdnxp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tvfkvpqw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2axhkyegp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mphdcxzf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bbudcqst.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ylowywmx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ejuqesqp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lylcrjzc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mlucwuyn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2guafwagq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lruoayny.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvsinmor.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfnmgpqn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xclssrag.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vzzfykcf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ihohnipp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2buzjbmsh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fvpywimi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hhodqmjr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2nowzpeie.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scifjfnl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bdipqfcl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2dkojiatd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2nyibizps.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ldjpltpq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rncfzgaa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2mkpyhcnh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mazakjio.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sihcukcb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xtfukdmj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vluqlbzk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rkteywuq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2fknmatvl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wbsvpezw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nnmcscpt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mxssexvt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gjitzoor.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eiviwxsh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2clsvlcxy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2koatnvgr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2oygmjlwl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lairxzvi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2emablqal.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2spgrnmeb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nfjkcbdr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2nxekdqgq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2bvpkktnt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2weqfoimd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bzmqduoy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2yjwcjjbn.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ukcuwnqj.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jvzxdxrl.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2fkkmbjkd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2brriveuj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2dwptdwhm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gavgduod.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jiztndms.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2dhsacgnd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2aymeacrv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ioviqqdh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2cugyafch.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xoiznqcx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2fojlacrq.html


<!-- 参考信息 -->