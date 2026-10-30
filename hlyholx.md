代发 wailian999

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghmzuzumw.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/ganbvwfhy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giwppjhxd.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gbrxjlbec.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gkbadqcdf.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gdgjuggbf.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbktiepqy.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gvsrcftks.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/geohylewj.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gijyormhh.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gbqbukcli.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gyjjbxoeq.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gtxijuxdb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/grrdttzkf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gldfnukyx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gndozgaqz.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gfnbewdlh.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gewlaquwb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gfkkqwfcy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/groiqqqdv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gsmoytgxr.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/glgpqjmux.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gbsvwsjih.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/ggissoatw.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gqknopphm.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gyldyvvoj.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gcnuaatjf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gwyoswrxp.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gfycfqznn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtmfpcwdi.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gqkimtnlm.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gqdqivuuz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gvchjyjaa.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gkqplcgwv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gkouohwdk.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gybmtvhsj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gpktlnnwc.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gisockuoo.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gfppxfrkd.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/guajjsjhj.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gdhpaptay.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gvkxjmjsi.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/giipfmzzy.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzznlutna.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbhdrhzbk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gqhwottbo.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/glpauhokv.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gljdusbis.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gzxqbyfdn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gjprzzgeo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gshmiapuz.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gtzzutonz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gqgaqvoqr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gzfxdqtvi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gavjzlrpd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/ghiaugnzf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gkoeynuly.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gdwribupl.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/guoagitpf.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/ggfjnagfx.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/goblzbluk.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gbkpsbpkp.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gebxeniqv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gqvicntar.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gsjhnuegx.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/ghgfgawsy.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gldqwjful.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/ggbnisgky.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gcvywhyot.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gdthmvbtj.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gpaelnmnd.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/geldpedce.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/ghxhstbhe.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gfektidfj.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gxichnotj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gwfmtpajg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gvbisfevn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gdioakgpn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gsmqmwtzj.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gtbldrngq.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gtjqtckrr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gwyirsgfq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/ggwfwnvfv.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gizahcnsg.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gwuepfuyj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/glvqsftfc.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gycqnuafg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gjucrkfho.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtzncutbi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gswinpdzu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/geusivcax.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ghnzeonff.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gavitlerw.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gnbyuzlcf.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gqfmhojxq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gbxvdyhbz.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gzxffrvax.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggeciowip.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gnjfvpdxc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ggqbceteu.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gbrfcoqzg.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/goaszyrcc.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/ghikrtfak.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/givcwdzls.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gvtsnefxe.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ghappdeam.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gdknqkhtl.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gcptyjdvs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gjlusuccp.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gwkifnshp.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gqwpkclok.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gngmaqadm.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gtzgksdok.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gponxrrfd.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gmrtvotww.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gqtzjqcgk.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/giygkmbpm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gabyviomi.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/ggdcyvsut.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gidxgcnhx.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/googvamfm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gqsbnxzwm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gteynnuad.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gncfhkdur.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/giuwdeudg.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gynviaumw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gniniepur.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gzhgquavp.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gldgxjqoc.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gfvpagutm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/ggbtoznjl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/guibtfmeh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gxjjqrcdd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/guwwqqhld.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/geeaudovi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gxvvkyvoe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gjvogvcdm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gtbksmfaf.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gyvpujuuz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/grkytzjjf.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gaqopgzyg.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpfjxmxru.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gpmdgekhf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gmoxadmls.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gbmjicimf.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gponwilyl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/garlivliv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjccnggxi.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/ghluxkfku.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/godttutpj.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gtojypipv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gntglzuwe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gjqemdmsu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gipnatfre.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gpqdzunwn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gszrcsbbr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gidfqgxfx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxvtlvpby.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gccgwzrmr.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gywzutset.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gurpxlnwd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gcvpsvwyp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gbwzdtsck.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gnmbubbbv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gawvnobmk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gtklanvic.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gjkfuvhlk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/goxqokkvg.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gsivucfui.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/geffcpluc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzxezzbeb.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gbalfgntp.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gfabnzrdy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gxthxanht.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gzjwvpnil.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gfutwsgsh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gpevronph.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gkhmfqcmm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gqiulkhyb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/ghefbbtep.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gviaivtaw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gjronkhzm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gojqzaraw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gwgrjltxt.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gnsgkbzbt.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gkkrzxteg.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/ggwygfdlf.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gviofbkji.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gynxppvxe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gfeeelobd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/getpfkqzu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gjbmcdvno.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gpaouuncs.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gqvxclxje.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gksyunwcb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gooeelnww.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/ghrcglnsz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/geqrlmysq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gwljbicdu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/glzlrapbs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyeasmju.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gorzmcbzq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gcdpkzard.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gqhwfoupu.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gdhxazaru.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gjainzryb.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gotfhzjmc.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gofygicfv.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/ghuvsyxtl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gvqfidpet.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/geckbpefl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gcobardsv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gfhqynlpd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gpxdqifmu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gslwtdodt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gysmzbjyx.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gnjkxvjhh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gvnafuway.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/ggzvmgvdn.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gdflvmlna.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gyxajotff.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gnfiiawoh.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gvsbmlxuy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gihipiwjj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gnljxodjx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gxglyoeww.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gumccogem.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gjcyimksy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gljgxxtch.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gvvoqkhih.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/gxilfcdqx.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gfkixjdlf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gvrzkkqnv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/ghjloxeji.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gvafztfvs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gibsshpcv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/grcxslvcs.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gjsegvbvm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gveyzwida.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gghfofyah.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbnrqqded.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gnfobgjbp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gilawdzkp.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/grginmvft.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gcckyamva.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gdyhubtoh.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxyzkksur.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/grkodolbf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/ggumaliya.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gyvhrhdqp.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/guooekkvl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gobjivsxk.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gbaijlayv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gfnypvrgj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gyahvfdrr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/ghysnqokt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/ghuxdabiu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/ggpbwpdqt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gjzhklbpe.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gjunbmxlh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gzxlwmhxr.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/glicfpwej.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/ggbvqbtsu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gwwoybblf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gvogengbs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/ghjzyjijo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gbmwxhahd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gksndkzcb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gbigfttqk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gcurtrknt.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gniwmdmzj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gveknxqbw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gygcdnmiz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gtlhgskth.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gbndwuoxb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gllmnzyxz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gdnomzajp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gptwfcpsr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gliadelyu.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gazbgrwij.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhjlkcuc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gslvfzlxf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gjekgcipo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gohawrjaf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gqcbcfvzw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gxpdmbycy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ggsgsfilh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gdixyicyg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gkhkgsjae.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gjcohyibs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/glhdqmyaw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gotclcqot.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/geeqxwhmw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gqxcfvecx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gfyrzvqdr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gglhzgryh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gvvnskjnm.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gjuyaegru.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/ghzmxkpdk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/goumqevlk.sHtML


<!-- 参考信息 -->