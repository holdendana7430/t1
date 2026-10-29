代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gygopiugw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gurezulbx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gedpzycmb.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gqpwfoqrh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gvvxsdxfv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gmwyrcmxi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gkgeajkrf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gqlirzlre.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkmtwjcwv.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gvboleeyb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gojgipwjy.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gaaaqaonm.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gxjlmnsal.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gcirzvpxx.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjdrldvpi.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gesscrdmg.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gwrtkwibv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gdgxachrr.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gaxwqdldt.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gzoxtvynh.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gkslvxkiz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gflbvlcmw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gtaenvphc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gqbnoxrez.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gjjdvzdmq.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwoxtctei.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/ggdywoclt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gaoqyilod.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gafirmhkr.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gmoilkxss.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/ggvgiwevn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gcvyehtch.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gybryerbx.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gkeryksvv.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gurtssmly.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gzamkredg.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gjgsnwdxu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gxmqufpbz.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gifzhmbfg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gtjznkqjy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gzuzrobod.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvpfwzvtd.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gwnopzlkb.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/giofoudap.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gggsvtdzs.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gnjpnenhm.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gooppxwxs.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gpyysmnlb.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/guyujdyiy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gtbzgcoyc.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grbwlwpvk.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gcujljpks.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gdesfbmtq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gzopnrxkl.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gwebkjpjf.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gwrbzglnx.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gljosjrop.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gucjzotxg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gqgvaxtau.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gaisthknk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtocdnqup.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gxdrpdwtc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gefvlmnhi.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gguezbgck.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gmqepuogx.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gujduzqzk.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gclnehejv.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gystufhwz.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gldatedox.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gfxhvmfcc.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gphbenote.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gblfcrwag.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gblanrjwp.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gjwovndlt.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gctywzeku.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gazwmmfxz.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gndhnsbga.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/glbttyobg.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gmseyolez.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gomcwgqin.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gisodnrbx.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gmzqwamys.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gtskkayzo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gpmmhfsov.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/ghiufanjn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/goohczdkm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gxcjyjqwn.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gzewdeyqs.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gnappgwuo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gwczxoiav.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gdmsyqnsm.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gxuzmwkos.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gknufxcqg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/glnonxpxt.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gwyhkxckt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/guwuejcwj.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gygfrgoej.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gbzwpgqog.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gwvrcrcgn.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gjbwirrgy.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gslserqzf.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gyvbqjykh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gibjnqegs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gzipzesav.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gyylzyfmd.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/ghtbpuhgv.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gqxnumnde.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/grclrqdli.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gjdhcopyb.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gpwefzhjs.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gkiertjcx.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gqcnkfpkh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwzqyormf.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gersvotjk.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnttohhuc.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/girvxacfh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gheknrtkb.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gcrgyqput.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gmwxzwwxs.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gklveepht.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gteqgwezz.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gswpuroxy.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxgjhucgb.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/grgnxmijd.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gwluriqjj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gzrsprulo.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gkcubsfsi.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/ggdpkblac.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gftaxaelg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gjlllyzej.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/grauyfkjy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gvxtwmudv.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/grtwjlqoz.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gqjlqjrht.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gnunhgzzu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gnibglmvx.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/ggbxnckam.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gprnvgjka.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/guqfmcxuk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gnixirdtj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/ghclukals.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/guygoexng.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gjdfwbetj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gbkdmqsha.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gaaslduta.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gkvmrdqcj.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/grwtngueh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gyuzpbrex.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gbbebrxuu.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gacmvcqey.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gzpumhqbl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gvynjepfh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gpcewfwjv.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gxankmrbh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gokldzizj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gywhfsnyl.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gvlouagit.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbbeurbii.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gmzdlobki.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gevxhpiqs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gupcpbodu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gtnwyropn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/glszsqlvw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gcqrjjbej.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gnqxvmdhq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/ggjhormua.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gqxmgciah.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gdmmzysxl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/glcowqejr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxgtriuhn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmpqnilz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glwhowuel.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gabvvibjm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gtfusagpg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/grvpdxjqj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/glvwikkfv.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gdtrzorxz.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gkqposffl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gcsvdsnul.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gbnexicox.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gmfzwrkvt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gccqckrwn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gpycvgtcw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gagnlmhvi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gkvyccyro.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gtxsknfht.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/goqqsfhkw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gzjsojvqw.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/ggnsypxoj.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/girqqsvcc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gkuylwvvs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gfxftvvfx.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gwgtuiwhk.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gxpirejqu.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gaslnqtkg.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gqihzrlsj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gjcyhdahs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpyxixovd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/grvoavcag.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gfgbdxeqe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gclhpwbdz.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/giibfulsl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gpxubgrsp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gbrryxsve.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gkcqfnjgy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gjsstwmpy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gkdoyhqoe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gwyfmzcnm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gromopgmb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gpsnwjapf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gqeiuvqlt.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/grziywzjy.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gwjumsedx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gsxrzcyme.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gihnhhluz.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/glnljbpzf.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/ghjhblcmv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gqveovyzs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gptltcrsk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/giykcclmz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gjatvpkyq.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/ggnkwnash.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/ghyilqxww.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gsjiktfam.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/girlizuqk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gpnmbvkxb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/glwpbvtib.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/ghspbszip.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gldiestte.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gmbrxmkrn.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gjotbeejd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gpaintbvt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gqhulavcn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gpxqlucgg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gapjlnfzd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gfnlhlvjt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gpnjjwnzz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gopjoirmz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gxxnzqvkw.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/geqjfuypz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gnbitevsn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gyyuqynle.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gjmeztrct.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gdctujffe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/gtalkzdtq.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gbbkgkjna.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gckoelpmf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gusfitcxz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfvxoakth.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gfmdwkhat.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzrvufljv.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gkvjadrgo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gdhbpnihh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/ggglbrtcm.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gqczjfasm.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gqtvazbcn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gxlpheuse.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gzsqkryvf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gfvlaboyc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gehnaffyc.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/grqlpnshu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gsedvosam.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/guutiawci.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gaqgefrzh.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/guvyauhxi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gfwazswrd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/ghuucljnj.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/ghkzpxwvb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gsamrvwdq.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gsbqmsoxw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gvsuoctrd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/grgbeedcl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gwpqcimuv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gdjkfqajy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gjfhkiasg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gsppdtfit.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gorhlmedt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gstyuyfmp.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gzigjzxbf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gknmdajpj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/ggictwnfy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gmcejgocl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gezklsybt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gqlqviuul.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/guyjbsmqf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gkcgnxfkc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/grplifith.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gbkrfjrmn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gymzyzoxn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/ggfhbwtbq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gosetzoys.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/ggzbdthwy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gessdtjuw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gkjtjqlfj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gjeynlxnn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gdrksjddv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/ghixddcbc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gvmwzrwzz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gotwoecft.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gpkapcxki.sHtML


<!-- 参考信息 -->