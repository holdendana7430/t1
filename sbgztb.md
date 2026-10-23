代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xpviyqtk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kydkwuhv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aahcmeit.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pnmvpema.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eebbwvrw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jrvqicqa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ihvpiuum.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tkqhjyne.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mzzarrkd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dcuaowot.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gigqwpsi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rcksavcd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uikhobga.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfbxmmio.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pgiaxkln.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mvhkbvza.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqwsugqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jfilkybg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wwsfeqix.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkrrzoei.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lthqsonc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygnpnzny.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxvoflyb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nnfbptyl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wigsjaez.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oznzkcnc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bjlklaye.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zppezibx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ksavneuo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3muzmlvzk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wdhfdiqt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rbjyqmhn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3obihvqmk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xukiypnf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tfcingmb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3uealkclg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apdosonn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ilhxzjkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwbjojxf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3meiwzbll.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3fapifrer.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bazndhau.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwitxtzx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggbufgdl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eantbhvj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3oflxrqrl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yitjkqjg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3znsybblv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kdoobrfz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3kvvnfzfs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hoazzaxz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gthovoag.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3egahxtlm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3edciyapn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3nsfqjoqe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbsvcqaq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zntflrua.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xmlczara.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lnhrzqwx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3grjykmos.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zdxaghva.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3njpobwec.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zjirfobv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3dqcgggxs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3amrwdrzx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3obklaijv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vhvpexav.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3akfknnjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqqsqocq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fkpimqzi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mvpueknu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuhaarnp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ywmprqbg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wfyhfwkp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fcgekrty.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tulswcet.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pfwfmtek.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xufgjcfd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3faynthvp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qynuzdaw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ijnvvnvp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3uiwidxud.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sdqobiuf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dfmkdwii.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qgdivwvo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pyvnmfeb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3txpbjlny.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iflubqcp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbptfcuf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xkjmzrlr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lawsbbfa.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3byjpesrp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ispkdkhf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tsabkaqo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3unjhtpmr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3rcdnfjqi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3acoijlgb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jswyabsa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ezzjmacf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rggpvxmr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ggnuwsnz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wfstcyqd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pampraom.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3nsrasvis.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkeoeoyl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xkfppmch.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hceigvxy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozdzrnlr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pvebpbvy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qcvwtimo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rotpdgds.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3adgpetrp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3fmqpetix.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3lwnvqxty.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3krcklbzf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xthxyidb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdprcmon.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mtvdziyp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3icirwahj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hlcdpxtq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3voivtriy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vkrjzhyt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yxsuchvn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3poldvdgl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3muilkggd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kguxrazd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vrgsyatt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ynngoojx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ruhakzdi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nglmwyee.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rqjngiyx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bzprnput.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpgxemzv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kymottak.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjhhqrfy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cfpwpgdr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jdofrlnu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3pycqvgxs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rjtbmvdg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bultrkow.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhionmil.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfvxrltu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3boilfxbh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aactdqzz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jwehaixe.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwegrmyo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rvbrjihg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3latcgnqu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cqfpodnd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3swujmjot.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aknirrye.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gsrcdbhg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3idvsbazl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jsejrlgl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3asoimung.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yxjmptnh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bqbgxoda.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3yuzkxnip.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qopijnie.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3irzyiaus.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pmldqink.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nehzgvuo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mpukgqdr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ohffnhtx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qkmrawzp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3trzpvhxj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3arnnctqf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mezcapqe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3cxhsppvy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jrbmnkec.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qcynabca.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dydklojg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vcwkuuui.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fwkbsaif.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3sclboapo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dypsigxy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yulwaywa.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ifzgymaf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tsgvfnuy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3bdktxobd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3cmiobufp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3vmfjhdhp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fwbbtbvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppirwwvl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vnlugsgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjtqfvmt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3tivvxsel.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sqqceesb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3juhexbmz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oavwwrtv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qazwspml.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbzwhsau.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tsbzmpjh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ufmqltyl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gtsccbgv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3faboykys.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3nbwtaqhk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmmnpkpq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mogofnth.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nkqlvani.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rgekexob.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cpetmljp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3imeezxvz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dbnhvibm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yubbjjbm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3yrhzpawf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lfaqmhqg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fdvaijph.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kdfgjtza.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3egoftcqh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3saukgknu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3uywngprm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aljgodej.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3uwsilwku.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bihfgbbu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jadfizts.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3utuzpzdz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcjwoqmu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsokhbjq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zcqtlisk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3hfiahzfc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3uckilsii.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3gqwzgldo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kjwcmgai.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3llghvglf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tulaasvp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3opnxjyoh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gewzykwm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3fhvuhifj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ovbgbswi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptqnnhis.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lghdcduy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3pptukwwk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hxxljrhi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mkrnnmmj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yfsblynl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ikfefqca.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3rmohgmye.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3fpomtiak.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ctaeliqv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3vgvjrsjz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3txqhadyd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dwcpscmq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fyfwzvkd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3teqplyxp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3vlfigldh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3knbxfomz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3zsoqicrn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uitslgey.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xjbpqnec.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3tirwepwl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3caqjubrc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3oiqnjcyx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fitxtmxa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dijaxtkc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3utrmxuen.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3qforlurv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3odchyvlp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3uqyroizh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3okycitnn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3jzdqkkty.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3oufmmzvg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3orhvojti.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3joidljkc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3qablqqpp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mwudnrch.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3qnjovqud.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3tscelkod.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3zmtgnyin.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3gwthwdjl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lawormda.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ikwwdtcz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ecjhkgrc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3nckzeeao.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tuuwqohs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qrijxmui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3foszvkac.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3truuqlyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yynfxjvy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tszgdzdh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmzmyqw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qnpbxvdz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltsdjuwb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bumstqau.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ayoagufn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3nomzhtls.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3cdtnsezz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cwmvcykh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pkxiqikc.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hdgvpsyy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3iejnzexk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3buycevjp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xeohctoh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3zttkwjhh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qhwfvrib.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwmefyo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yuhujeys.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3lbgdbeji.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqocvgan.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3umvakkrf.html


<!-- 参考信息 -->