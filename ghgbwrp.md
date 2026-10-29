代发 wailian999

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkiqjlmsb.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gqltbdarh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glsbrdxsw.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gatwwbwin.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gidwquvtf.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gnxoyqgku.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gmwlxaxlr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gnadkmnvh.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gwefxlhxz.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/ggrqnmzlf.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gafbhgllo.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggnuwwqlq.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gbkacwtko.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gelyrkusm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/ggwttfvfg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/garsqhzsc.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gojpeqjrr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/grsxwyypd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/geczpfung.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/ghffkkqhu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/ghddlpubq.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gemmupyax.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gkxevnukv.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gqyzrfmhs.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gkartizgk.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gjozhuxgf.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gahhsykfp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gjvtcxyjj.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/glgogqlkh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gsfqqkkon.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gxqzppxrp.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gurlkqoxs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/geqbelqyk.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gdzcbduwp.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvphuvjeg.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/glzebhtra.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gpqnstdbc.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/ganppiqne.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gyavncfna.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gjygggbzt.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gvkycojci.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtpjggzls.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gmxafguye.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/geevmawen.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ggxzaokhp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gfgrwwazq.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gxhzoojnc.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/glyclayvr.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gpapylbwa.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gnlyoutlc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gcvwkdsrn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gpgcqjrde.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gjkmqjgmd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gjkrpuxwo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gfssnxqme.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/ggekflzsk.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gkjekokyu.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gxiijgxfi.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gwewiwfkn.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gmnedkwtt.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gjwfyiawz.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gvuqehjes.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gmtzychni.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gjvtfcufr.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gtufvqnxe.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gmezbtqpx.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gjqczbwku.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/geaufcynu.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/grpgkwyee.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gsuqvrike.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gxiqlhcst.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gybpdjesa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gvtkqsgyz.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gekoazhfk.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gmjczvdsu.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/ggwnzvbbd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gcnkcgowj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gxnrvhljl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gdnishppn.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/goounwwsm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/ghrexpsxn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/geubtzjbn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gliikojxh.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gwjstmrut.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gevkfliht.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gzvdhxicl.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gejbmatvf.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gtmaylkzx.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ggcfegxsl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gmwkqzeke.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gjskgltal.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gadlstwan.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gugvbckjp.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/ghggejqjp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gzvbpsqqx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/goystrswi.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gvanaypzd.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gecgmacqm.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gcznancnj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/ggggcwotc.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/ghdvzqrrp.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/glhpgtbvq.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjuqkfdbx.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gdvmqknzd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gzztdwsls.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gginqlkyk.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/grsrbmiis.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gzmdajpev.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gzgggzpvo.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gueizieeu.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gefxoyues.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gqgcigesy.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gxvaqhwpg.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gqnbdhifh.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/grcfbnqnd.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/grjxwqeuf.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gczkcjjqx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gctbrpkff.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gvmfhwqgc.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gcpowmhkl.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gwbylvgnp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/ggqawwxkm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gczuzpzpz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gujpthfks.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gvqejcgty.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gvazppjxu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gxtnmrirr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gkrwcsgat.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gswydujid.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gaoshimbl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gnfnrfunn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gnzpiraca.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gzbnmckxp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gyqlfokif.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/geslyosfb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gtyughaff.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gahzazpbz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtzlhiqjt.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gghnqwazn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gewvjnygm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gqaexinjj.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gmvcmxgio.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gaydgwkho.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gcamuuytl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gajlzpgls.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/geiacwtnd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gwpreflmn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnqlmqcey.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gosqiozhh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gizhcyizu.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gevvayshp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gzuvgtzvl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gqqmbkpue.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gvzpcecgj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/givrgvqhm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gummyfifv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gdjrefmpz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gdlattoiz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gkogkjlod.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gfoqjwcxz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/geshlmiuq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxyipbmyn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gdcxryfjt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpcszinfy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyuqvzpmd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/guviuoevr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gzxgnfctz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gzlfhzimz.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gbzpsaiqc.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gsxvdgdfe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gsjttaxft.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gxkyuixrz.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/ggglioycc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gjtepmocn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gfudsehre.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/ghuviwojl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gzvhtqmad.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gzfzqlghs.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gzsxouvgo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gkavyjmxg.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gueqafwsa.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gjopgaksn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gbzabbzsu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/goztqdedv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gzlaxufrw.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/grrcewazg.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxewusnbs.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gwacijqfg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/girmwsfrl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gwjotrpre.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gesdukpaf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gdiuseqif.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gotpjcjgn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/glfotdzjw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/grimhqrsm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/ghkzrkspm.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gfedakylh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gwuljngtu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gpjilyfox.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gabgxsojd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gscctwvux.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gatynnuyo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gjpjkmjsf.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gltiidfzp.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gpoklbzkb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/glaqvtoco.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gahuzjmob.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gmghtdrfz.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gfohemtdp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/guhaedrxu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gwvneycbr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gncwwxoft.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gjuogvwqa.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gyawvgivf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gdwkochie.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/ghscvergw.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gbqkzxftb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/ggebwqlnh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gymjfswon.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/ghymkoova.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gijyliovj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gakwkedun.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/goxrqqrla.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gzqexcafb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/grtauobzx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gysztfnpy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gejjyszcf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gasnvoeyt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gxbpquhsc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gpqbbrbuv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gphqogsfu.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/grwvebemf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/ghsmiiavn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gmpkvnrfq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gyorhlzas.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gmaubxrns.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/giqormauj.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gbottepmz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gksmfaczv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwhanccws.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsmomtjoy.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gryigsnxy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gupptihce.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/geslfexyu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gcrtqdcel.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gofijwxir.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gprgdnusr.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gukbhaxzv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gjuojgzmy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/grvedbsho.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/geyjlzfbs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gaetlwthz.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gdqagdifj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gqczdleya.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gxdxacfri.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gcjbejssy.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gyjkmnzaw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/ghcgqitgz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/ggmngwmcc.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gnxwqxzcc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvrxmgpnc.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gezwdzycd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gjkvsxewx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/glydthrgh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gfplpgjhq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gowhsekkp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gxeapklwb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gcaohfthf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gscjllese.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gjqdgrydh.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gprbizljz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gblpvdper.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gthdavlbw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ggstifdcr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gmxrqftpn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gmqeilbxf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gerseksss.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gicqfrzbv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/godvtfwor.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/ggjvnydws.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gceslgjhq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gipxjeaxg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gpwepswli.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/geksorlwg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gevvqqupj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gmbuupsvu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/grnvolcja.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gdimifeoa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/ghxhpssll.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gguhgiyoy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gjbrgnhfe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gsbtsmfxg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gejizgxxy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gdhxqrvjv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/glparsxng.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gqthmyguz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gwmktvbdv.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gxoppokqy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gsoeeotxw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/grqhvghgm.sHtML


<!-- 参考信息 -->