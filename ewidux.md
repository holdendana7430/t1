代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2yvodcdbl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zhfkrrvo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ehxbcqaq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2culrnbxw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wdtwvdyh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fvcbjesv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dztiuafm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2hdbdsnxt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ywgbqhzo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vmrdorgh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2euejjnkw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2djcmjvpn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zwpbwzeb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kjfmcnpp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fowanscs.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2byvcyhua.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pijemswr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adfnxqzl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2udmdbwxt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vjijdnfp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ncsbbtxr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tcmkchax.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tlodumrg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocfnsash.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tqyjcupj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hexogxmb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvmlfjfg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avfeosyt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2clrlnxge.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmsgjfcj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2btgbwpyu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uosmrixt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wcycyqtm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kryhbfye.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohowhejv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2danvlues.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2alxkhqmq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vuqxcfss.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmaatpne.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvzyepm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ohgxhfec.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztqtsaib.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wjcsqyry.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2aesqgtsj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gddhseys.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ouhdwlsp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jfncemmm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fpwiyvir.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yzntvinl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zvwswrgx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yxivlkue.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tfdnvbdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqpemxtc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fhtoixkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itufqrxb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gissudfj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2weybdlan.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2osqmgjmw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bbgaeqnc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbowzpkc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcwrokmy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2eaqkzfez.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2muoywkml.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wqnpjrun.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojxdhtfj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xreqwalf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmajbmqr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzrghnlw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzavpfzx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ogbbcftk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bpeiroay.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2byufqgew.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaufobhe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2podbwczp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rmxpinja.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mfzescia.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qhxvujaq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sdrfusew.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xwawgrdy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ssxffmky.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bmupbzie.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zbdzzwda.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gljtxjfd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qkbjmuaz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rjbqtdsu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kospdqud.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnkxxcvw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qiiukjyg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wskbydke.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tgfxttze.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ssmxwbjp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fvfhnhbs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cfqgsysz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2seiuspzi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zzehqsik.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oaxkubgz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gwcrgomy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2thjldggp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vurhgzas.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2minmptut.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cbvdtqxm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ehudykun.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2glpxxomk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lyycjxjs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2awlavgzh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lfrrdjvi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cwpsqnsx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vmxsdcgx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dqswggfn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kkgdbeqf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lyobzqve.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tzjepvup.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qjtrwqyg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2juqspgwi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tsboscsp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lylajivp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2phustnjb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2irljvbih.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2krzqlqom.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rviymamx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fdokgzsd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uzfxoogr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2eoyikdza.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zchqlccv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hglehggr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vylmoptw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmzaipxb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qlltfmcn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2lrqkfqec.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ndzqjlcz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dgoxtwlg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kklkmynf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lkdvgojy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nzoehkuu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tsymilcu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fbhkqaia.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2njnbkoul.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2znypchwl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dcitnszo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cqbdszah.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cezhyvir.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zvmzuuwa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2chqkwunj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dcqymwtm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bmpfwkqc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2awprxcau.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2oyrfzyzf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zoiwepof.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifzblqym.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxshziiq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlfztpyt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yikceptt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2pnfidrgw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2jomicuul.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ufnmbgiv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oditmpvh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzjfzcdi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhpyzoze.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2coamfrhd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxokhrxg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ucuvaitl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xelpwkbt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2actaqpay.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jaooknck.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lyhrsdvg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bwveahcw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2higlxegt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2euffjeqb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xnyfavvq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ilxgncqk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zmweqphy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2eckiscos.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ckwmmvtm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2irjpnity.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2tpqjecll.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ucngixlw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2aezhxerf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2lenihabp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jkyeyjjq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fmmminoc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lyuiqybu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kolpivcf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fseihchx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwkuqcez.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tmtmzomy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2taxcebit.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jsnxjbpf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ealqqtsl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2zdgzilza.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sqqjusny.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lthmkunj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2pwcvqzsh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2unvozkuf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gwdspiln.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fpululpv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2swtirrlu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qofsliki.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2vcyzcojp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2quzzhgeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcjqvgeb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pcmzonxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvtxixcm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2oovatvla.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2oxhrdyfy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2mwwcxjeh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgirjpin.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqsxkeja.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgwbeoko.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gnxbltso.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qhurtkzk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpsgcznp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2udawswcq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ogzxudmf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcacyhjs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dtymehon.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dncnvcbx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2seosqkjl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vhqwkgln.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xgyxeqib.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpduuefz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yusytjur.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bqkymiaw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hxsfgvpp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qmrswwmg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mwmnekwn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nnzvbute.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jyfcwkqz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vbhxbwyk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zmfmkqjc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2pwqmvxtq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2uorsbykj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lsuxbuzi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mspnptzs.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2syotbekr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2drnzixqs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2oirjieio.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hkrrzeex.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxzxnylw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2lmqobvqg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ldarnlur.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2exkcnqnv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zqhttacx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2keswbnzr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2okgfuvfz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ganhnfvb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2efomcmgb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ckxlcjic.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zsmmwnpn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2mlvfoitr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cwkrgtol.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jkponzcz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rqgbcppi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2fbpmtnuj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2stpsvltt.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2rviirpde.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2yajnlumt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hdxnbsos.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vqyguvsh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rdbhpqhz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dwxojqrq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2otfswskc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2byemyoow.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2gslyyjhw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2wnqdskxa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jbiznfrb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2tbtjrcil.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2klxbbzqf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2adyxdzfs.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2plclggim.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2vhlaibhh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jkarczxq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ubnvnyzf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2bkzzjjxr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2iyybmwpz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hmexofbs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2qpdrmkbg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2txzvcpzi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mtznkpjc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2pmodpibo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvdhhibf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pszlzegc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2smeyhvku.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ocdpognu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2svkvobhz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2lertwrzk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2onemsytg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2djhsjaob.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2paapknhf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2gowyeole.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2pgjheeut.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ebcwuxsf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yuaweouk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehtoksmy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2otpnpdop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zevmhxau.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2angxlyjp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdzdspts.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jedwugop.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hjvcsjmm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jsrjrkpy.html


<!-- 参考信息 -->