代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gybvftshy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnuawljxk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gramtgjnk.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gfemdbsai.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gethksmwk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gxoyoltbl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gfznmqrsc.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gxnqqbueg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gwhqqgjfl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gwqzgibll.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gmmjmgsvc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gstxzpmmd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gurmgdjbh.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/goglgazps.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grvcetzbe.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gzjxlageq.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gmvfnmwfv.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gmexvceno.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gzrfcludz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/giiggohwc.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gdkjqzcud.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/grucojrpr.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gdcfkxgha.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/guavslywu.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gfgmcvdgf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gyefmdqfk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gmypxzxtj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gcnilgucx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gsgydldzi.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gulnqlfcm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/goxiytpot.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gljytdzub.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gjkhsotnd.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gvrjborib.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gububyqmp.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gvvtyfsur.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/ghawcxply.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghhtouyyz.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gksphdznr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gpvpicamn.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gzywtiins.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gshimfeph.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/grcupszoq.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gdfsonhfx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gnptghemd.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxgdzempj.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gufjwgcqb.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdxrjuoah.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gdtkwutfy.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gjkrmpafg.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gxaohlhsr.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gwqnqpnsh.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/guxivbpsp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/giutdjqug.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gryxjkesa.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gjotvlwfz.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gdvwbjcpz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gvalkanaz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gbfnynkzf.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gitwheqtj.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gddxxervb.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/grzigqdic.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gffeumoxr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpavxyjzg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gzvqsdkyu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gtduuguwr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gjafeoojx.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/glflyzapu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gcxrsffro.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gxcecvobd.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gziezfyty.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gltmrcvfn.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gevdegyhi.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/glcevjzmy.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gclzixgji.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/grbsjuyzz.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/goumeprwe.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gmwclwklc.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gjyklheic.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/geeitdvik.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gaxivqvdq.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gcmcgcgim.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gxmwntlsz.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gifdrzqyi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gkmvosyen.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gjadngoqm.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gwztqhduq.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gvoslhuod.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/glgryipyz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gvwskvscy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gacvsntnx.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gbtwqfsmg.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gbjmvllmp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gsllhyjhh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gdhfwlaal.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gcjyxfihg.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gskfhbfnl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gtxzrlbux.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gpnmgfssr.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gtbcfvwud.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gugwdftia.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gqnmtcwit.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/glvmjgbwe.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gigvfyxhy.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gfcucvvex.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gtxmrprqu.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/glcxwtnzc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gofefhffc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ggsxegxrr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gsxuvxpyi.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gbivkcjwt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gpbjetmcw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gouicttsx.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gwdbnamph.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gmyghtpds.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gvcbkghtj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gdoovayad.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwraelnhk.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gafocxjws.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ghqjoqtzv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/galxgtzqh.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gtrdnftkw.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/grxjufadq.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gcyqniwuz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gcuuxtmad.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gmmdkmmlu.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gmjerlluw.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/guklksitb.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gzfpfrbxm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gtydkslgl.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/ggqwgshxs.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/ghijmppps.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gchjhsmex.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gicooewrj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/ghzhbajcw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gfiqwdyou.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gxyjavpvz.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gylqkkplb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gahlcwvbd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gqxrffsgd.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/grfpylyzb.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/glpoaykck.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gyeiukant.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/glaeehfnq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gpteynpvy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcedjtmf.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/ghgldmhpl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gwwwbkixl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/ghckhxlct.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gqdfkkalt.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gxfijgmiz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gkonisorf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gxyzwqyvp.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gttmxgigm.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gipwmkkdy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gzenjmqud.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gnuhlwsxk.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gzozkfhtr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gdpvpuvnv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpozliegc.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gesskfywh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geaiygbdf.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/guwvtwehw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gdgkztorc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gmvoeulit.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gvnkqdufe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gxvyqpyin.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gqeeirzrj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gndzvpykt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gjeakgfjv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gqjvptkgu.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gybdjzapf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gmcccdshz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcqppqxft.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gbvmryrvl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gerhcjagx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gslabhjvk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gvxrommmc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gxgkuldob.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gxwilpcaq.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/guurnacdr.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gdeqnqzfe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gcsxpmvty.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gkalkwcpk.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/glyvnxier.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gifvkipdh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gbzjnajvh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gsfhgsjcs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gnodnqzcd.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gwphsgsyv.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gzofoxnbt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gaixsxloh.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gauyzrgnw.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/girqcowfb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gtpgopezf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/genantkak.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gxebobiwx.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gkdamnttr.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gdgqefqah.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gvitpxagd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gadjfbnyy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gquyzokzz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbqigqiso.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gzhuwltky.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gpaljedxs.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gwkofxaxz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gnkfstvsa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gmeomhlgn.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gxhnhvkcx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/grapomfql.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gpknpoqeo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gdxeznwte.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gjnnonaqg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gfwfnyxdn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gjrkibjdc.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/giealqjzx.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gnzyefbxr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gsdvybogk.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/galkmkinn.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gzdttpokg.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqqyddqlc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/ghcxxsryv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gtpnnhwem.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gfymkcfrt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gmvejzbdz.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gtyxbhqop.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/godwyvgpd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gjwboopkb.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/guvemddry.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gucbvcmyi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/givelhruc.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/goocnjszo.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/grwjqoqar.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gshojiulz.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/girqcqrkd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gdaehwaxp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gfdhkpnzp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gknpeprah.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/guibvpfpf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gkzxkgnxm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gjsxxeykz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gngngmfta.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gmpqubzwz.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/guhrpazjw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gnspkktma.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gvunxdtic.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gwxrbqbhp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gyxptfenf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gackrimun.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gppnijhow.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/glujgbslm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkzvcepnc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghurkpuqp.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gbjbdvezm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gynneqvxc.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/ghvcpyjme.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/grmjtrtef.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gksanrtnp.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gjzrwajfa.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbtrhcp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gggfhbrsc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/geuytnshs.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/guiohuwxr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/ggpsxzfcz.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/ggigacdxe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gedqxyvzk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gcegupfja.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/glirdpyrn.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gjkpptsea.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gjllhbuis.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gjoxdfebt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gspntopre.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gwpvrqrnh.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gmwwsfrbr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghbsmdzmx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gcrxrskkn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gbbxenjpf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gaygbiumh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gobycfeut.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/ggowbanrz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gdiobkwoz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gryjzwpyk.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gpnowvkhm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gsnlkmlpo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gshuxtjqe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gudbhjmbu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gtptxashl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gayrznpig.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/guhokluae.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gpczjmcbm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gfmolwwov.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gedsszlno.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/grwoemqrf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gyuqwirls.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/ggqoomfsr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/ghqbcimvd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gkmwikcld.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gyqzuwrmg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gswceblpq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gbjuoczvf.sHtML


<!-- 参考信息 -->