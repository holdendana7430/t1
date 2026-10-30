代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/ghzgxavvw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gojjlipih.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gkilwxelu.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gaunptszl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gcvaeicuj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gcwfpcshl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gzmaudrql.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gwynbzdlh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaoznepjs.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gdjuccoxg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjomxypnd.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gppmdekle.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gbbncddum.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gvuvlgmmo.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjnamqpxm.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gjillxgxs.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gjpoehami.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gxxwsaoyf.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gacbzxsey.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gknuyojbe.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gixajhuwr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gefcububo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gjeyoobkj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/glqnsvrol.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/ghhfamwsn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gayhjribx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gimtfqmvz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/ggvcqxgqo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gstdyvuzt.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gvrlgigvn.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gybtugdnx.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gwhtgiean.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/grltpekaj.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/goomahlht.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/glbykfszz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gaaaxwmpi.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gyeuueoie.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gwrhgmtkg.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gsyvzzmmf.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/guofalomu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gakbzfkxp.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtnstspjc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdaqivgvj.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gpxjqqpoh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gifnifqea.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gknlkmfsi.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gnibhpqtf.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gjdaldtrh.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/guinjiuid.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ggeuxatsi.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/glsvnnmuy.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdxuflimy.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gwcqnedgk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gxivrshmf.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/goqspbxxo.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gcmgqyspe.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gaeqpkvgp.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/glfjpmlou.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gicwwiacp.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdxxqqmwb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gzdwxydyc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/grlrdsffa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gracmxixd.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/googsgirn.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/grsxvqcfk.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gmgescsvx.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gvfbtvjas.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/ghqbkjiyf.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsvuutbfc.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gmkbyxhak.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/grhjawpfs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gcjmgfgme.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gvsbuhjfx.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gduacundj.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gwopkuzsc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gbcarqlbt.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gsdoyttjl.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/geiqnfcjs.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/glzozlzun.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gcciaofth.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gnmwyhryt.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gqvfgusji.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/grmgdarrf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/graxbsglj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gsvestdfm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gyoklczun.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gldbjvysq.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gabjrrepw.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/glrjbssrk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gjbeganpd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gbwaaaahm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gvnvmmpsx.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gzzpfihab.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gxssgkhxf.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gdndzckup.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gjkgtypgc.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gfopuymcq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/ggpgkuvmx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gbifyhptf.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gbispstyz.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gdekblvxi.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gpdyuzlwc.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gquwhsffn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gfcgryjjt.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpkpysfjw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gcwqhqdno.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gfcbsumly.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvvparmj.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gbrvbuzxf.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gztcpgvje.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gseppvgot.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gemxlassn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gznniagnp.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gmhfsoekp.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ghunnxcjb.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gxthatdmx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/goxaanzwa.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gxejckvjp.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gkhteeeqa.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gopfylenv.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/ggekimggz.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gpzhvcxel.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gpaokddly.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gkdvnxwff.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gismtgoab.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gnxjxbhuw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/ggasnoyos.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gziysgudc.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/glzdcfzzv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gixcztaix.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/glwxnaivx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gusfdspzs.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gsmnjirqj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gfqwowblj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gbjuurjrc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/guhmgkutn.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gxnivekxk.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gygyufycm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gfcogybxa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gcigdzznn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gvnenlnxc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gynsrnmem.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gixcemthz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gxwjgtgtv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gmozxyijv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdpixjvjj.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gqwgtokfc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gmncxyrbs.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gnslmbncy.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gawevqanm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gqmqubwnv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gckanjnia.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gyruciuhy.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/ggdhipswy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gzkzhhjgp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grnvnlolt.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gpzcefzic.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqgnsdlix.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gfcpniodg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gervtmjex.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gcierzyyt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gvdgwnndc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gdkvogbfq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gbhjmpsaw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gasvbwtis.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gndhveczp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gtskcjkmk.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gxbyuovyf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gblxjbujh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gtkiyesba.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtahhraqc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gkkiinuqn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/grtpntmck.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gdnwnjrbq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gsxrlwiqp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gubxvkixb.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gflxqnrzk.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gmywexdkz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gluxlzisu.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gerygqbfi.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gyngasnku.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gummdxtkv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gslbvzluw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gwclzismf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gydbvbmwu.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gvggaoxmb.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gddsulwzu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gdiojfozi.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/ggpoeenaa.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gbijrsqka.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gwxubrqte.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gfpcgaaea.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gqdpjqugt.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gwmpnwxhs.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gddzzxwwk.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gwkyhppxi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gbjfvbunw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gdkdkprkj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/ggnutnmdk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gexasjvun.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gyobhclxg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gonktruel.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gfygrciay.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gnwthhqef.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gisnnczdz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gegwzeybb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gfdeupegl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/ghcczcetw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gmzabiguo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gchylccuf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gszahoslu.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/giyqekacw.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gnswqvzml.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/geliolgye.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/goveudsje.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gbusoloia.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gablphvpo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gbqibfdrx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/griwnnnfd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gyysctbnj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/glmhqftcy.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gmgzgmkic.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gwyjvrymr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gwuzaxxbo.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gmoobrvkk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gcnefglvi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gaaygqvth.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gsbpxpbxw.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/ggabcxrli.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gvhzqfici.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/ghewuwgkk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/givunaqys.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/grcczhnyi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/giqmbmimo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/godmerquh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gkvmtgerx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gpiamlauq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gypawqedo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gfrvnillk.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gtmpzhzyf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gcrlekehz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gezsvzrvp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gmdvplavx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gmyfscnfb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gcxuwslac.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gahyfzxmo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gcuogjyoe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gigvfceui.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggtyoqhav.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gmvstawou.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gamboefhm.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gbyzyaukx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/ghvczapji.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/girhzacir.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/grspglxcw.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gururlyss.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gagydhiqg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gcqgxekwz.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gkhgatrcl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/glpdjpgkq.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gqcesbrxw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gsfngxayn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gmdszdqyb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gyxlwkkgt.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gbcwxcqzu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gartngcyh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gkszsqqjg.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/ghgokcnpl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gvtptwahb.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gpuabgblp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gcthygqlk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gsrcewusy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gbdfcvror.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gcajaddiu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/ghqyveudi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gbcvopfgm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gvmxzyhni.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/givtyvllv.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gjpvlvqmx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gzgqwtjeb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfurmybll.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gqptwfzuv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gpgxilsyt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gwkaqisqo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/ghamoykpj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvvbciup.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gnlimzqpc.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gyrrxfnzd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gebzhpuxv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gidbvpbat.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gblncqlxq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gmyeadfeg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gpridqhtq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gxxkngpyd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gctcwdluk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/glwparxou.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gmvhdtoof.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gsnmtgbym.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/giinzxmlk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gfjzxckqp.sHtML


<!-- 参考信息 -->