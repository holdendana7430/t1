代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nigwlijy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vxffwcyn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xwvhovyd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbwiuuck.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqnivjan.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtegubbj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hpvbllab.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxeznlhb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3owbaqscn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmzhkmal.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zsfynvgq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pedmsfcy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zvrwzjub.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgzsyfyk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wwsalmee.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ndblgquy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bhndcwvq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3seegbktx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3zysrpntz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3yvilcwra.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ftqvuefu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vwmgwptj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3fcjzwwnb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rqxloxpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtrutmtl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gdaofynf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdfwnbsh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ycyfimjy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ylmafipe.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3iiisdmuh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cflziyol.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3abpevlpf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3exmyjqmx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3btjbcwxr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qpjxpnzh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kmdmnjjp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujnxbomi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3muddyson.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydrauwdl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3moajlbjp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ibqfvpbg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bzuiukcl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vrawjcft.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wttlnsef.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yhtlvrml.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3usvvpyix.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3olmhcyiv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uzvwqtyn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mkjuskcm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3sswxnlta.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3eomvnjyf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nrkrelss.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bdlscsjw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vzuizxuv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3faejmjdq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qobhioko.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ghrhyeax.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pcfrufvw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsskurap.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rphxrsby.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3icgyahij.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pxqbuupm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bofopjzu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3eriyarig.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kcifyjum.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3itienlwq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmakxusw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3essfdzir.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qnxosxvi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cuajrtjs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kintxsag.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyvitxbe.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ogknfhep.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3roygagxf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ejpfoivi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qflyewvs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwyqexwe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uagtdnbx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ahnqpdoz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hpfjojji.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rtzedubk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3guhurlfa.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3yhuekvhh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xptsezls.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qirkxjfc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wgzyeksq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qadntlzq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3colpixcf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3qfsmrjzn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ghbzwyxp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mroxotkq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lxwncxpw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pwgfwbfx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrvrwtze.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ofywdojy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kihsqkiv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3diiwngzn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3teuqzynj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgnmvfly.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zcklxqno.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zdksvedh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3lnowceqn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zuqrvppk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzauxtlc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtqosawp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bnhqpiei.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zpbtxixo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuyxajgo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ggpztavy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fvklhekk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xuemuzcr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3vkjpxdnd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sjseknin.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3plovjdzj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3yjsrqktr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3okpklpsd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ogeqraox.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qozcieou.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wgdwqeqd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oohsazaa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vhcoqgvx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjpgmvrm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmtxdlgl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ibahllwh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3nzbctrih.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dtagzino.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hgpprpvw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qiqbqyzw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjneiwjk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tkjbjddh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfjqoyot.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqgveyni.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vhsvowdi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ibiovitj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xygdvgnr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hgttiivd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hapkuxia.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eismsmda.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mbauhlak.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dezuscpi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uczhtsgn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qfbaeotz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qwvzokys.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gdrgcvfh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3iopviszy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3prvotfre.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3goikdkmx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ttzvnoew.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3litzmuge.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gluamjvz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dflgfpbd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hcowiwsy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ojixvctq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ofwrqddq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vqpcfrjw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mqnosxsn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hnwogbgz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ijjicpmh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wixvjeyn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wvxjswih.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bskosusg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzzwirqu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3tlpwskxa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fboangol.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3axnnhugp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yqyzmglr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ogpunlqm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vpahwdvt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xkimymbn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mbzkydby.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wrfegbyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vofojylt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kmmuxcnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgebiptp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fpscfsfb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ukumibhw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjlsgvnw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uneltckl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qoaokgoi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3sxjznjyg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lggldxtt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3urkfrnde.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3pfhlccff.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lnstkziz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gupvvxav.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3esxpzsqj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fzndrnya.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ruahijdu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cfckomsf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xpkrnhgw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dmswoztz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hsuafdob.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3neujmljk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gvvffrzy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tudrsxwr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qgmypqde.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3azunsrlo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nddfikzt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3yjxrogqa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3scuhqtnj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3waubbyyb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ukbbtcax.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dtmnqcwz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vvvgqwtv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3iocphfgy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3byawkcrk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdhejtwn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3simogfdq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wiopwxxh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ksykptff.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3kftnkvqr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3crscdjws.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3jlbwkqlt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zamciutw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzuzafjb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojymulow.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3sbhdoiwj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3sruowhsk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3miauvjwk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3gmmmpvsp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3uwznflgj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ucnqoifq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qzeashof.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kplbijpn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mzcmenxy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3atdwspta.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3vuulwzcj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qmkwbiys.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3nkjciuue.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3cqqqeioy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vemfjsyu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oovpppfk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uhjomecq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3paukeabu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3oyipjqgq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3lrewrmnh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dayoayai.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3cpxhgwou.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3yrybwkyl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3upwdwyga.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rczknann.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3onczzboe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3hbxrtkup.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lttrognl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ugqxyyig.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3sjtcvlrs.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3brbpavky.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3fjxjghrp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vcedwntp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ftmlmzcw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3jckajoab.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3olmvkhea.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3grvrzkvz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3scbzlhtx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3cytrcymh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3cinpdqto.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3yfczrycl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3irwyiucn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fbxdwdwy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ktmmubev.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3deutyqlt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3drvqjdbv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3zuzucvsl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bbgebnmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwzorjtu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oyimklro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdislncx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3qxntmeeb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3espjggqw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3psvqnmtw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3amafvquo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yrjqtjbe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3bojwueti.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3unyglktc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gtenmrpk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jomibryh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3opnpgtfb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fcsawddz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3qccpdsck.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3cxbfjtvs.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ieeizsag.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lehdxsln.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nixmrqki.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ljjpfflz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kfkhliva.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3fuqmodqz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqxcqodb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3kswaqrwo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ptecrcwp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3cigrlcqh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jkpcljyh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fuzesdrh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3akwtapwf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3fuqcrrcm.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3elzafpca.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xxxwvwkq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3sgixrlxm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pbbtnbjy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3thuaisxn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3adtwqbuc.html


<!-- 参考信息 -->