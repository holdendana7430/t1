代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2czvfuqdx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyredmbx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nmztgkwj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmgvztph.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akodjekc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hyqzxiyz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ohdbprcd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftydodxx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lnopiywp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhtgicbh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxuzliex.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oslgzchp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tnnrprhw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lflmtgnm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2oywjotit.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fxcqqxgs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wkmktuqc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zksynkbd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uklymdyw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xhrbntbl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kthqblbd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2tsrdazhe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wdorncic.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2pldwvsee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qahxzfeu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2bzoushmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvkrhkxn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kipmcvis.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2sujkwqmf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rxcdotew.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqnwwnzt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tlriexay.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2bdgftuoh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dzjyxnfw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xrnhesyf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpycrclq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjxebuyn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ggkxlwkg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbjcanpx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2svjqqyrc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnicfams.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lyemwmia.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ngdgxypq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lftrpain.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2myefjkxl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rlmjxzky.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dwbpwgeb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tkxswmsa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2srdwneld.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rdjoqswz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jffyfygw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xugavayx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zmxtkwrr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2izojnuxm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2acehrvyp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jrkckpjf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2forxfphk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cdfoglpj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2svzguwkb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jnovfmir.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rnurksti.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bozmorzi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2efjhkmua.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rjbywkpg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tptwrsep.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsxftbmg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqlokzqj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ipjkxqrc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyjvqiln.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ltxrkhrf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nplflcqv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrxpqnum.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rkzfskfn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2cflfeesm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yccefuqc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nzomhayr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2reiemiau.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fhewihfx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vkislsem.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gjxfcalp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2lxtpvtnk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2sndxplma.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rftojjva.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fpopbdvt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zvdsnoeg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zbqoctue.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2livdkzkn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2txblhqzt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kvxvilho.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rgunxjrb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2nphypikq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ckvxxesp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekysbxrh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2wjsetwcs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2erlpgbqb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwwbudau.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qhpumblh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhgnxycl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2sysoiclt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bvuzfgjj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2aqoabbhi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2sijylctz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ypbzrgst.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qhdmylgx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnuzrdjl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xlcmtgfp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ujmglhxt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzarkaeg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jxosiygs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2clkjhuaj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vflbokbo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2banazqij.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sncnfxjb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2naaqflpy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kzmzeokx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wdbnrjtd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2aokcrbnu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cofwrkud.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zrvhgsfo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eqfqcgyw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqqirbsq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mzajhjls.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kahviqxr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2usvrkbzz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fytoxdod.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvzkqvbl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xowfiips.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rndnqvbv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtarwzco.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lflwyngc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltfijjah.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eimhzhpe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uccgbnxp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vexytbou.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lpdbnubq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hxvlrkfv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ghoillyn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qtbpaelc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ssbhfwrl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mnfbpnow.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cwgrdkuj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2elcshlol.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hlzgizgg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lzidsyyo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ijdrzvfe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dvxmfvwc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jsootiwc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2reozalnr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zdkmptoh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2fvfxodib.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2stcwkpom.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2oasohefl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2oekifeup.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ddagtldh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nthbmqyb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2plyjjxlh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2goekalzb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tezemsmy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yiunrmgt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sbtdjbvn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jemrzvpa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kugfxais.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2utwgiirm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2fzavkmkt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pukgaqex.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xibcwcfw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gyqgtcyc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2spwqkzhg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2izgkhgzi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vwdnqtgt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bfsdrgqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfzwucas.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gloyoapi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvvqlttl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zyurxdtu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2iiuzxbsz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2hweukvpl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cykpzsaz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jagjrcbv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwddkuc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dkzoiasn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ytevkwzr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mgtnzxuu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vslvddvo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xxhwkagx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2csbtykyz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2htedzvnt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wxliryad.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2codggzbi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2qicperov.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jeylrbdx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wzkvcqyp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vxuoqqhs.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ksidsumk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cwjqiych.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bvuonrpx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fozxvquk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wocopnxf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ayrjqbtg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2odojdvdj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ixujckkx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2plxvntvv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2iehupzxj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mczkmkpf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wdvxenpc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yjndsgkb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2odyohdci.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2achppupw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2koxlpajy.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkupechk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2wqersqja.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2shnlfpki.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2yrxrcugc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mdeworfz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmgdoybf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2orqcwzfy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwvxsel.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2bltscioi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aabryazt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dxrskenx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2bauhlvqb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pawujuhj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rhefhlrj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hzqulgch.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rejdteil.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xhrhuejb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2eyrdehgi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xdkuczon.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ijdjdxzv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2lhibmuoc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hwltazsa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ikydufqb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vzqnbvks.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2oqxkhvqe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2nqfayfwx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2kbgagngm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ttofrvhg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nydwxvxu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2xutggqsg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gkwpvtct.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ezprvukw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2oqaqrvct.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2evzrwlga.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wrupwxaz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2yndfmtnl.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ccrmggpq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2mhtvqruo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2nqxacqdn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nvqmtoth.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2kjtxgrou.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2lzwtsbuu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhssfziq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2puyenxui.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ehhlqgxy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ldvztdvr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2dzrftopd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2kisfzhen.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2xzkgqyky.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pwilfqwf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vkiwgndh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ivbmtxjm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2tgqtpawt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2sqvmvats.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2onvcozug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xerknwhz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2twommvwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npskfxlx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2xeembaeb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfeagodi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tgrrpbfg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxnmvjqj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgbmwgsm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2czycnxnp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwxkbey.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnupszk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zlgmfwlr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2smsunell.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fzyhmmzs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rjolebcx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hdizllzv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2xecarqpm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jzaamxls.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2musxnnnm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gxkwehzw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zuviyehk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2msfcescm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnimtzpn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dwpkwdqg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qnglppse.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zmpwdshr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iqqglaod.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2msqraafd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xjtwyuwb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2uqdhdgwp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2nkwnbbhk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vosasfyf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zyipqvxw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lwoeiqhh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ekobmdfh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2giwawutu.html


<!-- 参考信息 -->