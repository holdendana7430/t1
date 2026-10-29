代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gjspqfcpa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gcyeezohi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/ggxdhxwbh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/geauzgiel.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmcbqurns.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gigfkhvfg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfuompqwt.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gpbnuhfvq.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/grodhcdfc.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gesbtqbel.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/glslxowtk.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gdsuhwvkj.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gizveccsz.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gdwtqzgfq.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gxbhijcad.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gtsovaspc.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/glsquqzlq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gzkhvvzml.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gkonwiyka.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gkyyaaufh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gdavhhvhh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxfoytgse.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gfbiuycie.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gucvymsxd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfpxcsjer.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gloyarqbt.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/giwjtpayp.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gxppiviur.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gdjkktaav.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gnahbctfa.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/grmisosop.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/ggyfcjfha.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gnsvpewqu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gwbluznii.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gkbjkwjla.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gqmapkfrh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gnvhjjyet.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gkmfvrohq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gzohteydr.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gywrnamtq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gdabovhpx.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gfeenpqwv.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gbckllvbc.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gxesdccov.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gahoevxcc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gaapwxiyp.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gssminato.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwneofwng.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gqosdvtqt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gozkaieaz.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvsdtpqfz.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gcplyxsmt.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gtotzfhvv.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gascnwtpe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gvckkzlvc.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gstyrkedn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/grjvjinud.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gvageuuqc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gbnumsnro.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gghjgnamz.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gwgtvbqob.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gbzmyitnk.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/guhlycpkt.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gboefesmh.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/guejvtifg.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/grpxbnsza.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/ggcmrdzqt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/glovaowhs.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/grsqaqrgj.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gyfljibat.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gvtkdbltp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gmjrluxyn.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gcfguixsr.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/ggenfmjxg.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gcgkexaio.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gwbvveckx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gaoiqjzgg.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/glallfxvo.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gdzqiipbi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gdzolyckk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gtjbnkxji.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gmbqgmowt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gqxiegxyq.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gjcbherjk.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gzvaancfo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gulevpcjh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/guruijnxu.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gidiqnpuy.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gvbiqrpaw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/govwdkmbr.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gjldkerra.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gzmbdllfq.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gylcpcayd.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gbveaezji.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/ghonsrifx.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gytvsxfkj.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/ggqndjdry.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gcorrludp.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/govviamqi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gyznedlxw.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gzpcpbssa.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gtxexiebr.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gnpbabung.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gyywvllhl.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/godogghqw.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gmvevgeis.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gzsenjlrw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gggqnstad.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvvtrbhed.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gvevytykb.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gasbzxyjz.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/ghyfwsgxm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gtotijgst.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gcooknimh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gyxsmvntp.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/ggelkhddi.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/ghpmrhmgu.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/grqkmmzue.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gbdgveeyf.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gndvgnukb.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvpnsijvw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gnpwrjqau.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gvqehdugq.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/ggvmvirrt.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/grarltxgw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/goahgratr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/glrvxdyeg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gkkkfluhe.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gwhpjipfp.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gvnpjxnjk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gdilwtlxt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gtfxchdus.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gflwfqdnv.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gyxkiqual.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gwqamfijr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gxyfpjvov.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gsrewbdel.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gyiqqftbv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/grbqypqll.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gjwologai.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gvycgwrsc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gzcqwmoux.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gijjzypvy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gphncixeb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gpazdnfgd.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gveigifwx.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjmydfjzt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gcqxwiiey.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gqevgfeap.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gpbxkuthp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gvvwimsgp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gltfaccbp.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/goiihfebw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnxabzpeq.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gwhidycze.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gzcgzmlkf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gizfawmgq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gcydzyjlb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gitkdpivi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gcohtdkwq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gxasrzdmb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gvcoeirtx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gazcqpwtz.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gkraymdtg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gfvtbwbzs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/glwrgpdgt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gizkkrtyc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gqifbczqk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gutiffarg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gjoctmrkf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gnjyfipkp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gpvjcaxuh.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gpjwkaghn.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gwcjqdwkw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gvmaxmnsn.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gfdptjmhc.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gskrwlnzi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnjhbxtjj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gyfdzbdws.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/geuhtwpni.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gxgvgjcqc.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/ggcpxejby.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gfaagzyam.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gdnebdbwg.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gmjnkypmj.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gbhqciscj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/ghgnedjeq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gwvhfswpl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gwrcjllci.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gasroidvx.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gdjxjrevc.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gflgzkzkl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/goulcputg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gpdvpozjb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gkgbiwyqz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gbpaoadpg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gklgqmrea.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gsprguivx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gnendssrw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gsmgdfijm.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gapljrtbo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gxgczafsu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gxojrzzuo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/ghyrsfqjv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gcxigytla.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/ghbgtgavk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gorwyuned.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gslbkgbgv.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gdildfofo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gnicvleeq.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gzdinbctr.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gzthxgowd.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gistravkj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gwmnnjrbv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/guuugunpy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gccxuufip.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gwlpkpeug.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gscmmhxcd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gpavqbvna.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gycdfffgv.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gxcqlnwnj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/guxurmamr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gxtloervl.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/guozqlzfm.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gsaowbtcx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gwuruqkry.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gequscxip.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gtipksudd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gqjehnsgv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/goqorckjs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gzxkkefpi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/guynzyqkf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gxyruuiue.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gtqpasesw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gxglsoqiy.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gljldxpce.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gfkuuwlhw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gxzfownym.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gjnaffwjb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gpaoaiydr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gydoovocm.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gansofrfj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gpgjwfycp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gihrtnlic.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gurhojpcl.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gtsamnwco.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grdwfabmp.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gdlogklbl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gmirxklxh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gpekfrevt.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gikgwaksh.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/grdhfxekb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gvfhbtbja.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gpyyjlbzn.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gntmcxbbq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gvzqbkxxq.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gtaaqhoty.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/grqtpdyuc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/goyqurmon.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/ghmnjtjdr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/galkaqrnj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/glvbnjitv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/grfhebmpz.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gpajplwaq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ggbgsfxuf.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gfamwdinv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gvhozpyus.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gpthnrvhw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gexxiewqg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/ggaisxdpg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gocmvjjeo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gyrnuzxbf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/ghcqfsurf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gqsvlaaig.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gpsgamxml.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gxjalsecz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gdqhfbceo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ggqdmewxe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gsodpqvwl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gbeatddys.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gwarmfsrb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/glqfbrulf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/ghejcujxt.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gxeysnqri.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbtcewmj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gajnfjuls.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gvgffpdkh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gdivvdhos.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gcywpkdhh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gwaulhhut.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gqaxlsght.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gqxkpyviz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gwiztknij.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gpncsxykk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gvolikdem.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gjjragakh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/giygctfpf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gusvikluu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gwhjqbgqn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/ghdjsxwqo.sHtML


<!-- 参考信息 -->