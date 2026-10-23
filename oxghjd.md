代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdmpdqix.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bhwesqtb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kfgfswtw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vrpurlbl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3zngrhtcf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hsynrpkq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zjzgevtv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lrltotpb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3tvnmvssa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ypkdkpfk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lixfbyup.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3agffpxhy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3imopwovk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fqkcdeqd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uemgnqft.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fmplkbcv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fxpogwqi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vueyidsb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ufkjwnia.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3twuvijda.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3kkhzskrg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sdiwxvci.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iywbykir.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ddmhonyn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jazmzvoq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ximsnezb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zzamctgl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wcdupgkc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wkxovsnj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3aormgnxq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbjtbpte.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wcddzcaq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qarrmjpe.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kivyuuzw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mfvjgbcc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhvllnqf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbdvwzyd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yscrnbwm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ifzmrwsc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbkwyanb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kcnwoscf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aucgoyip.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvgyebde.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3afneysmc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3orfkwsoh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qakchkin.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3tcwgudfx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ivegooos.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dtwhqgmh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ryewthpl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mnmuubgx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3euisiiqo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3bqqbvnbl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3eguphatg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rbfwqtre.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ligpntbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udxyalni.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xkdkbowa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcrgvwoi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lkyytyxq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fjkxcpqd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvczjyyv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yzsljrsb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3hplsucmk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3joindmuj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3mpujnefr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bvfjxbwo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dwtvoiss.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dvkdhbdv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jmfuifje.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpsjphoo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vpfqujau.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3pbzmsmwj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcbvkxlp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tbwqnvts.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jjesgfhn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edqhudzp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ztwwsatn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qrifisip.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3borarbyz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mxbiozye.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fgajdxps.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3igqeotcg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uqqhrxtb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uktixqik.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ueuefrlj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kybjapru.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vgmoecbp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qeysiyel.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbsuilmq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3culnqxfb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kqayfxjr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wamdlspn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aubwwpvj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cvzryvig.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3fffvttlb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jhktahal.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3emxibbea.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kmlokzby.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kceebvct.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gzfgvsud.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3iffjrzrh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jqgrrosq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbuecinj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3srvqkrll.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3untlxyti.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xblxuvxj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocmdpced.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzzwwwwl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkjnkpdu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hjhsftlr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3eqdrkcmz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zapmnhip.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nanididz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yjiheegr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xhlkjlbz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hpojnqpo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ffrgdmzr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3etrvdqar.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qsxeqpax.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3xmtyewbw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vlomyjii.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cstxuycd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rvmqqhrj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bipxbqur.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xekxcocf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3czxqqtpl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbdgqasf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ucppvhzc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dvykjueh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbxapbsc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ddylakng.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3lhujybdo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebpoaoyh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ejlwnbef.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocrxvnzm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzowdmnx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3uidrgklo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ilqvrbte.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcczrwkh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ijxzqgwc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nzlschru.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gtvmegyl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3quikbxau.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gcxlnbrw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hmxkcoqa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kebturji.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zvsvrfnh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3yfqtqstu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3mptvzryf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3tkirycbo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsljlkcm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ydoyxmun.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjlehppt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dxdphrvg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wqjbspkv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rvcocgvv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jusqhvvd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fhfywika.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rmxprvwt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymtmspbg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mizyznnp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fagudkrr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pntmjazo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qpjxkqfk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnwkmnrh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zwnfuqlz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jeehdiyv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kpdyfkgy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qyzbtrye.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yorzamnf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3daegjlea.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zgyhskyk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3fsgavudt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bfzwjwkt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jeawmfxi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zuqzpkjb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3dymzzncl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dotkkoti.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3uswfoczc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3eqrlufgf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3lxmogfjt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3tvzceicp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ppsnjvrj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ritpekzt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cbeymvog.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kmjbazdl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkkblsqq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ymodrijx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hduczcwu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ophzhiyw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vjgiamky.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ccejpjxd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mixrnhqs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3iknbsphe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qvlogrrt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wokhpggn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3plqhogtt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vwnsqwww.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3opnbymxw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bddghbop.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3legbjmje.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zrrcgtwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eotoogdr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ugtwdijr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3puluyjev.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pyjwnpca.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jwpareyx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3pktljdvx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cypratyi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tcvocyic.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xjxdlkye.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bvsawflz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qwxrjlso.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fvzgequt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3oxzrnjsn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3uovvikuh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqwxjbmv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xodxvnaw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fumypnjt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qcuktifz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jozbtora.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yvswjlyh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzlrdpcc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dihqvqke.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3zqcudgvg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3indwzjmb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kyhqfznt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lfsvjaag.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dbgvvjwc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3tjgajlwg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3teehutio.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mapencmz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3evumgjkx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3yrruirpv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jmppintw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lebvifal.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3smvpqmim.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lvdtlipj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3witfbrro.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ughpgaxw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xltflbwf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3kqgbjgap.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3rmpqemsp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3sdtdvtxr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cnxstpbi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyfdadox.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3yxnsvnub.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pncnskwl.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3avjcwngn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixzyzmdm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3orzqlnxe.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3hhxtjcjl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3saqahqif.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nskcstre.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3owmkgrss.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gzwlmtcf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mvsnijsq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3zpwougar.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3udfepfty.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3lkrgrtdk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3pqhdfxml.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gqgxothh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3knreqfyf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lffcyrvy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ajndtouy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3egzawyfb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3tmvnfleb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3brgegami.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3oubnglcp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cvgvmzay.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ymqznspv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3kmykqgst.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pjpjtddy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3vpeptfdz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lkbqnjyl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3mrbsvqrw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3illxanjl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3pzhbawhy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vqzebsgh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ggvkfywb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3bxgktzag.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3rcmrlkos.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3wtqrxypa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vkxzjdxt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3idklpirj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3saiajixh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3tneugeog.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3zaoobxen.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ayoztukx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lzmvlpgg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lathxlyd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3uofoyqib.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tvzappgf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3myjzblsd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jasdmbwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohiyoboy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fxetapxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enqcbwqd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gbprxino.html


<!-- 参考信息 -->