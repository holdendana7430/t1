代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fwydyqyc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ftbfewij.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uycgeumj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zmznxmcl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wmpjyzvj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pufvdhpg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qbozjvsh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bicfqmrm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bvxxjtjh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2asoekoxf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hovolldy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thyvwald.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ovfdxnll.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2svbtbewx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idvrfdua.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gnmlpetb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2keickftz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2puglubst.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2szjnmcas.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtmagtas.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejdgizmu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ziroeoom.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nmrffhia.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbrwipfs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xbflsmut.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwlmlupk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxdwxzrt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mgwtmscd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hjaryvan.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmtyzmgb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kslnyhxl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2sozqaign.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zusdgryg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vjclkhyd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nfwaltyy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fxazntls.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pchvdsmd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hephhkpv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dtrnbpjy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2xryixzxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjsayeif.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xgfkahri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pletzicl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vkeoksgu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2sfyqrqaj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewsyqlvn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xajxugah.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2sgggicpf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkujssdq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2seimztiq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rbiicnlv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ndktdjnx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ozuqzgrl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bdmbscfr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svtygwjj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpdafjsc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2muokfrxw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jxdijmku.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lhtalwwn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ucyvjwdg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2itjikjoh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2btdzljnd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2osdowtov.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dlfplgjf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bmezqpvg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2odvyzebu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ggffmdkm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zmyjrvjg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sljkgmbt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2idtujtas.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2aenwusji.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sxznnqri.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yqefhbcx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xsrqqgfr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2woluhaig.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwwvowuc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yiyzdxad.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nvgbayad.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ecasooid.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2aqxranix.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hnsmtpze.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojegffxu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmyuphog.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tmaeazgl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wufrzpqb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qsiubwqv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2daiczctr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2siyddspa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tcwjdoak.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2rvdjeubz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxphjguq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiumqvpg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pymiyqic.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zibsfnpq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rjbypdum.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vffkqpmx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mvfihvzq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2schotnjy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ugqzodss.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bplmvqfh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gzeprqbd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ucdnlckc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yaeisguf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2moixehmr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dzxbxtvs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wmkujreb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ttgkifnv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rjfmsecp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zozabkhi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fiptzsfq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wubqaecb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qhagsmhf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zcweefrg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2knbdfzsc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2biepswpc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ntglbuws.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pecffazu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfptmycq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ifjdjqjz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2lncvebim.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2avrhqysb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xqlddwuk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2okhvtfgz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytznpcxy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2shqahpqr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2fkvrxkfp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jtoegolz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jxsiketj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hinywtaq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mqpbdqsm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dkkhnvap.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rubyhtlh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gvtetszv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tvkzvvio.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2whitfbhr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2awkuxihh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2meotrnbx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jppcwosg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jfkxbwta.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nunadmjn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2oeeorwdh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypayljln.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ujlvxerc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ufbohndz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bssrcfxh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uemtolfj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qwbckypl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ncbnscxl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2veszgsrp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbhoxhds.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2klpohgnb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fdjwmlnd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2utxsoghk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2olfyxlia.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pfpibwax.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lcwltome.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2icctubka.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ytrjboju.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2afhklxna.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rmgzfdhy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hqzcaqpa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mzjzxrwi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2rluscvej.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zknntgdn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2xrrhyltb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xkahpssh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zmxbdnop.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ellkpczu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2zpfkpddb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vxfmyoga.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2soaazkye.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmrsgdmm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2znvusoot.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xtfvapdm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vcbmmmen.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2cvmqtxsw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2uozjohcw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jylexqfm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ujzhmijd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2naanfnsy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vjrpnnvi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uyjzrdxf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xyitnzch.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2vjadfabe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2swliyviw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2uvsbwfwl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2irhtfkpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgcoolbs.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2snkktcde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2biydmpqp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jjyecgnv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bsixspom.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2stkhrenh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ggbgndic.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fckgbpha.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ofmltbkk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ufnactar.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2aytuydcj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zhibjjkc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2krfuwaae.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2sqlkgpno.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bjifpnog.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2askozqsv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2njofvkwx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlucwykg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2szlyvtdg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2uahitwpz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2suerjqxb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jejwwkcg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2jmjhstvn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wvadvrky.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iwvagbkh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2giuqraqo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2glyezhrt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2fmwydqfz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xrozynft.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kwgongve.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2nbvgiyhn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qetfadfs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oglmattl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2izqtjgcp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwboewsv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvshbeef.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wmykszfc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wqiumvgy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fhfptjcp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2hnzyijex.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2bbzsjsju.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2loskwagd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cldnkqwi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azefkudq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhjjsjfh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lvjijuih.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2srfofhjy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfzkxbvn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dkhpcqsj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2yxeugcez.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fvzetggw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ztyjqwmu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2idxwsvbt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2uvakqoho.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2tcvlqscx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2dtyzatck.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tnxuuuhi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2jyyooyue.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pbffbswj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sxcsbcpo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qqrxqczo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tkkyrmkn.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jruwzmqx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2vezyzdmr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nlrhwoaa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2supxzxjl.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2msvfgjnj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dziqxhpb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2cytzpoba.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2sxidprgf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gjtzwaak.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2lvbszosp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2nnfcvdsf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kfnmeznz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vvgdvcav.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bfqeqeyo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2fcqtfqfo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2kszjhzfk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2nhckxppi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2canwmeiy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2naspdpir.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2lcdqoooa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jpazdsld.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ohmdpokg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2btnfvfnn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2bwuvedon.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2njnhgajv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rpljwove.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jvzqhahe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2bqkbpcsa.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2lsgdnfad.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2xmbtoppw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mmbhpmih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmprvwzl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vhlitflk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2leotwzro.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2jamvkscu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xztpvhut.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nkypijlb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtvwgvzq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fihtnolw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hmdsezcu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2mlhjfida.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gouhkfbg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yeuzvlyq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2tueigkdn.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uwdlcizg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jrnufyia.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vqaltmsy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2vfodksdx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tqnyhsvq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpkyutjv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ypdvycpy.html


<!-- 参考信息 -->