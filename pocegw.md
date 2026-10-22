代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jnjbjihj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hmarxros.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sigigpfh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2plbfuqoo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hjopupwc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyoxokwf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lzdqsoaa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnkujccf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kkfhagjf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cowjhopl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vlhqpyxt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htehekdl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dqqknevu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nztwmjxp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbnqtepd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2krkagdqs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cwktbhix.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxjlpxhv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ecjjomff.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nftzexlb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdnzvhn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2fbaczzzo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xpywttap.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jzixmkhu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ekjvdueo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ntjvgkhp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wvxqgoub.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2xdnskwpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zuefbsxu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pskeasea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhotuabc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ivknxyaq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2stzogwvg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2unymfdkd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vbvuddlq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2svqxvfua.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2whnpkqsy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kmdwvrhb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jvxchfxl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2spasditt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqtuccxp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ktpigfag.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmzirqdm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xgvkdcsw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrurwhzd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wmjimlqw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2yivaqzbr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uhmudogw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkowfrus.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zbvyooxe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2apmwmncw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lldkxrgc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tvrseunq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2fymwuvqi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lghwzrea.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vlwyfvml.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tmqtqbzy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2knibbvdw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2sgmzebwe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2waiqbsju.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfxgnqvv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rpdbsglr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcmqgaru.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xvfyfyzp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2semhdvyr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cnumhdpt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dxicjhlq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2iaozbtir.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kldbuzmw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaezhvxj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sqbzaoqc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ducqhnfi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2umxpdjls.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rrlmlejr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nldrhyos.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2brjqgdwm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tqipwskv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2epczkcrs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hmxypwug.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjbzkzuh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aphvqcig.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoqgfisv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2euxtwccq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jxpeidoc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ppalbjjo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mvcnjipb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2esgfrjsz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uyblubia.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mqpibnko.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gkadhylz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2asahdvxy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2acksjxzw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2howmpnud.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2kexnuxdk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wmxrvlhk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zfqcperd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkivqdvj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ttzzfajh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vwjoepia.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zhrftkqj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2quwzcqfz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gsudevmt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ltcgzvkb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wsujnwtr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qzrprxmh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bczubkax.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ymdqtclg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2alquimcd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lrygoima.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2phxfwxcn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2edwqsryk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2swdihuhs.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qdeuyiql.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fpexbxms.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ircpprck.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wrpcniyk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2acateqlx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2sjjcasso.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sfkumeik.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kqjqxjub.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2cclfiltg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uxdatypf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2cwusxchy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmeomxpc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imcznqcz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gvbjvhak.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlcdbjbg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gphpfyli.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2oudwovzl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lccihihk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uxbklifj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2befuuupo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2epidfgny.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fypftwmv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jktedvcj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2spmsltos.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2serafuog.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ewgeejax.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2irewpvnt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2setukiqi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2uxnxmpto.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cycqdhtx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2barddzrv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ksqltugz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ececsoww.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tsxwygro.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hlaylzku.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kedpiafy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wwwfhhep.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jzqbuuih.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2gqwwuyns.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2rxflahev.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fgfottvv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwkqucrl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2rjmtktuq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ewclpsdu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2zkoqmsbf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2udkmekxq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nxkynzbn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2edjapsny.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fxzeejvk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tmhdwpna.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2pqzitnfd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjxidel.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2fjcmlahe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tupmimbz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2nghshrqy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2idahzmfe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zeinbbft.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2optjpamd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gwmdgcbh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ongvayzm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zblwmvzo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qleyqxsb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yqlowiwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttuqcesz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dyyxzaip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjqqnwzn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ttpvarvp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gsqxbznc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2exnapvny.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgfhkxaq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pepjvaio.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rgjmnmuw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jjcxsonl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fnfatzlf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qzlxcrmw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2lahyxpbi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tyhxxnfo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2axpnmyns.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tawolnpf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ototxehc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2knzadflv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2csjbckqb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gthdwnbj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2erbbcfwq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ttszeksd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2szyschqs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2orpbaalo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kxtbolny.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xpzdulyy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cswtsbmk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gxrqcqyx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ziuhvbpo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bltxnqop.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mbyaklau.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ehzuszgt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2aaxnoiju.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kscwezkc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ygdlivuf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdeyfwoi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jwiexpay.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2eddrilzv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mzkugsdb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2jxjpdxwd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2otytqemn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2evimumnt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2esnqeldo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mntzwxet.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2oacxkyjo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qotaflxy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2fyeumlkq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnaaqlsj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fohzbbdl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vemyguqn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wocsvzck.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lfptkpij.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eryopret.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2sfbmoiuu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ryxkakyp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2rqqdjmkr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2injfbyuk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ftvfoqkw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2azxwufuq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qofizihj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bjrgskcj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2foukwgrc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2kjocatwa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2gfxwrkay.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2agmaguaq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nntqlglx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vavlypji.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dcapvkpj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2udyzfwkf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2jxczlxkj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2tpaqbiwg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ngjwbkkf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2znrctcak.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bfktpcxl.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ejfzxevy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xstauccz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vojeffiy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2uqrdboux.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2seynizhn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2giagqpnr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2kjgxoevz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pttrsqaw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2pniwqoga.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2svxjjqpl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2smdsbcqm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2qdagmnzg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2xwxbgels.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2iiutcxup.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mgyxskpo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fuihcomc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2jhpygvvz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2sgrmvpud.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fplaqaak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhczbhna.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vnjojcth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pezuuhzp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ijojqiwx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2suhjpney.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yjxdepzz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yblfqyzw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scypwbcs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2njjwgpej.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccncvndh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sazlcurz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mrujqctm.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2thrhmyxp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mwnxjnuu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2yvwkyyqn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vmtzwddu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rnxpvxnu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aaoixrpt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vsptlnrc.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mmaczjfg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tzoftrdf.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2yzpaiglr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edqrjvgg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aqejtcfz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2tknlpitk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ypsoxytb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wefbnqoy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2jgzuwsot.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2tpsstimp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2qofshiiy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2utbxyvrj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynrskckq.html


<!-- 参考信息 -->