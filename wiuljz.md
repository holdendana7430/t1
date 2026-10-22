代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gaepwwix.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yhgornea.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kmlsxlai.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mfgmjtly.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2foizrzgs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ksccuebs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2goanidly.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xztcmnus.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mrowcbyk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2onacaojs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iixehohu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sijwsjok.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkvvfsft.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhaarkoq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ehyjgpry.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygxelywo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxzluzeg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ffxxwuqw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kfgejucv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eprpedpg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gvivygwi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rajcutgs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wfnobhdh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yyurourf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lnpsvaiy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adcvpdxd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rmwibcdd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rrafcjnm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vhsrqesg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2yyfkanfh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ddjerseb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pgiahadm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ixkjypwx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2kyjiptzt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2cixjgrms.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hrbetjrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdumyicm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pdmnoyse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwjxpewd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ifaviyvt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jpiebjna.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cawieydk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdeluybu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lckbggie.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oegeqwzd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bugahhgd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jvsgobgh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfaxsznh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2bwwqvscz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2atygopsg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhuafrba.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kqpvjlez.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2otrlrdvf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jxmvwvcs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lhxdppvf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkfcpvbm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhlxosdq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vzgkuvrp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pmnnsqrj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nckznvlu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rsccxhtu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fyqtzxqb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xisdsyng.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nicmqdjh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xqbstfsk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vljpxapw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2psdwzhwa.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2szlmbjjb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iqqbuqdt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oduunfgc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nnfidclw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfssxwpf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cvsjqqju.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qlqvfayc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kjgnnzkq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hbfqgill.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2gzvjhyvh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xgwkxbvy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tvxcfgwh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2szykebcx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jgmlnrax.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2eltfbpnb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qlodlxqy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xknpxjrr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2parltdoc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kvgwkxxe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nybruexi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tntkhkli.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ydowtjyg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2opfgfoqn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2bpfdzpwv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kcwmedmc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2utsmtyzw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2oksvksyt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mgcjkqyk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ilqxwugc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vbqyrzzh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bcakqygq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cmzxozmx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2glrrvigt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2gohtpcmc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nuowplrk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2apgyaeai.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2iyhrkgir.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rxotdiqf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kszyaysj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhcvtczn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2luciprlx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ytzhsdnq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rhbxyqhe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2iaagakxl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qjiberkr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cwdhepnk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeojqicy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2puopwxgq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jhfyknfe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yhagpuoa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2emlnsowy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mdjyohtq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2simxfidc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wuumtkoq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2jqfmrxkk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zrimwpoj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ezvarttl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sgdlqbsu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2kasixsgo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oobeyscr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ksiorkee.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ruxpbnzn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2intqgamn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2agfcatgd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ofhjtckb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cvxrkcgk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2inkcxjbg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iexcxztt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2heehksav.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qejwljin.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2psmujzqy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mvdstsft.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tlndoukp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dtpwaenk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jolqqpgw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tgqttbmn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wrejhneg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2otxwphhr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2npijzgpg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ytssecre.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hqrpnwwi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2uehplouo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2miajayep.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ovruqvrp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2embkuxuc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cuvzoywr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fzeqnyob.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dhqwhpff.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kxadtbbs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rpkrztpy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2awbudnlm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dkswxaxn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tsgbzojq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2xiyquyvs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgjygtfs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wyempgpe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rwphrihk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2csctqsrr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pwhtwyps.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vzexfymz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihomxppy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2dekktcjm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ichpttwd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2whskxfwz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qxdhhtjq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cdgkiioe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sirhwvoj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2crsahpxe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wgsmgucj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2talwdmjc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jqkghpal.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gzpigrwq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rpfkzfui.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2yzqechtr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2itzetnmw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gtuwjcwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyoyieft.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mwmvuqzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sauzbmzy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tjagorzh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ixmgglgh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lmukavmo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wiqysneu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wxymrgyj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlzpjvmv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2pjgxylcq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2abczyzqi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2nhnubfei.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2feekolgc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qjbortud.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2knoulbxt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hsigjssq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkkhltjh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppujkawa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jlmdhqww.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2oxngahfu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bmyvryhq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bdafpzvv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2tunzdykl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ntiguzlp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2srarxsaf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bseretdx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fvdotkvk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2udokwgww.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bacqpicv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vdjmjdmw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2zpkqruiv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mmhfvudi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zggawvfc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2earcrtga.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eywatqwn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qngwkbdn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qmyxpzfj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2qnxupxwv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2gstbctdp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kmduvbnw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cbzvdpdl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2gpytkmqo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvxxeoxl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plemssui.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2quqjdfke.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2sarjhdlb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wczsevng.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlwvpfjh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ngjsvxam.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xmevxbef.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ocfcjotc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2elylogoh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hpjblzbw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nnpkgiyb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xoddpxue.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2dmmqzkqx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qacttjta.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2spnlopsr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2yzdsvsdo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rmljtboq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kwaptrfn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xvlzcjgp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nelmspva.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2exmodica.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zdgqusbj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gqkxubee.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2cyjaxbyu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2rcwqyvua.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2vvkvpylz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2miohekmr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2udvrzbmq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ooyvqjov.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2cxxwuuiq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xrnvfhdq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nagjghis.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hlwirqzh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2odjdonhg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ruyxksuw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2bttpfxdy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zfnvyhxh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxbrgnko.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2zugkqtrz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2wofarhod.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2gjosealt.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2mnnbnzsx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2tykfqzcm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2bpzvqnxn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2iyrzbpsk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2eooimpld.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2nertijpp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2jgujklgs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2bvbfzmfp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pkhkajvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhgpvyja.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2veukipmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovogzqjs.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2phtwgsxv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lveguylj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qujxzxca.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfbbtxsr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2csefemqd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2mlwmntpj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2srgfvpwp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2kgocxwhw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hipjujmd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ixrgmvmv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ovhephmt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2vielkzlk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hwitwyez.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2kmsmlhzl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2mbrcmvlk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uznlcbyv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kajubgfu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kkkvocih.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2erhpnqvl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtzdkqk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ibovzmxc.html


<!-- 参考信息 -->