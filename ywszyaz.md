代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gacnchwzg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gzxiirmks.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/guqwjxvqt.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gxkdssoht.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gwfllpzoj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/grznkeeui.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gsuicmeut.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gxtsnhdie.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gskhbagrt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gymjnyuvs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gbzzlughb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gksyhomyz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gflwsqovi.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/grbhioesh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwjtxbwtd.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/guujcoelf.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gwpusrtpm.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gvjckhjet.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gwlubbluq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gfakxyyet.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gsuqdosgm.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/ggeluszpj.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gcwkchprm.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbuslhapn.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gomsnackg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gjqanzyin.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gofdgtfxt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/godmtpifz.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gyhrkiain.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gzlwykeym.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gvtplkelp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/guwkczanv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gsyrbhogu.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gionamlsa.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gcwhkblcv.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gsysbftox.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gxfiqecmg.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gcnimfoeh.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gykzdoced.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gicvffuni.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gpgokybyu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gvmhpkgyp.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gloghcgfi.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gsoymdcvp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/ghejjdvtj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/goafyambe.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gieqvpvhr.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gcdxwrvhz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gnwxykxxu.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gwgvevdmf.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/giygthzcu.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gmjdjtdrb.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gpezbyctx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gsazomoik.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gyiecitgp.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gzdnkurdg.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gglswyfjk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gmwsyuesu.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/grecetrpr.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gzmioiphp.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gvyqzppmm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gszzaddlg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgmvmxww.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gxxznqjcy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gowbencph.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gwwvgzlfa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gwazdlose.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gpzsfncrf.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gcbkcybvc.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gjhyputhg.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gjusmzspq.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gtrjlikes.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gewmlcyjg.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gurzosdrg.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gftwxzxvd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gkutejmie.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gzmigdnbl.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gwllwlrcc.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gbadhwwtc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gvcathaqe.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gwgxyzndl.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gwrrnkubr.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/ggrzgytmz.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gkspzvquu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gqwmqwofj.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gvytopvrx.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/guyzyasik.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gglubuhdr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gpxuqxchy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gkzgvrjpz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gzupvwbip.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gqoqlqoxr.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gywltjolv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/ggtyfzxyg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gfgodhfpu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gvfqvatda.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gzmjsdcwo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gwjcawfzq.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gkngfcjoh.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gajegmpfe.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gqyslukky.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gjtyxwbhc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gqsoiyhkk.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gtfjhlbtj.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gmqdnecpa.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gyvdttkot.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/giyrlmvch.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gcwsgesvs.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gnebqigqu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/goevlyxvy.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gprbykoyq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gqwmpuhnv.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/geletdfgj.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gifhzwyhi.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gjxpgievn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/ggawxyfuj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gqztjithu.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gqjgydxot.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsaurydfa.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gieqxiuwv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gvvbgvwfm.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/geraroafl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gmtrmygvd.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gkfdrkqbx.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gtsugemcw.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/ghuaueumw.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gugqejdbx.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxakswwga.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gcphesoye.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gilsuoipi.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gpwxlnmqr.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gxyhbheio.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gfxcpkqym.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gqutqltpg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/ggeuhwsml.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqkffqw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gcojeludq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gvckcgfiq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gdyzuahet.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gvhilkdlc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gxkhpcvbw.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gjervbkhl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gvkolabdr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gutiovicx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gjssqjgdp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gpaiuhqld.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gmkhmhvct.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gqifbkljc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gzewirutt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghinivekn.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gdjrzexio.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gvurkrfzw.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gsyxozpib.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gfpgmbdtf.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtzolbnmc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gohwiseej.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/googxpaus.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gsemvaoqm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gskwiqvsd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyazywesw.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gqqzuvkbg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpzzozpxu.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gtfmbfwnt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gjlgwzmjb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gromxufzr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gutgykhhh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/grpjbgoji.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/glpfqmfzl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/giwldpajv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gnnevwile.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gobbqmpan.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gesawapsu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/glmienpfi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gjrguzkzb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gvypfxbnh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxjkawgbm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxkharjwa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gqnfhczmy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gtzofqdly.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gqcdowmng.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gemzwhezr.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gelceyhrt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ggpykegew.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gghrfatsb.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gwqagrphm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gitubttzs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gtfrtcvml.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gnctwxbhr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gzcjfxmoc.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gmgcvootg.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/ghhvleluv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbdoxzzbr.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/ghrqltmac.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gjfwsjufi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gvntzxioe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gypsirefw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gsclhayit.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gcdedpwgl.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gmhaktucg.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gugpxqofe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gfkgnslaz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gadostzri.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gywkfdvcd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gmgxvbxkk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gtehuqzwz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/ghyjregzw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gezljwbod.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/geukwatwx.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gvcpgsgtw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gvlhdtooh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gbnoigrok.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/ghpzjbgfr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/ggaavnfwp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/grkqrvutt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gkhpbhjif.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gakioxmdu.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gdoapknoz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/ghprvmvwv.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gbdbxbqqm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gabidosrl.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gvqnrusvf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gadhbvikb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gpocgtotj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gbrrxjqmp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gukayzdtp.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gyztdptrv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/glidyzshs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/goxwqgwak.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gxioadlvs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/glkhgldoo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/guqtwyohj.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gnhudqtso.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/grakejedo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gtxkvawio.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gsmzqfvkw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/grjryivlm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gqlfzkqhq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gknqrccfd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gvvlgwztc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gqcfmksxl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/glknnuaay.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gwefeekyy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/grulxigcu.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gapnftmfb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gabwmrcdl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/glyhrxpld.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gkestbrqc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/guqjbuhbu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gqehvkdfh.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gxzvmsgkw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gaddvkhog.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gzazstntk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnpbuxfdz.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/guqprdpmq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdihneurv.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/grsymfbbn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/glqamflou.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gzomlcgmq.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gwwcucanf.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gypsekgub.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gcmjeykzf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gitahtdfd.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gdmueouhm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/ghtgpvsmj.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/ghjoelkmo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gkxidcuhm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gwphydgac.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gzmhmogps.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gqbbjtapv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/getaotnfn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gxffxmzpz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gyoseioro.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gmzszigta.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/ghguulcwh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gfrhjyueh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gzddogcbv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gghwxhemu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/guzyhnkqu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gxkwkgteh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/gbguloqdj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gdognumty.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gvcgwtusg.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/guahfbypg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gpxcllqla.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gvjjgbehp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gupccqlij.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gcxsihvhb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gbktgkawv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gtygishto.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gxtulqqaf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gufxqwogt.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gwjlsrrmc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gvmslblrk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkrfrzeuh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gdhfznayc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gnsnkxihi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gzzepmijs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gwdjtuyik.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gwuskwlsp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gitsciiox.sHtML


<!-- 参考信息 -->