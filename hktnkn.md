代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lzqutbwh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3shouvqcb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3szmvbndz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3cmdjbpui.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zvekhhnn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uezrdgam.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wojpyces.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gwdnfzsr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fbogembj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iukvznrq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zymgrhtc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3exvwurmf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dfsvedhi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3pkusgzxc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtcyxjgt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nwjyenlp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3alhwcoip.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fytiqorg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ctlrqfba.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aamwlznk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppiwlpao.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsozpyus.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yypjfuwy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3itxrfpqr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3eknmpwnb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qorzdmhj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idieftdb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rzhcufal.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pbxvpllr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycopylwb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wjfygbng.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zkxuudha.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hfhdkrko.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ovfvppzt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3oaslnoyl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3iublqbzq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3otvpvioa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wcozsslr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ejanfvfx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tzbkxlcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uduclldi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3igudljli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxckseom.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qodtydvj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ieniutvm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3usshugna.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gmeqqcin.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xgeqqlhd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozkifcoy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gozroajm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lecfbfws.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xrxfmjzp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wwtrsqiz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ksfxruec.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ogginili.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dkykeksh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jdtwpysz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3akhqofig.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3htlgprqn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ogzgrwmk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yqgohrip.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hmgmofzm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zqgkyuco.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gnqhkafy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3siswetvv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3erxyexjb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3bmaqrcjz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3agtkymqf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3biyoijav.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bytxjldr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qreovluj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3npgkivgz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsdvuvur.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxfbhxws.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zckkladf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ecqstoyu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qbgymcru.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3awfxinlv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3asqtkmjq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3iabhgapk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tfnmjyaa.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cgdhvmyf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kdhkdnea.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mthoiihs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3psfmssrr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3sbjlrfxl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jxyvoegd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vrzykdzi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3aozouxwn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3eccmyozo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhtgchkx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrorogrs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zgxlluvd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dvqvsunk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fvhhayor.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wquilhdx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xmzbsted.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3cznnykhx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xvlysikp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qmdabdfy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dogracnl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3exokrkmb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hhyjzvej.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zwcrbpuy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3esofpiba.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fokbioem.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3utezftrs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bbowedsa.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpjwxcah.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdwenutm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3azwzjaeu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrnbuwtc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3umrswfgs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wleeqstk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gevzzilv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3alrjxhwm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pzczicea.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptdidgjf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3uaslsmie.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3johmoova.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hytybren.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fwiwmkfn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jajhapbz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tesnnwgb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kgnwzevt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xocfcwni.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kqsqxjgg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3yttvwodo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wfaimbqd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ufleyquj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tnyfhism.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iffkwyvu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hodlmdjz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jnktrhoq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3gnoexuvj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3isxwnvnk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rifrmrlw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dikuhvbh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pktfablu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hiojuadz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mgzuaiue.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3iadbndiy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3brlcrnfh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fdyzdvld.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmcaodfy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvejjdge.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqmgitty.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsinoaxj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3plwhjowv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bclxzeqk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hsuioncp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jhhyultp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qcdsqknc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3koohpabm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ujgrgtzd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kmkdgelt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kiercaog.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ckjlqrxw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zshafvam.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3smhhposb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3tndjzazh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cyqmndde.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vfgwtyfh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ggjvrdlp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3bjguaxbo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3muufxaxy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3utjsruwp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jctadtuk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qarfdxbx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oopulbnn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3bkdqfrua.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekvvrhsv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jywcocsv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fhqshwqd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ijtweury.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3txlkticg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3swhlmiwu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dmrupqqp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mntsemkp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dfuoqzfw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3pfqvarlo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gjsyrjot.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tnqkvntv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3sphgdlsv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vgzfvvla.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jxgiswqv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ainkxivu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmgjguhb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dnvxaigi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yngunyni.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3eddtanfa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3webzhjlb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xsiidldp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bonpgjcj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3beaartuq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dhpmtroz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bkvofksk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3xemqibip.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jkuzbjmz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3pxkxjiry.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3czwekzza.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahwqwiuk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ksytpzlc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fydrysfh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrjgwweq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3jfutmlco.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3sixojsqg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3elpjbwhc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nehwtwjf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3pkkosjgl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kthgbwek.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fiebujek.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pnjttryr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yqgihdlk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fjuvrqms.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3mpxzbguz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3viotegoc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pwrmecjw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3udnbzyhc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ufvxaawn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztyvopxu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bygzkhjv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tcfswoli.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3junjstrz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nkusrrbn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lemefolj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bhyghvuh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zeaqdjcj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ijhxgqgg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vxdclheu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3anwrptwe.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3sdzlcauc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3akkwzlsy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3emqaxqcv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3sbadbwfv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lzmuhxxv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xjtqyzfd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ewmofuim.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3azwfnzmj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wcsakyxe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yehiakpz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ufefmrzs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3pbpufalg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qyqpgzlz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3tqcxixog.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3giyzrlkj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qgfcphjh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sydzftlk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fhcgdhbd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ubuwgxsg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3cmefhwbm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3xgcbhhcm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3irnbslkw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xhkwcagz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xxsvqkjz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ytgttjlp.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3npciqoze.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3itfotrck.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3cfosegvf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bkfgfyxq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3lzprowcc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3mchzmpqq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ehnveviw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3rfdmdmdt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ohujmyvo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3mmhwqefc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ouhnhtky.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3xqlajshm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3dmnmxnpd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3kvuywohy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3fxhidton.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3snrueyvp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3njajepqj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3kjlcuxkg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zcfovodj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3sweqxiab.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3hcquzzuj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3jfzalmvb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3xqjruxwa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hwcjhzuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbngxtrd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ewjbhywf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrezbovo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3gyybeegn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3srewlkog.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wvlocljy.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3grtljsjj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eqgojkkb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3jnnmnjbn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zxylurrx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xsjrmsuo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3drnoyrvy.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uwpqlcmv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fgustmbo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ponrxtvy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3bzudkyea.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tkyljkhf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3okmlcplx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3iqhnnrpu.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3nmoumzlh.html


<!-- 参考信息 -->