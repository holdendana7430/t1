代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2npkybbtm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2pgptijui.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfjbsmel.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ydnteaqh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lupzowke.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vqfdexqy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uxltbqlr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqrianrs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzuscuwu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hypccdar.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2odilzyiu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcwewglk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fznmldre.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sfwsjzaq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bcniyewy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dsjiukhv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kbblrzzy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzngzwhf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2kfqcbitb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2czrbmdvw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pxivbvbr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jxzldaso.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wezulpnv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pfehczue.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jggflydv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2fghmenhk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gcnmsqcb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ieafetgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpoplabx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qkocpbgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hugbuggm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2knihvtvm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2uzsswmqy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ijogmpvg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nwxkintb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcxffupb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xntycmsn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2bumptmuv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wewuyprc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wizffkmb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dcwyovvp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2khaiblud.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gkfqlwcn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grzbxcvx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2aaxdshdk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2owudjrog.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ybhwofen.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2krlpdrrk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mkmhuswv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qdmghyij.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jbrshkvw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ihjzxlum.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iuqqqjyd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ltijfqof.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2khecjuar.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qwwtygjl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pjksyidk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xrqjtiev.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2bxepibgp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zpxezwsv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nquyfnfl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2girurboy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kuddqjug.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjkjslbc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2slmenjwe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2otnvnfru.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hrawumjy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xxiaswgr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2szefhuzz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hvzqmjxq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdaikbqm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2srbehsdq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kuvyccmm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zbpoaima.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2yjtprcnz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2owpxbcfy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ybesbxbu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pawgeneg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2czydvylf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wepivsxn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yxbcxjoi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlgizvkf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2syzzdkdk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2evkpruet.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xznuxzjm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pcrqrabp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2swjrdzaj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2uxyboslp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xrfogmbw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oatlmfkp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ekxqdpbj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lykuscai.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ypviftff.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2lwwqvqwh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iiugbwby.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2uszqtjlu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vqcsyiup.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jutdkdny.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuocyfst.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2dudejshw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lbiwzitn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2pyqlettl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cesglovy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cgevpnyy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xeatabrq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nrxdflzu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2pturlqem.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2intuedoy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2otynwovn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mkywmkxf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ynjyqtah.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2twhyfpyq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2usdbgwlc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bnhoffmv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yixljaud.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vhswfzup.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lqqilglx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hzsqzhmq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wqmdyzdq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kmurwzke.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2truuidzj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bxdojaeu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bnsmaxxc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iebzemnm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwechtnn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljroijpl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uzwhvtpe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hnitfxvb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rytghbwy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2garlpfpt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kbsqziub.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2voigxeou.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cigvqkib.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrsubnbm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfzqtknn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxlpxeyz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nktwhzfh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ryrpvfvs.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ijrnwgms.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xwtgymnj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2iborwplr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dpmivkop.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qsgtmdpu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iyckvrar.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nhdpbjzi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nfhouinm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2odcuqfbl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gmgwvxdk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2dtwmatfz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2gikoynxr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vahpzker.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2sqnkdyjr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mukklnrh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtjwrvom.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2egmhaikt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ijtnsumz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2taegabkg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2zgqfqqyl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tpcovziq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucregajt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rkwudddn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xyweamzm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jvwpkcsv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ouujkmdv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qxrepnij.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2akmxpttf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2iyzrdblo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zoycxowu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fhrewbxt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vurjfrgd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2frogkhqs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vkxfuela.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2monfvwlj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2tfnzdevx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ikxsadxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcusvjpe.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2mitiexrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqbtmnzo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2aqxfmfzt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rtacjsok.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zqwvqlnr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2glczzhut.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2unsbeyuo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2esgoeucz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2oipzjmso.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qhnmbgpc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ienzoyge.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2sbzplvjx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2oufttajf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qrglkdpy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qrweskgd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ceecxsds.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpscldku.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pbipejhb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2duvttkqn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ratcbkns.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2odqwpkde.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2btmmmyoh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ncihzqde.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vbrlzqvm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ejtlysvp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kxqqlabn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2spjbfjob.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2radkstrq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vaqwdmwu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ommfpkqc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2mjbribtr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fhugorqr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vkrzkdmj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnvuesys.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ucgxbpse.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rptvsvdk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2fvatkkvy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2dvzeagry.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ardkxudd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2eavwjmvw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ugnzshak.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxbpztmi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xmucukzs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgvmjaku.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2uzqpsnzn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2udfzjbrj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2pvbeqdfy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dmovzrqq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qwdcqgzb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2glnouphk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rxdfqyup.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2obqtggma.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqfdasm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ogubozgf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ngevuzut.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ugkcyhmw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gxmaltod.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2dmueifyr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2caqcsgvz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mpzngrgu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jammoyqs.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xvwzoecl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hiqzawoq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2mtpkdjzp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zznqkivi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mqkaykpm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2khngdzok.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2naappsmv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ywwyxwru.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2anfgelew.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2rrbxyvfx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2sgqveqpw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2plyjwwfd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2wmdgurek.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2sucislki.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ssskefbw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2lvtppdtc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2jtdsixyk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2muveuqmz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkhtldue.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2dezszbsg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xkdvljxu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lfjscuwe.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2xqhikuaq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2necwrszx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2jbhvcebw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wxoaccqi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nrypovws.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2cbeprrql.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2xjgrdaoo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2tzungghi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nyxtlbma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgomqjxo.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ydkjovsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbanvuim.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rzdayfpw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2svutxkfc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gnxcmlnq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dofbwiqr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vpgtiwxg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2hqugixuq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2acatdxzc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nfeyzfew.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jsqmienv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ooxrnxxz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hulesfui.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2pqqcoixl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2pkxfgcjz.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2palakpcg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2otztblzn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmmljgov.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ttrwjjew.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2alpucafr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2dfaodayp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2hxcevwrk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bcgpejlr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2tkicrkik.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2hzizixvg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iimpzbva.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2bjwdjhfq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2khlqbpoh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2zypowwqi.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zsbyqyav.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2sclbtjef.html


<!-- 参考信息 -->