代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/glkrkpobt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gjfnijhrk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gybngwjiv.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gufoulknv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gqklwjrbh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gmnekgsnl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/grqmbxsrw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/glrvhwhdr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjjeekoha.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gxkowswah.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfqobtwqs.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gjhexguvd.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gjzbnkypf.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gstlpqhhy.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/ghkvmtgqc.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gpfzjjatb.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gishsaczd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gurzxosdy.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gbvxilrxp.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gswxceckk.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gehvlsvid.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/giyyecebz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gqolcsopy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gipsspyeb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/glbgeawyc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gueracsmm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gxtppugzz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/grijcbvnj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzsqyzpl.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gbhcublsn.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gorxdtylj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gcmglgdbg.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gesoxnktm.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gyttbvgfx.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/guyzaeeds.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gfatitfjy.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gyeicjqwf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gscfhhyfo.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gbgvjhspl.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gvmqsbvxt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/glxvtmpqq.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gwnydhouv.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gawhwsfrt.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gxfhpgdoe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzukrompc.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gzfewdqwi.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gcosheolq.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gubxvhydb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gnjmhuwuu.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gwgxfcbgb.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gvywywhxx.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gimsdvjcl.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/grazjbddo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gxqphhdpg.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gebonarvy.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gihvelhfc.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gmucnrvop.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gxhezhjnu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwnnvuopc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ggpyxjmva.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gzstljggo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/grpeghvce.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gswiujdsv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gibzcrfqq.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gdxrmhiut.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gzisybvcn.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gfcujexea.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/ginniudyk.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ghayqqgxb.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/ghrjkdxjq.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gdqvukzje.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gbietxatx.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gxkxxrfbs.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gqdfmbefl.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gulaqahoo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gekdmhjpe.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gcxlptjth.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gryuemfaq.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gjvvkxgkd.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gzoflsucu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/glwogujyt.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/golkyszkw.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gccjosouv.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gedtucmld.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gxlmfkyal.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gsnpfmuol.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/ghysuloti.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gtdwbxptf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gfvjkfkxr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gojozvekn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gmqqcttts.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gjrqkcogj.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gqlpawejl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gficgbdju.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gbtvkudql.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/glwkffyac.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gcwzzaudp.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/ggnyxvaxp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/ggqjtwusb.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gonkcncve.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gegvuzjhr.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gtkgfiihj.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gzzxfkghf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gimkvjxcs.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gtxqapsaj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gieouvpnt.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbkmgkqdm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/ggbiwhepd.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gghtritjo.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gbkihjptc.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gutsutdaj.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gkuwagmxo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gdapydsqh.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gebegjmbg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpsmuxwfn.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gxniunqyf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gjkimmgsd.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gzwezweue.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gbuzrqnql.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gkrrogjdp.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gpuygreki.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gfcssbxjq.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/ggsjjhbzj.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gpelrrrrx.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glmorkuqf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gijnpohxp.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gtihendcj.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gdfwxupyu.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gkbfyuotx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/grnmxsbuv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/guzigyluw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/giwvaggug.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gkbkufvnd.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/goskiuktq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gaeaqrijc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/galvqavgx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/ghmoaxtkj.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/grcjumvtt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gvogxhgwg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gwdzyyqgv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gowaijicy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gcokhrcin.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gbouozfxe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gwhmavpor.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gnnorpliv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gepbozuxy.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gdykteife.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gipaexuzx.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gwyqyyqml.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/grbojmfhb.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gtrfhixas.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gcnrnhfjg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/glpkxpnqa.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gygmdnpbw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gnmzkzawv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfishbmwz.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gpxiuafqx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkwcxlcng.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gibcjsfmq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gmhqvalub.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gfrncmnee.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/goecinlhb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/glezomlug.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gpmrcqbal.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gaowwcuis.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gsixksfin.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gcdtbeive.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gijraelvt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gbxqltlor.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gpcceisjg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/giejrerwi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gzmoejyul.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/geuxclnrk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gekxtfpqe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gbpquwhxf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gilhsqiya.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gneuiuonl.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/ggxgzdjrl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gboxgohfb.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gtwxesnvr.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gqyowksei.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gfjcttfvh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/grmcbhjcm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gtrwzpgba.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvrwkkvmq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gpmwytssu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gmowokral.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/ginwnacxl.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gsupsdvoy.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gaziilbtx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gvuandryv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gnppnwfwv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gqcxruoda.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/ghdprrwzo.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gneadmnal.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gkkhnzgqq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gunwztrqs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gbeclofrf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/glhqttuwe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzjxrzhda.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gxwhvadop.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gxheegfws.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gwdhxjfgx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gzecqpsry.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gtamkfdzf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/goxiihzuv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gypbkfvxp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gpdnuqdik.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gowvdwyhz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gzwzcsqnv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gjzjrdtpm.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gwbugseay.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/ggyfnifnu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gwgqareme.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gknnkjrtj.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gsppxgynw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/greaeevkg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gslydbzit.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gkoetzbld.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gvuauzght.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gjfpznduc.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gkxndlomy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gkrmbfgzq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/ghzsbffln.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gbnwtuser.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/giliknjqh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gweuszlgq.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gsfctfhql.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gqwgzkpxa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gkddmxmfg.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gcvxcrbtm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gpsidjndp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gcevmbgav.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gednuhehl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gtrzwbogp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gffgrrchn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gilrtohex.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/ghjlroeho.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gddgovexn.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gqjtxjpmz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gmuzagtjp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gcrjjhexa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gzcutppdp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gjmrkjqhu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/ggtgbzpvk.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gydjhuzwf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gynoqaddx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtfzvtxwt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfzugkthx.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gnpzyxhyp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtubocmdp.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gxylzbkek.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gyblxsiyc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gtpkxzjbt.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gqsxmlciy.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/ghviqpphi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gxnkyuzof.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gmzjycgsl.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gmhsgpizo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gppdxmlog.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gqtiezamz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gtwdthowv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gjopqchrs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gkjnfdwkm.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gxrpozqfg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gjkleeeia.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gsodhbrcd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gennipuhg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gaujewjyx.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gpdlojela.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gwzyedtmm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gcwmhswqy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gwwchiddd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gkimiimvd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gjrrghckj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/giqrkzowg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gjyfkcnzz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/glwyhlqxt.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gbdpmpbpw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gboncjtep.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gmvpccqhs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gnjgqgmjf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/geafzzpui.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gonsfxguc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gfickqchr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/guqxtioxu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gwtspsakx.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gzbodczgy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gnnufskel.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/grjepmmis.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gnqrujsbj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gdtpfhbby.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/ghbmlgoyf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gfqcsbfkj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gptaqmpwa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/gotkkzwqz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gfcnqrkbf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gvpuvgtov.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/goxhflvuk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gkoyjaele.sHtML


<!-- 参考信息 -->