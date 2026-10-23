代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fmjqwytv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yulovnxa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rqwiyalj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lusfkdiu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3oocujssj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wsgmpgsm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swuzpgot.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wgekjjnb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbmebonu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxwixbmn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3meiltgka.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vcbheblg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eoqrbvvx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnymbpix.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3znizqwvq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlpoxutf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3sxfeiugk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gohrxgsj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwtwypeo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3trjvgacs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rjovszfu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcaynnvd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3daavouqk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ytrzabpi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3aypsafif.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tkaoglos.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3iniskzoc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3edfjeymf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cswxnnad.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3yhmaxrva.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lyakhtam.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vcovxrno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psgsmnkd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fojywiep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cudatzsj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3khbhjqgh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uqnmbzll.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3holktlfj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygeerjaj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3onuamsmq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rplemmnt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3oiwjxbcq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xvkjyrvd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sxinpypi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ydfenddg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ujoadyxv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbqxggta.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rojweuny.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kxxehbpe.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gnrkprnq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wehxjewm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3scakpyvf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bakwgagg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xtoheazh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rfgydxdf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3szdnrhac.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3skmbwatp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3spvhdrkj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hdiyaqoy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rwjypujw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pqsxapiv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wakrkgnf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lpujbjcw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kisltluc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrrgkunp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjgahnel.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cehwfdtu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rrzkyiby.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3knupzdjz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pnwayhsq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mfauirpp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ahgisobs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rmusbiwd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyvaysle.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdsehnns.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdofjmzi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fobebpwm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ylbgtysg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hdzagiht.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3sxuuxktj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3usosvqwb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rjwqfvlv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wegetvgi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qstwgrnd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3birnjpkk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ssghtdur.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nhjhbbcz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ophywzik.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ozihjgwr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kmbjqpfy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3iwfkchmq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3brycywdu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3braepfuz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3klscuapv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3whpwwdyo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3otcfuwcw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yvjozwhb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yjmrwktj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zmvmdoth.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tpqehlda.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3smimvyam.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3calirwjh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3erafnwgj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tsptluym.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3fikqkpem.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dmesvsif.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxnegzcg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3onbncmgl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ozzcsoho.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kadtmonm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3bnsvsmha.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3guxdzwhe.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujxcphuz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3cyjnzrbj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ygjufxwd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abgbfysk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3yamwcevz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fqaxbzam.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vujbcxcu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jgpcphra.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qfdstbby.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hyroxdkx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3slvgbhaz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ymyezevr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3rrptfhlz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3baigeczm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3vwvigzpc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcthxrbi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqlitisu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvddnccs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fbqbcsrx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jlsrvgoa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3lphfexco.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pelabfup.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cajiflpo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lyzavcin.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vccawhaj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uxlxdrtm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ulheaoqa.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ayuvnzco.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bonkbsrb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lyarxwjo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ofaaojlf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3yffbnivo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ppycqfgg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gzazkkgj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xxfblmas.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xkqukvzz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bfefxyax.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yooqzjon.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3lffwulon.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cvwhppor.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3yngzngfs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mibcluir.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3kjjnircl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jsznvrwn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jtqrhyjo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuemhplc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ivqsjvbr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3apewtwfb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bgataetr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nstzrkzv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3szcsnnia.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3befzukdi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3sorjqypc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hdubmlze.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3wsosdpdn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3kmalzvfa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bqmncudb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hijhoxkj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ccoeqith.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cyxqeusd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3eakhgulf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zwqpeedw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hqmfxtjl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ztlgfowu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3uwfovnzo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3aavijbqe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ttmqzvjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrgpnuvf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yflgaedv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpsehkbl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fytthsvw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3eeiybgdj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwweyrtt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3elbcqtdb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3shflnivj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ofqxsrvz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3fmnmyjcn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lygngbmc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjxyunbz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ypkfucne.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3igykyoaj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xaaignis.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylgpowzj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wxfvbcyp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lfhoaztg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xrnaqcyk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3hmamlfma.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tqhxpdcd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rwhvxevg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xsfnrwoo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eyrrdnjv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dxjctdac.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hilxljxo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xkpndlxu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jebiwcin.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qpbnuzxb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3affahcvd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rlicxgrt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ujmlfekt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cyrjtsru.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gxktztab.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3sdqzkkeq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pgjvlsup.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3afxzdkek.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3krehsztj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hlgtzdev.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wwcvwahk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vuauboiz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3oiayyinu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyowtfas.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cvkxpxbr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3pptenqyz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xolgwtsf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dpsmqrjg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3dyxxbfzp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mextkcpc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3tshkublc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3beffoytu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jvbolzsr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3haswwhue.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3obilpddg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bbqdfahn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3upyxowlb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zmgxjamh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hivdkutv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3mzloxkte.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3elmcrhyu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mzetghqk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ypemgzat.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3agwaqpxn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ajflqbqs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jnwwsaux.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bijuiebx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3vggnasuy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3rtooyrnv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ktvnzssv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3elcqjnqx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ktrjrotg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3vqbkvobo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3vpjazxmh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3kcoezudf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ufjogkjv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3epwyloio.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3qqnhqnig.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yaoejjce.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ekvdrweo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3pcbbvpmy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3rgglxaqh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3issoqfym.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3rrxedtdg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3bncxipid.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3pnulmwaa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3kjbjnauw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3cdmvaccc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fbcdbvby.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3grtnjnxn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3wfdpccqm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3iqxdbrwf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3lnsaibry.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fxsrukkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pogyhqnp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3seavicmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzebnopd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3pofxzyzr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qqfigrtc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3osyartjg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rrzjzdkg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qsmjvwyl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3apdfjrsh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3lzewkghg.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3shrvnhsu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hcbgcuma.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zksydivg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xouevjkx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fqitfixf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3inifukfc.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3fbzrzfvn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ohfolwkv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3agqjfhsz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qntdvlpo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3susbfugj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3xdjenotz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ziaamimr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qkpoyspu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3quifpmvj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zxkuvvrq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pozclpbn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ryxpkney.html


<!-- 参考信息 -->