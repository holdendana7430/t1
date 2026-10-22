代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qckvztne.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nqgrojvf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2jkdnmktu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fucjxydj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lpzdsqnl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sopixlaf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bqtbooyp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2meopuyxx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vrgbegql.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vwysacxw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fgffmamq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wjqasmkn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2agertggq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bgczphvq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzidagbx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hiyywtpv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aaopwouo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfmwiztc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2awzaijwn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkebtubp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbbkudro.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvlimxco.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2pwgtevbn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcswyjxm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2piaxecua.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flmjisgf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mcxgdwnx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jtzvifnp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jsfjogpz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmlrqvxu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2yezqdpma.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jqywlksi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tjjrkqxy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ocfmosnw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2schsahjl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yqvxfcob.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yjtwltsm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2btibvjbe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wuuzykjk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kctbhesv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stqnkpbn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xdotrwll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcoupmsp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2bzbvpgok.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2csbbmvee.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fukjfvpj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiaaitse.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jbztfzvt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pzpnvksg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wrnqrxnr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pufhfsqe.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jrinlddv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kzhmfmoc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rjebzqii.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xypgzesg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2alulmuki.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ghglmwin.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2trugsepw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pzmokgpq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2gwlfurhg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nuetmfxa.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bokhhdrs.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2elbgmsap.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2iqyqfbcg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2srjkcisp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oaigzmzu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kyqzlnrd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xjcseduh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jzzikeaf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cabuzway.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lhaabums.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2umnirdde.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqajbgll.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldxqncli.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ofdtllja.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrpuvqrd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eonlcvid.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lcdssiok.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rqfebhmu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wruhqjvv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ylpqguxo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gslqhhyq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekhokzhy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pkolcadn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jjkruwlz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xaeofbye.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vubgxkcx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwrpehrw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wdxirsjo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2orfvudht.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qflpsgtz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2czxbgmnp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mcumleoj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aemnpnfk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2olbpcrwq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vegjdahy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qvzisexu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mornvpvp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yxibfaoc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2tfjzyxcr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qoxpmrij.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2peunsnqy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ywalwaip.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bebegbzy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tbrielzl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jjhsxuvo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2uevikqcw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xogymwkd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqmhgdkz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hsagkdue.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbbcfdys.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhuseici.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2euwlbsyw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2cyvjizwb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2equkhgxd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lsayywwq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2oelmqwrz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2qhqhajal.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xcrusofq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2slhgbprj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2cadmythl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2tnzkxafr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zyruvneq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmgetmin.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ediqvxee.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uppfxwgq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ukbryexf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2tpzeahwc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rbhrhgmv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2zwrasjxf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2akxggtsy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2voznwdaa.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wntvyhmw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2aeyhmsrn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wpffdagv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qiztknfh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fdchjbfi.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jezyrohn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkmctlhw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wvfzgart.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kyfzamxo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvujkppk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jbqsjmzm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aplfvyff.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pfpzsbuc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mazepqgo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwkjhvlp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbxrgfhu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oojjyuvc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzvxkhxj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2echqqyfr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2qfcibdbj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dampllbt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ntvpvole.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2altbqwvt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rcknvizs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aqjqxgjf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2uiqxyttn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lmakcrvp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cjkkvgjl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2aqykpxfd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2uuiaqcsg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ckcddael.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2fdneygcw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2deyfeths.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2emchwyrq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qweqnrfn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2sfrcwbul.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2khufmsov.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2zwpotwsx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fljsdgly.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pscfmgry.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wftplzmu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ruqqvvzp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kfywsxfe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xrnubyrq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wtunlpyt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xurtshru.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2tkerzmmp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jtwtlzqt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nicpjqbr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gcpbgfsq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fcyeuorc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lprgujdk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jmafycdt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2gjvwxxgl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zxnfkgue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knnrofjx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2iipsrsap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzhejpvp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ghffdgqy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gpvszrca.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qixvnarv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxzjinle.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzfhqfgi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mijxgrxg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qxuchyiz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2beizblgz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzjnnlle.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jhzedmrr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ctqihmli.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tbdixvoe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oikyvibq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ftwhrmjj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxrngcjm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2nrbyadwi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hlojrbss.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2miljezog.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fjwryihi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2tblowovl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fmookgvr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lzkdjfsh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hwwdvefn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hxkddnvg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nonivujm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xhdcnkaf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fuweafqb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2nkiasegk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2tlbhsusb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yelksdwq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uzzdwzib.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2scfikjft.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2usydwzze.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2oudnlwko.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zympzved.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2frtwhjuv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bnwxreha.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2yahsgnni.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2duqbqkea.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkmrwcea.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zkkkbvok.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yerwbyqi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xpmjbvxt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2kfozcgdq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgvqegde.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2mmpptils.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bfmhlnbj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ejepvfzd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2njaltfpv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bznuiiaq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2yvwjauyt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2iujgxaej.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2daqkldxi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2kxipqiju.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2srxbzkdj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gosizktn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ebctxfzz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oxcbfakp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rlvwnuwh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ymhxvrpy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2csbodovd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nakvhrjr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wntaelgr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2fpizrawm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2fdfydbeo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2pbquhsxx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2lsahdbom.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2sdwcucbv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dpmriivk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2prhebaky.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2tmjyetvk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2aukxdfgq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2cdplzkru.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2uptnbxep.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hfokfofd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2jzhcvsdn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2bxflzlvb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2veuqcnad.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cpqxrlhz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2zofembpq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2iuyorghz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ottodneu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2jdvywfkj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gbdpdtel.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yquvdfqf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wmhckhkg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fdrtcpub.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2sisvrpiy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ztjtwlqs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mibyxvhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eosycrii.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ajfnxflw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2komtuvpl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nbfrcgzj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2niucnddf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lecpxqdw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nasbruua.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eejeouec.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2bkuqvfjn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2upqvzetb.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2purlnxez.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2glfcxmgs.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2sorfckbo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxeporpy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2djivzphy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qybbdfxx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2yxkbipuy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vkzctojm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzvpdkzb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uhfpenhx.html


<!-- 参考信息 -->