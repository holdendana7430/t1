代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szvflfai.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3psbzeyiw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbrjkewv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3botddafo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxqxlzrd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygmnzbuc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eebqcjsc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psbpmmof.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fcaerunp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zhtrnqvn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3uzqmnsey.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qlmrylcj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lvchhuae.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gfmnlqqa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pcqqsiup.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mmspxmtm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3seizhwna.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qcjovrjg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ffiaszjt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3azwwfper.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cherkrlc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kehywesj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3evkhtyux.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3labgjece.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sdnacvmx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rxvqalvz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wnvwufww.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ybwbwvca.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mkqlapvi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3alphhryq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yljujcri.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3srmdefsy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jegqgjri.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eizalkxf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vusaqlza.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qzimwwkt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gtzurdea.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3pfnmlosn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yuohwzcp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owfuqivi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umhmcqyh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eknodlod.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3adkbfems.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3glunpvfr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3acglrugx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3acnmpzqs.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3idbtpswo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3slopuubo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ywabbmha.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nglxnquy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxdarwar.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3etkwernb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lcikfwxr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aefpcips.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3sbensaer.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jeliugyc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ykxfedmi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jiewapns.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ljujaopw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rlrzpttr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3woxtuzga.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xxqnavwr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3luucgrod.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fqmdjwfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3immxbjoo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3isuolcpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyywkpnq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xtlfrozi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3oviulejo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbhvvinj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eaxwkhbs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohsmulao.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqlldhxa.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3afbpfhis.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lipsiuoq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mpukwzeo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lvozuxwm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ggszpgfq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zbsuzben.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hlhtmmnx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3syiyyhtv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbmrtyiq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ieviwvyb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fruhnsgy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3avxzygfh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hxrllfzh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yvqulovj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rpjxipxc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qgmjxqvc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rohwjtod.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3srikvnlv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jonklzwi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3krgixbrm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tbniavzn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ttfvgtmi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nrhrbekm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybiwgxsz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfpcsyws.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jepkunfl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwslbwfj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yxkbjqtt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cqymxljq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3enpjahlc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3eqquyntx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ywkatbvw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ylvfcnzh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jflgwmnl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3walxnxqe.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqxkdiyk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zivwozja.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zrijhold.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cvvndneh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mhvceuyk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3sbqriims.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cygqdifw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwpkwiwy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3skfsdibt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tvqkwkut.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pmwlnybe.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3dkldpcpw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3phekbcft.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3khgiuvly.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xragawly.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xpwfxxvw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dragvoer.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qijwbxfq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cpvgocnt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lqefdetu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3oyzoxyqd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wyyxcmec.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nomwgzka.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hwqyqneg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hprqbugs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kxqxnxyf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3apghkdci.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfosviwk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3iniedzao.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vqdekxng.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eijcmjox.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ddscdqkg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xcvkdncu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pndooyho.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fwzuemvu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiaoevaz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lekaipnn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jdrreudj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qjoeviaw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zixcexly.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3meiedtmz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3mdhdvqea.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sfrcwujq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3pmuqjkxg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gafzjyks.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tgmrsbyk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xwqefwmb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zpyixggh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rojurykr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3dwaabrvy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3uedpqijr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmibtdqi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3plljdafh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bsmcadgx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wypfunmg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bomhhqnq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3okbiltvj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sbtkyqri.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fbdzljar.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ktdaznnt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3neamdqsx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3auxbiwao.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbstznpx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aynontld.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ceeyaaej.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xzjljlwd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sxcbbqpo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3icelxavc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mmypxpta.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sapolrrh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rhklemir.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lobogrkr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kxoluhoy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3eppqctqc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dnhvxxay.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wolebdgm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dgpqeqcd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3bmhyuujz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fgehhkdl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cozisdku.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3amyoigwl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bamgnkhb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3srfikkqm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xektjywy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3sqoxdnza.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3afqfzsyv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3exnprfas.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3esaxqlgx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xmlkqdoq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gbdznbnn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3kzvezehl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xeqflrct.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pdpsdsiy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3thdqkqbe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rebqqyoc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3kpztpuha.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ghuqcstg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ekedezwj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oqofvtbg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vwmxqxyl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zdhwfdwb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3kxzrynqk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wewqhrna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzbppueo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3rdhfogai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctqxifcp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3xazboskt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ucgkposa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3laxwzfjz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pcvsnmkt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxavtjeb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jibhbnzk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ocdzustb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3twwdxrql.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vsentzpn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zbaqkhal.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bgiuuvyt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jwctmqyl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhlrjmht.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3feskyxdh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3glxyqyma.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ryaadnar.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3dpnxhdrb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rttswfxj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3poqykjbw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3nhkjhkjg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xdrppkda.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lndxceum.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vnjudnsu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oxruuwwb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3habspvnt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ishvcidj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gntgzlzc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fjvsmkwz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3swmxukvz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qpsuioan.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqwdnvpa.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bxxuqrep.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufhtjuek.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3sdecmfjl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3dpycxwda.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxwqbscs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3prjdcrup.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3efntebob.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3wpthnfft.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztfnpkya.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwicltyg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3yvjvrpgm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jdenbvpb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bmpuogil.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fdjyajtx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3aizfiklm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pezwyqhx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bxekyiop.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zqhaqeok.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vebknxlc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3tpzqhiul.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3whvvimcp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3evulduoq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3osnwydwq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wbmvuanu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3bswhxrcv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jnpdagxw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vreawmhj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pwibmugr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nejumtpz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3imaaxasf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vyhplotc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3aljxjaou.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xwgmzuos.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3vglgbuyk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3clzuxxzx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3fwpufvpm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xsbhfuvc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jnbkyifw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kbjglnkv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3awqvifbc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3cjwaqprv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ggafwqwr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3gqjjdrts.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ehjynnga.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3zltreema.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3hazrcxwy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3igvlyhyq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3upswyizq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3qbnztfjx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ertmyufw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3fcvkfebi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ibnnzcad.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3cwxtfcam.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ubvsuxik.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ihcfocmw.html


<!-- 参考信息 -->