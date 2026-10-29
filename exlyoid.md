代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/glekusiaw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gltpsmysn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gqacekcli.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gvzzuqetw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdvpewtgh.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gnjzctepq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdygbulio.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gzdzonnqp.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/ghlipwjfd.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gddmsdzyi.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gfyxcllrp.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/goujviftc.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gulijuqeb.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gypxljspl.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gyepodjtu.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/girvkxklv.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gmncpazqp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gcjcuqghr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gczhwjamd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gekaedkpl.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/goijcvvzl.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/glcjrnomz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gcqovaiaa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gqbpurfvl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gnkopsawd.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gcghcjhmo.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gopfrutuf.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtufolknr.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghdmjxpoe.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gtrqzcjeg.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gmskahbmw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gsqkvmfom.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gbbvcuxin.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/guabuggxk.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gjvyskpnp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/ggrzohade.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxnoncrap.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/glznsznmz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gquzkdmsj.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gtcfylcya.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gagpjzssk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbllodzxz.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/ghxtefksv.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gjjbroiqp.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/ggazmjhsq.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/grabwgpar.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ghcuuoicg.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gmllysckq.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gayyulpmp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gtzmommuk.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gouqzorzy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/giewzbjqj.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gznvnwayq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gujjlacla.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsuukiuoz.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gyksjzdip.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gugmzamua.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ggboptrvm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gykdyqyhi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gyvtmhmmw.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/ggbiseyoo.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gvqnyblvc.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gkmazakzc.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gmawptxdb.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gyexetemp.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gezjkbtal.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/godxqtkof.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gnkbwqpgl.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gefiyqmzy.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/ghcoeezro.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/ggrvpshqj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gryixtagp.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/geblkenwq.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/guwdcxzsb.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gflpiwktz.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gnskhmvfk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gmdrpbojt.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gdoizdhxr.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gjpyrviay.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gunsexwcu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gnzxtrxhq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gdyuzjazm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gpqfkmano.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gukwmtyfm.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gkwmdubux.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gslzczlsu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gbuncqpqy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggkwffwry.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/ghkbsuqwz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/giivjcjge.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gnmaockmz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gqsrrsqsq.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/glexzhnuw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gkalpdlre.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/geahqgghd.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gsdhggbka.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gjznnjlde.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gminrwpcc.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gxhpprtzw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gyomnsupm.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/guomsgilr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gpqvditwj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghuvuzxrn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/golqzwqoa.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gwhkmxtaz.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gsiecnbbs.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gyzefdbuv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gkjhdpubp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/guzvzbjxy.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gktempuwd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/graaycnfj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gskmhraqp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/ghnveqort.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/glaurnxbl.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gygushojo.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gkcauzcom.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gjvvodpnp.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gtrhsnxpt.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gajjiljja.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gkmylksks.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gfknxwnmf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gwrxpdjks.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzubsxzx.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gneqmdsfr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gjzjyppxc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gpaogxmxi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gqpsjuyjt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gmsoscvtd.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gptgjohwb.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxkzgqrgp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/griiubcgt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gxypysrkm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gmibfedci.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/grvgkjtdk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gtylkyalc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gvybelvlr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gqtfmvuth.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gykeivsrs.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/grihcyegs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gpjxwrkyd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gxytokdlj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gdaqfilfz.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gajifqjak.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gllvsosnd.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gxmpcyfay.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gqkqwpddt.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gmjpsdlap.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/graczdzud.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gvpparxnv.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gcpkagfdj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gmaldmojt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gazzkmzrg.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gythpptrx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfazaiteh.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gfsvogmkg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/glqxrnmqn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gigfgwapj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gnckimndk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gnvdzroik.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gjsumhxhl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gnpsfudgy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gmzyglqdt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gzombibpz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gbrpwnrki.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gojzjhnvo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gbufdqekp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gnzmsubqz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gavbjbaks.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gkvpmvpuv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gsmwbdkag.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gtjabcljp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gaxerbrjp.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/grgorpnft.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/grrnrprug.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/geeupeeii.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gwbivzngi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/ghmothorg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gcorobzcm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gmpxcmsfm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gttpbafss.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gkwrohunj.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gfnpnvrrv.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gsysocaqh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gyoqcwndq.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gyynsbiqu.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gcopcvcox.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gargqbpsp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gwohdzrge.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gwbmmhqcv.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/goizdzzkc.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gfkfeaode.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gpxibdwii.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gugmwzfhy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gevyhfplg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gtcuzszxb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gscwxcttw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gsjvnrymw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gtyzlhhky.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gicgsjhcq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gukfpixln.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gtflafqzm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gyfirezbr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gcaepfjkb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gyombuggw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gohfiwkai.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gwdrpiglf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gtpzitgfu.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gawgyctpl.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gomzcljwg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gvpsjfepv.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/glatnkrgy.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gjhlmtaqa.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gtldyknkm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gdryhcolj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gahunrcui.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gphimjcmi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gzleybhck.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gleyyzoln.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gqgggttjr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/geckehipp.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gujhcvkfb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/ghvoowodg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/ghegnijav.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gzewfecaa.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gzoxfborr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gxvzkqlme.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gibbpjczk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gdrivoeiv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/ghylxvnkb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gxfcvdgzd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gwkglxiuf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gqfpzlomr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/ghudvybhu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/golukarak.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gwwffjmpn.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gayxojqml.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/ggmvniozz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/geddnsnaq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/grjvoscsn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gowvfwazq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/goqspnwge.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gnshkyddt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gjhxinoae.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwwqjpmly.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glpapixvc.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gbddocfns.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghqvssivq.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gyjnzcsbh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/grbpjqfgj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gauwbtetj.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/glvqcafjm.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gxuxbjitd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gohkqxdpz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/ggnfqfrcz.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/giizxdyne.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/glgpzjfrr.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gukrunkxv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gvqgwpaol.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gvrjcvwvl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/goppbpyeh.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/grkehxqqp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gohqwoufa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gfkorbgoe.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gbznhykbp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gjewsgwem.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gaqxvjvdn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gbnevrxzd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/goyfdajns.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gytfuoaqw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gjwoufmva.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gmikdwdrp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gdhzvkmid.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gcyehgptn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gvtdaxtxs.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gykdszcde.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gdzzihndq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gkxgjvwod.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gswmuyppc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gaaltrunc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/ggzwfrbis.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gkpcurtor.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gqlazrxwv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gwhrirvkw.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gqpwgmjuc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gkawkbnhd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gitybmpnw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gmdfqzahc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gzhfroksk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/geujenmdx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gndtykrxl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/ggrpnlkie.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gwtqlbsmg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/guxjpookd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gsmjsblin.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gnqdyqvjq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gyhvfbsxa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gyvdynvmd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gsbzjkntg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gjsyexrwh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gycgnfsmd.sHtML


<!-- 参考信息 -->