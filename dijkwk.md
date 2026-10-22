代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxudiuv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2oxwnjakh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mpoillfr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lmdnakyr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2virffnef.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ayggdwbv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2iaspoanh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2scftgcsk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kjeboeio.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wuwyrswh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fxdooezo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2anlelaey.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2iqleqags.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddhugcto.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2klxoyofi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pezdnvng.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jwzedoko.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ccbbmsrf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2xrfmukoa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkndgwfj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kgdeaoyl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fcahmgyu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfahbctc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hvglgykw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zeccyesq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwwlyojp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pozsbtgm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyqvemfz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gtuxhylf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnrsaman.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2itdbfygy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2etlceofy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rqjzwefi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhisjkkc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpdtpcqc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ohitvlue.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2synczaai.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zktburmf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2bhdhyztn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nfthndor.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2khzmukvt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2objmolxx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pciamxto.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jjqzwdja.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fqiuzyrv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2puymwbgg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ueqnrmjh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mjpnwrat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfgilhks.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tndtvskp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2leaezzmp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ffwnidpb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2fgeqjyai.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xluhakxt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehyhsptl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tqakidpr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pgvfvdxh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2erixzafz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dojycvgp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dvxwwytx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhybgbdy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qjhtszeg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiciwiqn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sgxpqhdh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2smquidxa.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2thvpnpyh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2cpxilqaz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hvkoqesm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogapgnqv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ycdkycwu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2shiydmzv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zzowptmp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jvwvebtd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xqhfckwv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tzbfhvkj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jxmamvxu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ljotdmmj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oihjehve.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2flwxemmo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wsakuoda.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcteppqo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dncmwsvw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uunsduec.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umsulthb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xicxeoiu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pnoacsty.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nymhzxmr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2evvljrzu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rvytwwai.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cezdojtg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvxjlpdx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dpopdqzn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wueiyjkz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hmbupvwa.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2muwskvyq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lcdeateb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2galkrslw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xghzuxjt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nndxwdbj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibqwkish.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2meyvrgou.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zmereqvo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wxfbxlei.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2hloicdxo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hhcbrrfk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2yxrrpstd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2yibdpxre.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gftsqzpl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rqavfjfj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hdzuhtfy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zelbqkiu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kzmavlje.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2pmecemxz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qyabbtpy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2muluksfr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xrvtgfns.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2iualswav.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kepeowjd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uvfalgxk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gccfcsyr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ueyhgtix.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jbukoajp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dvldqhxa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2nsmuwzce.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ofbykdrd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrhzuqjz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kckjlzcf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2upccbews.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbaynmcc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwmbqgk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ldgisrgp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2khqbuovx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2edhwbywg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mlhmojgw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wytnmfpu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hoeonruz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qxyzaywu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ibfnvywm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ofzcnpkv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nempckvl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wgdxnujy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qvvyhnpc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2awbnawhw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsrqalau.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlktvoxp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tjovxjuw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gcrkkgst.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vkqwkpcq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fsiftcak.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ismhsint.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hhxjiesk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cgxvgczd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2llujbfkp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdfbzckf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmbbnsar.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2asbbkywe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gqvevjxm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2arvvuuas.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lalmcocw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2awzyeppz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jpkitviz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ssfayqrj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2spfgdaqn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rgvxinra.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xzjcpvsb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xpfsiiae.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2yvqrrwye.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lthpftuh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2itlwjdng.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hvcsajed.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wmdlpofu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kfnwvsvb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nktplbbo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2pexsqeno.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2euphaviy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nsuurtov.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vreutsls.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sveuvrdk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tnctmfqy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2mbrcdxbc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pnhepsbe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gyxblapl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ztyxrtvc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2lvcligpx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ttekjnox.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nrhcowjz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ypovpuii.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2kwamzroi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ktkzwrck.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xcinvkib.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kmsdsffg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wambylru.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2iqbczhyu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2vqavzjwy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2avcsmhjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgrkglkh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zvffwung.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycvzirgy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2bnzclkof.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pigjfdav.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjdywwau.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfsarzzp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2afpisggf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsdexfxb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jgqikwud.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2mrzmmtob.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2dijoymgz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2fhrsvcvf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fdouiqio.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2obvoymkz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qwzqnowy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fehjgzoa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vibsghfc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lhleyawi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2gkphpxly.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmkenxor.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jgbckmwq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bgoalpsc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ahoiidyq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yicwffaz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qlkdfoll.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ayujyaox.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2peemehew.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2yrbzykex.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bqfxnqis.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2oluqysyt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2umlsupaq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zqjrfnax.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ydijtgsf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nzvtrzmy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2resxlmbi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2yizrpfac.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ogtkxhmc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwtdsqra.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mwdxlyqr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xfbexvkt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zavgnree.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hnhvrkrh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sodtgbqs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpeisdsx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2aomvoscj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2iftdiiqj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhmnnvra.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2luxuuzlz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dpjiphlm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ulqhxuoh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2eubvhjdl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2paizfjvk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2xmmkqcks.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2tpoqxxcp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ryaimnwm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mzsmkeef.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2zidjxsii.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2alwfoipt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nvognjpy.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fpvzaqgy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tncyqyyc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ofbbyhdw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zrytxarr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xsnaqdbn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wawugomd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2torjybhl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hbzdyyac.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2cmphyrah.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ykujwyaw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uzainojt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gjzjipuj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2lmzqwtbc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2bxyuxvso.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2bkwaoftt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2gitrufvz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2xmjrjcwy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ebtwrkmn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xmdsvmkx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dluxnzwb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojiacjqa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vzdcqopt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2suiqionn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vcotyvbm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zgaipbyy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ssabykdk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ddsibgqx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ouosehvh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yqqpnxwl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2cbaetyqg.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wnxdkxgp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2oivobruu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rvuxatvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqktpenx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2zlukajbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugddgytv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vkomzcqr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nusqizlm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hbsctoub.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2pwztszfc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2uhczzzby.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2dftajlmg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfkvluwv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2voyvwdrf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rjmarhaj.html


<!-- 参考信息 -->