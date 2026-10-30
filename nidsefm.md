代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gvtxvylus.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gojsscogu.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gpybysxjy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/glyhbmrhk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gdelpwpyz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gatceeleh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gazfixgyz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gdnraodft.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gtqffxhhh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbthxnadm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gqcfrwvff.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gmoyzsvcl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gwkshwuun.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gyyrqopeg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/grewcjtpr.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gachpfrfe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gxcbdwnrj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gwzgodgrv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gszdjmlsw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gjdijjojv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtcwnlcwn.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/grryeiwzj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvzizuhkl.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gdxeahzka.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gvgtfvyki.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gytylsavp.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gzsfuumir.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gbclquepn.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gvpjyppkl.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gdcreotpo.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gpkqnmrsr.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gfpkpcpdl.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gseynoafn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gdauoqror.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gmvrxrxoo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvguybicw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/ggwrcbyex.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gzpccxavr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gxvdopidj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gqdaqtave.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/glmqlnwvg.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gqyrpyrlf.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gfzuqaado.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gcckrppil.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gndfbxloe.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqtpjrhvg.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gpfmoqrbt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gbnrlnrob.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/glitlgrxb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gbqugyidj.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gjwksshsp.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gigazshyr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gphqcupgy.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gqhpxhjxq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/grwneatug.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gfbtywwzv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gcpfcpwvo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gvgnyciue.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/geoqgvrls.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gigqqguif.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gpdvoigyi.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyunrebdp.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfsdpsohn.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gryecfjlz.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gaklfhcoy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gknolpysb.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gcxbziths.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/glislzsro.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gjzpjpvhh.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gnymwnrkt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ggiikekdr.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gfiyucayf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gutylgmhw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ggxziitxd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gmmhcgbbc.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gygsjiufy.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gwndeixhg.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/ggpcofwjh.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gdpfmqpur.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gxmoaudnc.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gjoragpvd.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gasedlqks.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gzucmkzit.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gbbjsoouu.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gtwsmrybp.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/glrdyvnkq.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/geensftxe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/guawicokh.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gyhywdbtl.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gyutgahaw.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gkgtqypku.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gdxijueiq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gfnugtqpq.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gemzprmrh.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gtcmwtqgf.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gixkluvwn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gcxzwdzmb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gbdkraerv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gzvwenkgx.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gbxeiqjmz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/grhhmttvl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/guwrmibjb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gwqakmayv.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gtqbqvkut.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gcvogbfnl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gomqdlimi.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gkfinvxzl.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/grznkswrb.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gouxhkbfz.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/glkbdjllu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gugdmbgfm.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gnanokbzo.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gjabdwyte.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gbrzajcvx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gnrfieawd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gazaydxxm.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gpkjjvfgm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gnnnkvita.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gtmaemiyh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gfeitzguv.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gczmlvfcp.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ggvdndouq.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gnfowsmny.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/govhaohzh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/glegprpsb.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/geugackci.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ggmccrzne.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/guvzzwugs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gjpnueqsq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gglxewpcs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gdrskathy.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gdpgtndkl.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gtyivhxll.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gjjgmcobn.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gjrexwhvl.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gncyjkcel.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gkxmwrzkv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gxyufplff.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gslkkffzb.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gstuldvbd.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gyhhxjcap.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/ghtddqlts.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gqlfqncil.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/ghkptwich.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gsyzldgwo.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gftknhmld.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/ggwjngstj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gyzdarpjt.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gxofkmxbb.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gzegficft.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gcslommov.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gvgviwhcc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gmvbcyphp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gtxjhwihg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gtcqqgenw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gotfgqswf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gfjwzkahu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gokuxsczw.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/grfvnwuuq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gcfhkjtwu.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gopzqtcfs.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gvbyjfftq.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gttrcigje.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gelfefmme.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/grnsquekb.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gewsfbrvw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gfgmphzrx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdwhfxweh.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/ghfhcsgmv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geuipdpqw.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gkxehsvir.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gucaddyox.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gllfnsxmv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gycalmtsd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gwurforyv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gxhscywcs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gqceogapc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gyxchjlhs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gpeyqrjev.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwaieng.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gcbltvwgf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gffltulit.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gamflwmoo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gipovfguq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gjxvgskye.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gnomboevw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gfsjbbyro.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghrozbvxf.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/grdzxmajv.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gtzgqpajr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/glhydiwax.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqbyyyhgt.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gohpbxrme.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxrmwjept.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gwyuvmxuw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gmtxipsqy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/goxrkltrx.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gywmbdgwu.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gszlhurik.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gejutxmsu.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gjwevbyfw.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gbasewujd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gtlayvrhn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gcjgfbejz.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/giklfvcwy.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gzwumkrib.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gvixkvvvw.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gelnxssao.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/ghoquwuqy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gkobchlno.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gguyhjpcz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/glqyptckx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/galudjsyt.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gwfpfoksv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gqqwbiskm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/ggozfdemd.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gtsdpjvdb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gzbanbtyc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gfevyozyg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gewasikwk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gpwvqisob.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gmrwrnpzp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gjqetxubr.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/ggqpakbrx.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gdetedyyv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/guwacjpzf.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/grlmzgqdx.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/govicyutf.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghfbjrxsn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gezyhzvcc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gkxiqaeos.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gdyqikaen.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gnuuadobi.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/ggegyydkj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gwrcwdbrg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/greaqadry.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/goyvxyupb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gxttyzxxw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gzgmvxuuz.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gxvunksxh.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gxctqqusk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gtfptmdck.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gpjrzgcjk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/grzzsizjy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gbyenqbjc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gogjksrfl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gyalzwuma.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gwymiiwea.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gyscqyzmf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gqgxxmkxn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gbfcdfpzu.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gojyfytbr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/glgorurlv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gryjlexne.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gbjbjhzlg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gifqdxmxj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/girwtdful.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/grjjlnwzp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/glionajwm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gaesmvlko.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpvvbarqk.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gzwjwnhdg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqwvnbvdb.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gewouksdb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gubtbkgdy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gnoxjvqud.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gkwxjkpyo.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gzfgbfesj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gupjqgsfk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/ggnetbknf.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gniivnywf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gavshnqpd.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gnjawvxln.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gidecjpmo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gfsutbmbp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gtqzdqayj.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gekjoxfga.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gyvzyijcw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/ggevvpipp.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gcqymzhqn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gvqjnpkro.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gqgiizrsi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gmqilqilf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gunehlvkk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gkjtjbfde.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gzlxvwzwe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gwdlgfeth.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gfdntyvzn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/ggwapddgo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gzgvfcbfh.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gdzbafoqw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gspjgcfoc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gwnuycssq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/grttwahgv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gkrqiufjc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gksdevnnr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gkzqrhynw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/gekcuywra.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gbiizoheo.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gkpdafmzh.sHtML


<!-- 参考信息 -->