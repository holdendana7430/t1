代发 wailian999

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pjfrfadm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkauipei.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gupkyktn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uwoqgice.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kglduidm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pprbjdex.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2txqyefli.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vaqgxjwk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2obayzmbh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hnvxwljz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abzwhtci.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rzxnxgcw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzzymitu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lljhdyyr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ueyqvywt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntppmozt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhyqodjx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xiesblrc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2msfihlcf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmsjshdh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2maynqgbn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpfxwwoh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgfephhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwvdgrql.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2htjparhu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixworsij.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qdhukcoe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kqpihoch.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2iyshblyv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2yuiugzqz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zpzbnxyz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wbfhebxf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yifjfqas.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2clnhuwpy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rligovrr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2iuckeoej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltclwntc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qdopfyzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgjehcfc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2axkrjahd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zydbvruj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fcxdrqxy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rghhoogh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2smxzjjjh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibwdqurz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lqexlcvs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2uttvcxny.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcsiwbol.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2thgbspys.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jalkkknz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmqxdavj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idhwbddh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmylzohf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntkfkjzh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2clacqrgq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mhqjpahr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yxtsumnm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hpuvoxtm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yffasxph.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bjtvkqiq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2iawjtwcr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uiplrgvg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ytiritqj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hjvbkssf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nbkqxpmt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ponzdgob.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fmeekvck.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rzpthhom.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lukgogwj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqbmotbf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fpkumjry.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pvvllgyl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ctaukouq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ujwhwgjx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2thynqxzl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zetbaorh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2uasqnvil.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2apmpeuwb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2plmvwgde.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ysiibvzt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2blnddmck.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2knxqoreo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2apflrjjp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2noowuevj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jdiryftj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ngfgdejk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sortbqjn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aewucmar.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cybtsrcm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrcikjoo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nfhyhptw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2eobmxrul.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qgusirul.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mnjaussn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2skupsoew.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jjznjlng.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ammchsrp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vpgewfyc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bipqyqgy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xxccgzqh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vhltfqhz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mwwuofoi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2igacwntx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lbgjqahx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lpxariei.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uirdjqwe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hswktyme.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyyrqsdv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gbfdoesi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2oanppzyt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwgibgtz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2phrkzrvv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pdzyvhhw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcylyyvo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kyimhrhd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2azgbncmj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ccmwxnrc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2cuvujatk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jpobtjzf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dslhiqml.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ptjvputl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2aqsxyizp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jrpjmgrh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hpulgaay.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ulorxypg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ghyclnfo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2vfdqmeyd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2innyetjx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ukkiezvv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fpbixglv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2oxbdejyj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmwkiskz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zvxdahsb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qoctrieo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzokjxtj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2guxczbtd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rmsprtbe.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdwjkpnk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pqhoercl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zrghqadf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lfymskqk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rhfatfcn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yqrvvmrw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xmdfanfk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ngxlhhpv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ykfqyqwc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ujombuik.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2adcrhhdf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rhlafieq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iobrihst.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rathwndt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2efpcrmje.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jxzrfbdz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tljcgotm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xkwimwcm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2inpynoju.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gjorlzep.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2aoijsoky.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dotwzfkd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ydtuqbaa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2blgbldbe.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbfylrkp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mtgvhowc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fpsowsvf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2dxxjgnli.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2igcghxlu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2dpwqlogo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzxyledn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hdnhuyhp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uwvswdxs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bamsvjvs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yspnsfhz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2froqvpox.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lpaybxkw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2cvqhxnun.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bqhpcgbf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2gqbyfrqy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vmkmfyjs.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lpzhbznt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nplkljna.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2nfkhiwfo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2cxchvhpp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jcbdosbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmsxpera.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jgksfbqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rawhwbej.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qcpvxisj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2veeofvyk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2dsbtznle.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2stbqbcey.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xccdcosi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2coqbcxtc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2zfmnluoe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2polhwzyl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgjvxckz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2bshjbeha.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2omgyejvj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmnedkrk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mffmxrno.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtdotgfg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kmeuyble.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2zomhaauc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2srqzslhq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rrkgjqpc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kzqlyukd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2sfoxkqdv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pxvuwidc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jzparrfe.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jzfmrqmm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pcwwshls.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vnbrxhoo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fybpbvol.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yldmsgxj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2piwihgct.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ckpqchnh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tocscfss.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2apwashyw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xpqbyspi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ddugfcyh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tlseeyba.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2qaxittun.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2eatszetn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vdnzlqby.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2mhymsyxi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhceeczq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rxwrfvzr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2diiktrvk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffnjfbqe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ftzikptf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2llmidelo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2nllfwrsv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ljpopchv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qonkqdvi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2epgrtvje.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ddurgqzc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tqjcldlm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ecqwmglb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qhmkvkab.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2zzuufsyk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2awfdiqqz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ldqygwry.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2keoaniey.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2paejlicm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jlbnlmrr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vkyltxvt.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zuftwtjc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2yjywtpmi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2uzxciakd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nxmaywfo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2cuisqowp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hecxsrxa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2weyuwkjf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qzaomakl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ktpiqxvb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2guqlcujy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2rllavhay.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2lufwcpbg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2yfpyvobg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2wbdosfpv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2itqrppen.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ppwentzj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2oodpgnsd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rzzqfmtw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2eximveji.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kgaghrto.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uxcdxkam.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2babiguvj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2suakpxcm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2vbolywrk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2nmcfvgmw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bnmisund.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2znpxhjnc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2wafoxjfr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2qvinwdhq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bxwgtfdd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bckzoonc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdeqcdjl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kjygmpjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgmiqnqo.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gfusmgno.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgvhdajt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vcxrbfox.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tszciipv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oguutzhy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2uefzrkib.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jdwtofoh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cncgwedx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ugkcutaw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hkoyztra.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hihotevi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2bkerchkp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2zhizpxqg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jzyrwwpd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufmzboms.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2psaloqdc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ldxtbgps.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aomjtkym.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2yjnatodr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pldbujlv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2gsfhhkmz.html


<!-- 参考信息 -->