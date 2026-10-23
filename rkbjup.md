代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rawzaxfz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oydkdgeg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mubtdyay.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kepywgqg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3anvqirif.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3adyzouwj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ibfczbyc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dqadijem.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sutrbclc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lbzbtyix.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3whvmvqhv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xgvmztvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpfmxcqu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3eebncwdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvqjbeil.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jmewvllt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lrrtzwza.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbgfgoyg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rzucmwwk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiftiblg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rrsgnojn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rdkucjxp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3svzkhdyo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tdodrqqa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3uqbfzlyz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3vlryejeu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukahufcw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ljdpfryk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3umnuvyea.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wbnagqif.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cgwspwpe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3waumfzln.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyilvkbm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3lcwljuzz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oyfvwqqy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bsrlruam.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vnhkmmki.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aptxtozt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3yenfatch.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zslruqnu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lmranzar.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xzggwhyl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mdgbxgne.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tnllxmhh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bggluhrg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkkqgoao.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ejonfshg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtfbhkoc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cwdjblcv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uzjfaaou.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3psjifmac.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qkycjpqb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ylqmshbf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fypbzeos.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3knhwczrm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxcreczg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nfuhfalw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gabvisbq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mynckikr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sksdluhb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vadlsdpy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3upgtsuus.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3siethaoc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qmyqeqgt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tsxcwset.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eydzuilb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3plicctex.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3llfwvlbd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3oynxwmxm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3uleumxvp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qagqsiko.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ujjjtxjx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vxzqgaxf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ydkdgjzr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ruqsfpni.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pavbcdij.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bsammwdn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xxvdadtq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ssxoixux.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pvzmcbkq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbsvbauu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbjkohes.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ctnpoyfj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qldmnqlv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ydxuxotm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mgfdkown.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmrckjzb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bjsqrzxy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rpxvzqrg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkvzxgxi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3yflqybir.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ixelcotl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncelqzev.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3plmosiew.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vcvrvvod.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihlrvsmi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jgwhbbtd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3pfsanlfb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3acmkggil.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3gekzhvwo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lfenzthf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ryfxpleh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3btgqogsf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qdjailbj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hhjmqnxg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ibwdakba.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rfqhpwbu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uzttsguz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppncuayv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bthdwbsp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gwidlbcl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uquxcfzh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qlbsocea.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3oaojlrmk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vgfsqjqa.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bquzscdg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cmrfgtdr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3soxwaekw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xdtkxicu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zxrqceow.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oruoxpta.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gdpzqyzt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ftiuhnpx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bvleuxng.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ewvadjmg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gbwaymbn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3thqwntoc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pvasbypv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hfkrmehb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3pumcthqz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmtivli.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3zvobnehh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zpuupszz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3kngxlazp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kzklclzj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3yoprtlai.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cgtrblid.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwfqlbes.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gjedbcfl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ysfudkek.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ccoyrnmt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xbkbybcq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vcnqiwhj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qcfkagxw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qnqtpesq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wkcsfdvn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dibnnbwk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3onujpdgf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3cebtiriw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lldrvesi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qtuahaqf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qbvnkipq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hoomnwsr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uqbsownc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rdayogcx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wawehfof.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rnokkwmy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3fqtmbdni.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3canrwqfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qskofgyv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3izsxcatc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhzubgri.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dpnmqacn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3lillawxx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxyghlxr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ozxwoftj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yqavzzul.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3tjupncwd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3hcymucil.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jvdeuemk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtsbzmpj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ktfcujsu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3vqttpivq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aiafjxtr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpryjkek.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wfbyqivj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lgzeuaxi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3uzxjdsxh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wlgfdfzx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zrpbiucm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jnvzdkyg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bgohyweb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fcgrnqyu.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uvijddwg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tuenwyxc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ekjpxsos.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3vftuvltu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3gntjqjkl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jzhekvqs.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3wzusdrmi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hqpzclba.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xclplnbq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehjrndtc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ndkyaphw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnpusbwl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3uhlltnzd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3yohscpng.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3punraiuu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3krzgtwin.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3wugofxfi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3idfixmau.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qihvxbxz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3onksjgfj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lniwmcpe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3psatziin.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wxvuaago.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3zwwkebyq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zzrlbgpo.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3usghkuij.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fnlyyltz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wpinjcke.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qyldccqx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3fhiillzc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zhuljmas.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hdhidvrn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3fhadyeen.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3pbbaqtgp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3dqsjwile.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3axuadkrl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qghygdkl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yeqxcobm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yiysnncm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3zbwljjfd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3klyrsofl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aipjbxij.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3cmvnfqtx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3alynzndl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3kaxaiyuf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wmunlkgq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3jzlfwjyi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3kkujjpyz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ofaaqpxs.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3bkdgtdxg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ydzaqyee.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ndaxhadk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3uurorqyy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ewxuuwcs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3aupayqsj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jlolgwqe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3efotzvli.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xpelirir.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pjrqwklc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3tjaliooq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ftbiailo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ticrqvik.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3eskyzuib.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gwrrnhqy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mdvqrowo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lqoanmse.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3kwuifwmt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ucerfbrs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qkkalufm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyqkiiuh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3rzaikfsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qokyzxvl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3yofvgnwn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppovecka.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3btphctut.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zazmokse.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ruaqbpuy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3vyrmefco.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqbukemv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3yrtvmwqk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qwloumzl.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3nkkdkqza.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3euzbmlpf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mrexbhwn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kafaxtzk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cjgmfbdn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3hnulllte.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ruyrigtc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dvalqpbm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ceetebjm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3xoekekej.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxlxbgbk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3axhovsun.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pmmcxcxl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3agxmturk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3blyowznd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3tvjpipgm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3moshsclv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3esjwftvs.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3prenjuyc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sdicccve.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jcymddzl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3avpbxuuj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mxjdvett.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ynmzsapr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3azymxtqq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3unxfiuxi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cepivwpp.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3iycnvaqr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmeftzti.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cwlbvirb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rugmcawd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xfpovgpj.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3zetgelnz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbfnyhnm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pnsjiaof.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hpxthtbg.html


<!-- 参考信息 -->