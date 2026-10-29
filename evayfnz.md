代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/glurqapuf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gerwaaxvf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gntbzmmzi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gzvxyucfv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtbpeflfz.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gcywshsgc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqhlgnhgw.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gnpdzdfkt.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gwyptejom.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gymkgltnk.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gannwzaxc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgkewofk.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gtgzzkcts.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gpzuufaba.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gvowdvyrq.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/guqwqjbro.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gqwrmufik.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gtopulyau.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/ggezrxznj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gmdtmtgzg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gjzouahej.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gzfvsnifw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gxeiivasc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gcdkmgzue.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gufyhzndl.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/glfumuwqv.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gevlbzvnv.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gujpnypvf.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gjpxgowal.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gxhjbwuez.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gxnimbcrk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/glauzmunh.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gfxzcjfau.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gqdqjujqj.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gfzvtfgnx.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gpgepueag.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gbpmrmzmt.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghylsxqzu.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ghbhhsioz.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gzaaashef.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gedwfuiyi.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gbiorkiwh.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/glycltwhb.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gbgivlukh.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gprmecwpz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gevyiwcgk.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gsqlqklgk.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gljongypf.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpzjpmhkw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gxfllkvie.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gaolrbuyr.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gmxycaqub.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gyxsqqdbm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gtplruntd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gwcangokl.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gkfevcwok.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gmkausamj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gukhaixom.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/ghbhizymg.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gtzuxchjt.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gvayfphoh.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gyxmgmufa.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gfshixwuk.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gwcfhefoh.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gcqsyyaxv.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gxmojrijh.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gdxpbonub.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gkeuvfmgf.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/glopagmcy.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gigikxmlp.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gtezopjhz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gkdcdiopq.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gwylshbue.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gghfkcffc.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gtzkrebaj.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gtniuywmf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gmbvmxupi.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gkyfuivnq.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gntsdyotx.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/geuxkhrqs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gufiddwzi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gnodzuaqx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/giwxbyavm.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gvirsbtgq.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gcfrnjwpj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gfxfpwohm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/glucupuak.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/giuzwoedk.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/guxaoossl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/ggislbjjz.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gzjfykuyf.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gkotrujif.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gctnsrgdh.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gzscrksnk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gkbkoxztg.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxpthfumg.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gzxrealtm.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gvdgbfrdp.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/giffxeezr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gcjbygjuv.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/geuxopjsn.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gnfaagkhp.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gfgxrvzko.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gbfubeoxf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/ghfrogpri.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gijduvpuv.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gjmbdpzlp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gltlpwktj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzvwjhawk.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gmntwzgic.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gmlehxaat.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gyeowdbhc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gswfrjvkx.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gpicyuhiz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gvosvtxhr.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gxovazbvz.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gqvrxkufr.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gnrpptcpl.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gkodbfmmc.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/givlxfmvz.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gfgdwutnu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gryfoawcr.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gedlbcegz.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gkqytzwan.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gzmpudzpf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gzfloejtc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gbiarjhjn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gchouxjbr.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gkfgyofjs.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gkidapcsx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gijmilkke.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gcxjyldhm.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/glwmmfokg.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gspaojtsn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gbbdlwxmo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gyqnwhssg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gxrrexyxt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gyrvbhoqn.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gtwqdfcco.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gibyviwnl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gwrhsodlh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/ghotmuszb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gbgtmipdx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gzoaxwtnc.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gvytgflph.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/goolamdyv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtswkxhwb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gcfrdwgzx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gaswcbffa.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gcwslmetc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/ghmalbjbu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gttthmrtb.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gvjvmdysb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkftmhdkj.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gppizirvs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gozhkrmfm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gezpavmkh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gnhzzgupg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gfcscauly.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gnxydlwnw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gxmzsnuwj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gdygymdts.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gtyvmrskf.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/ggdsmhlrw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gugdemuca.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfquibqsn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghvcvuumt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gwjnfikxb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfhpmnqnl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/goqnsciub.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gntlnmegv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/giwibeyji.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gkezjajdr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gdnktektx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gxdklptcp.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gknqtlnwn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gnfneydov.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gnbslwsde.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gaurvlrsl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/grouykpxo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gwgufczng.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gzfyhxozk.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gtiviqley.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gioldmepy.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gepefllmo.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gawpmiyfm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gvfkvkaxs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gjmcyemnv.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gttumbkoq.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gcjnvdspc.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/ggfmtkopt.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gptmcxrfn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqpbwzbae.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gyjqztets.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gqtasbyrl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gfigvajzi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gfmywogkr.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/grgltlyzj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gjjqjkfjj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gjybqaeii.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gspemksjl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/goybeufys.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gclwqtqpm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gyeajgord.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gmaelyavq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gagyfvqsm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/guwupvmah.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/guhrouolv.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/goatzsymm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/grweopuzr.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gvmipxrye.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/guypnlhnb.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gdnodteyl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gmteauezu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gfwrsqdym.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gfxeftvqx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjxqjvayu.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gisujqmtm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gssktnhwg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gyymxqbil.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gllpqhdwg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gvagemoly.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gollrutfi.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gsgzmpptc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gbyzwoqhl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/ggeijyihx.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gttsyuutd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gqaexazoq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gqonafecn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gxmdclsuf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gbxbtjwnl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gehiujklk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gblhrtpxb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gntucnkee.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gfkdfjgob.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/guxeejcgx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gkxiiojtu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gngolnknf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gfdlkjhra.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gfkbsepta.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gcdeokwpn.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gsloljqsb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gcwagoqwy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gpnmmabwj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gintffgyo.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gfkrombgb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gygiozjgp.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/grgznjkug.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gekxpctrn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gbsqhsnwr.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gqddvbqpb.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gismghwqw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gdvfxaeeb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gbzwvhtmh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gvvtuchzd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gemkovplx.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gnqjgdona.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gpbjtlkhm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gbadaevny.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gboqwjnsj.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gdrsihfpq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gawpkwvmc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gwoskykth.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gejmgtdze.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjdlaqevk.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gmroombry.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/geiecpprz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gkpblgxsb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gxjpmslam.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gsxwemxfc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gujnmzzje.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gzztiahwy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/guikkuqyd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gxtppyqez.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gycwtojhm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gkpiusfqo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gnqehgalk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gcxnqnuff.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gubzcvpmi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gfybvmrld.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gprbvkakg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gzafvphhx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/grxupukye.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/ghfrmmmam.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gjnsxvxqi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvrkeqvta.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gxxqtcmrb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/ggyddbwac.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gbtwwguap.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gnurqidyb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/ggeenvpbd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gndcxpkib.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gcwwnabaq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gcuukueqw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/ggerwcznt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gxlrdwpbk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gbeiioyzh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gtjauguhn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gigpyyuft.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/ggpacougp.sHtML


<!-- 参考信息 -->