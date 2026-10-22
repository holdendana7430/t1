代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zdblncio.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fkdcecxp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ilhmogrx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtuvuedh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2joiocmzp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2oxofryhy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pysptijd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rpfoqibg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2esvxhlzj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2omtvmhxp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2iuukykxv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2usmndyzm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llznkyqi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2svukiazi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhftybnx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpsuzwkh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qnsuymmx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2igrlvqmg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slbuaniq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2menifmgg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2avttznrp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2enabkmsn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2maxtmplz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ijeimrxr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nzugwxhn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zzaegwar.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2rrpijpls.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2upyqluco.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tcozumso.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2isnnkwni.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ihoottqd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2djfuqzbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogdftbfk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dajzdatz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swpzaemb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2frltsbyy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bdxkptil.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ehxvuluy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mchksmxb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2pktkqzmr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qkkfblsi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2uzwosuqx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ivqkzqcz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2acvxcivh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2inxwyaiw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ytjzfstf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmgiezdh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfcapyhu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szwbeasy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lmdcyiol.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2sdiwxrst.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2opuegdfl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dghbszun.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tiqhlvnz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ouhndcwt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gkvzdzev.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gmmzmkwb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ixbomumg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ryijcugo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vaeidrwt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rfvlwjkq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2spebkmlm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2dngvhchj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pqbbrgon.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqbjddfw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bgdnuvwq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fltszpxr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ngonyhji.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ursfatet.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xtxahmix.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cnchzayc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2sqzddnhe.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xkktesya.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oepzswzp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bgypzbmh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kikpiywd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhsgeexs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2uezhxrcv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xuglvpym.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2seblqjqr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jqmgsijv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ffmewfag.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gbyesfab.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqogskfx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2teyklbtp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2frltzljr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kvrhuiiu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2oivnkrrt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hcovstzd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xrqedrpa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vkstbhgr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uiutbowd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ncmhfrcx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ggqvpiav.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2msszcykc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lkdngtkh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xnsllerb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ygcrflxh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rvarpepm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2maxssqji.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhcfxzxg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywyqckzu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcrmjafj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zbjczghy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pboqsskq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2urwdulmw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2chxnljiy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qdafqttx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2flvtsvwj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2cxhfxerp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jaggwcpu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzshgugv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbczsdxb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2knnmgcsd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mqroxbha.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lkykkdjd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2mbfovrgw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qdzvyqlc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2chtppjvm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qjxxkejh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2chhgzupx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nbrsdrdw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2glwpmjck.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yazqdyum.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ujajldcc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rcxmabtj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xhhmrwjy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjpvblny.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2svjsxdnm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2upqwyhwg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2czsdinkq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2whvqproa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xmirgcrj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2baijhmnj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2flnzopiy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yaunonaf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyglbiyf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tphrymjc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjpxqfyj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hqfhgauj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dxtjihmr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ityrhcvm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ukyxyuxa.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fxrfgoui.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ybdbbzwi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ahvdqwdn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2afeihadl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yroqmcpk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ntzyemgj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2pnosywta.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nochhwhi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tgeevmcx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jyrzpddy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2nxomxhzf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hzbjeasr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2irwilrtr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gsozbeqf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2panghfwv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2rasjtmjl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qiopdlgc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2guwpvfhg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2stesfltn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2orbhfqzz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2xusncksz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hohsgtlo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qbahokyo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2neshxwjq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2tmjplglv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qrldlqnn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ecektomc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nzykchws.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2atdzourf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wwhecwac.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pxmnfdvu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zycybvot.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jumigcdb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2cjtiyyji.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2mmxasjnj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mfwfigpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsesxjvg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gcqkmjls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guoqrzqw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ryarnsyk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2leeyqono.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2idvppydo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjgrqgie.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2oapzorxx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2tbgzsngj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2hqddqqbc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2knukexnw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2nkiafqew.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zqshxall.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qihzngfl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sjonizbu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nybnzcgo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtewcbj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzlgelwb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2spsnsvdd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2oyyiluvd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zdnpadfs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kiqhkwxk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zdvtejbc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ddskeuso.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2athdmuag.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lxnotlbq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cwewehtu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzpkgao.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mecdyuvl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jfvyubhs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2jzigdsfr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2isfggmtu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbbdbmqb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fpzpuhod.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2abesaksr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2unkbiahl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2hvcustoz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2nrsafmlw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ugheumuj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2rpxshepn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2kvwayspa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2nlrnuqoe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jgcazdss.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmpstoqn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2bukzkirf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxdfzjh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ngryuptc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyztzoad.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2pyxotxsl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qsaolvxw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zcwrfkiw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ybhjttph.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tjgnsroe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2gyigtmfa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xvqialqb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2waqgiyxy.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fokcgzem.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ofbibasg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2hzxjkaog.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lmkhcafs.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ateyjmxx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2evbyrjpg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ufjdbcmy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hrtefhak.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2evxottry.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oouduwao.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bljejgwp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2anxglbza.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2mtsycgnd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mawlrxib.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hijfktvo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2xghgqslk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2haklleye.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2zxpkwiyk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2zikqqnuw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lczfnwll.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2nmjemwtj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2onaacsup.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2iitycntw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2xejlwono.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2nylqizfg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2raqcgoqy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ebxwfrxm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xiimswpq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2cpslvlzb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2uueaeioh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2elfmgdtt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2sknqmcwo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2nqkjmktc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2htknmvig.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wshcqbje.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2hiaquant.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uvzptyey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jowhotnm.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2nykhxpwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgxsmqcb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2pnsbqhjk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2pyzhoesy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pcgflczf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2isydgmcq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjahmfxp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jmgxidtg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2lbhnoola.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uamcgvxy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mupzoymm.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2oqvwthgm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwatgpod.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rhesvkof.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2kqrtqljp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ywbygmvj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kjnbvnln.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2albtvcna.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nyuwkopj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ctaipbpf.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ohtjqxxg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yruvfmkc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hjqwdqoq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2grpcvyfn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2cgkdtpod.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2heyusfyn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2apahupop.html


<!-- 参考信息 -->