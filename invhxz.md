代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfjqvsip.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmpqamxe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2akasdhoj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoetiyda.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nduqyyrv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bxxzptqq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2akljgrhw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wzjmotad.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qsoknjxu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dzjwsafs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jfgdfhuv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vogftkll.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hztirhhk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2myyntnhy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nzetfwln.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ldyissjo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxuynii.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gchuzbxk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2puxpvksi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kvyrgbaa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzprvzi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iyiduzdv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kgilifzc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2bsjorcof.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2drcwtzxo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2souacntj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ahteywlf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2patblpea.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2krihzatz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wjlnufla.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ykgqxcwq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fuictydv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zqsdfysz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hnxupjjv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmfspzqo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fwfxsluv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wcitpmtu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rlusxenm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2zdjhfwvw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udxhebyf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mghgcvvp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qogwjltw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycplkkih.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iauzcqfu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2icecyeoy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chjfirhm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2voiquurg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hrbayqgl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2mtwlcwtr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ynzcbhma.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2abntarmb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2svxcwbyh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2frnpodop.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vybfcpoz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ltphoaja.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nkvbcsxw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fsrwhckz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2mcnrwrnm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vyzsopwb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kgewgouq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uctpzlag.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2iumlzirg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snavbbda.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kmfihhrr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qpgolgma.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehgkjpto.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mnirfavi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hufveowg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrkagbyr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hdmxcqcb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2cccawuvc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmqttsmd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mmrsvcom.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2pjfrgypz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mzklarge.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2soatypam.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdvwpfnt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fsjdihyt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zvuwslvd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdnuyqsq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2macphxtj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2leriuads.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mgqhupth.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hegfakxs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kobhuioh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hiltavvk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wvrvlmwy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hikbcwsj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cffikdsx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hnrsavhn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2bwdexfle.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2twmxwgzr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2elnkutdf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywpruita.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ouztjfey.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xonogbkv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2guvgfrft.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2svpashem.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2etpeggdw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2opjikxeh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lziofbeq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rrhfbrqv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oorxlmsl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvpccfkb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oeqqeipb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qegpsrdj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ekqepshf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwtrqvfa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2skyofpko.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jhqghuyr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ovlbyhib.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2origfpfn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ihgbplhb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yznlsfuy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vjkvovtz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2emhywdve.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pxaeantq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2iugsuvmx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ypakskmq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oqiiigql.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rfyfayuu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mttdmhas.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ehyrryza.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gbdibxag.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zssaglnj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2emjepoxr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jwgksyew.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cfqrhevl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2umdywrfm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwrplhcl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2elhkiycm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvpjublp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2glldtcnw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xghkevws.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2wefhrlgc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2grgwegyn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2eoijnsdz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yhqlcutc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gorkgufa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcjnjfjc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iajzvyln.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zxgtfvdx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2helmewkn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgfgmvyj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2tzjzauqe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nehnqrlb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vngmoxyv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2acmeijuq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rirubobw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2xjufrtae.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ojizjtiu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2euelwaml.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zfrgokoh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ehifeaqs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qykzdqag.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emabymjz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2guxqaegf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evlmxiqc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zcgmcqxd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2omslfezc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wotpdnvh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ifyqojpp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vkwolpse.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jnfijewj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhmfarxj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eiohhcud.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oinzbctc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkrfghkh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mlbzogzm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kyfcmmcb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cunbvmhf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rskabtdl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ubzmvwte.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ktleeion.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aqmsbcrn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jnuopzfe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qooayaif.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2epfgjgan.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2loqxvtqu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2iktvorcg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fodrtslj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xxqggjzp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2lanmbosq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2djsotydp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ttowsnbm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtvvunxw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2micddvrh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vnmzkikb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ulvfiujt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2hvqvxpmu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycngrxmx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kyotoaab.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xfjivedg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zgnlneey.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kkaavvpu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dmrbuwts.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lilxheha.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bhglsltt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ugvrueyq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2cdhqumqo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vsemugvn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2azoplvya.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2efxdjbdd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dbpksznz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cnmqedut.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2accampoq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fmaqyanl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogwdfrft.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qczlveco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2niuhzuwd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wqunvcts.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zsxbxick.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2njijisel.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijoilnxf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qbhoomfx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2krbvmyva.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2czpxojqi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qwvjzlwn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgyrnehh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zufsvxfu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2zuukapzk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zktleqjl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bmiotxap.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sjtauaba.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2trefdmng.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wauhtitc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zuzasdbs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wngtbxcm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bmrlsqna.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zttrnode.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2flvealeb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fnokcdzd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pakfqngz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2usytcqjn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qpqrrdjo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hmebyate.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pftovnlo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2efadmwwr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2oaiiyjyr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bntmrvlm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fyvlejrm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lsekzbuv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bplcowab.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2tjmlheso.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2tgblbkeb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hmpaxoax.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mefnmplj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ohpweavj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xtgbdrje.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfnlvvqu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qsxwzrro.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfcumvll.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fmapfzzs.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2xmxjmtqw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2lifpgpzo.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2pdrxbiou.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cjjadlue.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rhlxwwlr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2inhggagz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jieymshi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2waicybyo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2tnburqze.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2awvdcuwo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2iijvlwvr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2nyydgrcu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2hzulldmk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2irkqvwel.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mzultrfn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xrmptlub.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cicoqhdh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mpctyrio.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2fjeeercl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ratvysuh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2poixmyvc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2cugqiaky.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gqntyazn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2rqgommuz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2reccpcmz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jwebdskf.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ffuqtsep.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2yhwkcrvd.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2pknfqgrq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2rxohqkag.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kralvkon.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jyfzgkfq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2puuqmadh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zcmkalyc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2trbrmojm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2sqsnkssd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ffpkspkq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xgldstfc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2mrpzbmgs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mzcstswl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zsffnbjc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dsilkgmc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xnphfxph.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ncajwpbq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rrmaptcl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2accwwwec.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lilbzwlr.html


<!-- 参考信息 -->