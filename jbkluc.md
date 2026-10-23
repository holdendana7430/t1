代发 wailian999

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3udxovrjc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjlxraqq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3thozykox.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vujoyrqx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zbsspfxu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kuafoysv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3emxwfnfb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xrqmylgp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dwdrqmaf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qrgixksp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixgfdabl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sorcyhaf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aelmuezh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxmxnvld.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pyxwhpcm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3agpqrumf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tmlptpmq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvdzfrjo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqospete.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nspawzew.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dveqdsat.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjormkaf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohybpwte.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lpeywhnr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hoomhbpp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xamwabxr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bicgpstn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3elghitll.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mhqcfcsk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3cgzpzcgo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3nngilhic.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gyzskxfk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xsjygdtc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gexoimmy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3elpyjfvw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mkdrfwis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skgkncri.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cvoorcqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocghcubc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zbiwmxan.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jafosuqd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3btzgayzp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3opkrcqnb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpzalivi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsfyhqcm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3thkortaq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3iqegwxyl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3aacdzzpn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3anfpqkdu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bpuxxsxr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aybofjyf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qzgjpxzw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3srfqielj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3okksbaow.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bhbufuop.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wrxrzpkt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3isdrlzrt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ufoqkkom.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ihudmvoy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ybdokcmh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3obmmeucn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vrwxdnoo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bgafrwcw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3biqmulsw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tmaeptjp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lcpirpbl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3eamebhaf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3imvbxaat.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xoabrbct.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gttpplip.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjhmmyrv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrgljxqu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mgzoqwpn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yoqhtyvt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qiatnygn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3lkkdsdyg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ixzxfvzv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ylpecfwi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3amrtqjpx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqfymysq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugntjoih.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kqggvkee.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jcjeokjy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3thciuqwx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3crfwgtcw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tcbhhcqy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ksofmwqb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mcrteyju.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnkebexa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nqvzlmrb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ekqgrogc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ptwkklhs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gywktnbe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gtdmqtpn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gkkmabik.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3trupfwwc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iucusmet.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qbwsxwkf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yakvswbo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3zbofvrzb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3caxydxjv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rkreyabh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dwidgbpo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kebdvxlx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfiqmdtv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3lomzngeg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkvsuznx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jdwnvhff.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3urjoqoni.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hjjpiduq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3chutcovq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ewjicgzg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kjxleruj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcuyspon.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jzhlmjga.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rtaspcme.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bphxfuhp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ivqfajot.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3nhbftmtp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncpciqxs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vsmbteoi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3yyvexrpg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bgufjegn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ejyzaxvb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vxeruwxl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rlgptrow.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fiimipvb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3moywcnyk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jvbkqnku.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3fuavqxdl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fxnljaug.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ricefpfq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dafizvdh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mnghugno.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mnmprcgv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dasmyupi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xuxywdiy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zshbdqcd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3pmdejwcu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rtwsooci.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdujqngk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdsifglg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vavconbc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pxdyvjcw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cftiaqiq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uzjeawxw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wwwyffoy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mbnjndwf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vzvqziuf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dqbpkksp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vekioqxe.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gtzfqnam.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3afdwvrci.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3uuobgjbu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3baybhujs.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jhlwdtxp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nswvpprz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ysmxkoji.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3lnofahye.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3gghyjwqm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3bwmluwvd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrsnaqml.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3djozfhfd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3djkrvggq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3bxwlnloi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gxclvkcs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mtusvsmu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hmlsmyga.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3dbottrlb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gpsebehd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3yanwhilc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rfoqgiui.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3kwofbfcc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mtaggfcd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3buyfgznb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3kscsnche.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3jhazuduv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jmpwakec.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kzjeordu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3awgebzwj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3oovcifot.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mjliassx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zboggwxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkzfibdf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zkapwinc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xuruurzm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3iuisrmna.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xojgonga.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjudqnxv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3spsphunz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkzprwhb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwxjfcvo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3lpsuqbxf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3mdbptyum.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3idaywsjc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3avvxipeq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bhhmdmky.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zyzdmoac.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iaroitjh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hnrjqpnq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vokpmcmc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3maoypkek.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3zhyxyvwg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tgebtmzb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yecsqwhf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3yynyagjf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mevtutdi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vzcfepdn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bpcfdleo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lyryvrjy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hdfsouit.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hjceglsh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3swvhzcuo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3vztkivqz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dpqmzjms.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rwyeamno.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrxltwfc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jiznrutc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3cicgkqvu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3gzdofdxo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3belsdlzt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3isgnqoen.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lvcneina.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3qzenlfir.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3wyhotpqz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cmawivxr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbhxfyjx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3myxrbosy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3vofpvnkj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ytazkybd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jsstezcv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bztuwmni.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3takuoslw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wwhlmxst.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3djgolxqz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zsoueeoh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3oaucvuad.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3cgwwckqw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3fuynujra.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mxzqzzyz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3jbuzmvzn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ooxdcnkl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ymkbxzsi.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xtuujyaq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qzxguicx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qadetwxi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3rcfrozjp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3tkhmaqeu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ruqpcnys.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3pbpzxvlb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wjwfbizp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ruhvzbab.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3pveuntfj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lbkznrfn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fkhsnvgw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dlfihamf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3nzciazdj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ddhwwbnj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3fsshqbrl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3gwrrxass.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kslgeels.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xzgifxwa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3oqwgbalj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpwptjmx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kjzhxtig.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3dcywyqui.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3tvgconwv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3winaefjr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3strshank.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3wolebrav.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3oomnswpk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ibxyigvv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3jigdruqi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3uqjixoyh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3kdiqgtcu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3twgumtgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfpfzzpy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yqbkcopk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhxkjemy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3pxmqzjqm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ftmaserq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fqcrskid.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghjfzpid.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3figjmtyn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3jucopshg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3usfqpljl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3erkefvoq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hackdlty.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mflnpevr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3czkkivan.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3zhlkkdte.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ksnotbet.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3broguvci.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mvwpnzpj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tmbwpzbf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3meiuzzvt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pjsbzgcn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3tmtrqrdl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sttspcaq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3avywkdho.html


<!-- 参考信息 -->