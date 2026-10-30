代发 wailian999

Java: class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjlneatkw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/goxytkeqx.sHtML

Ruby: class User; end
来源：http://blog.fanxiaobao.xyz/Article/details/gxoktkxhc.sHtML

C#:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktlqfkai.sHtML

[G02] 构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggsdparrj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbenazkgp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjllokyv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlgjofdj.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcedhxxoe.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/guuilhwjq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsttarnpn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvjyrgjk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtgeddon.sHtML

[G03] 实例属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeyazmob.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gshswezeu.sHtML

PHP:  public string $name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gdgcacrps.sHtML

JS:   this.name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhktxomd.sHtML

TS:   name: string = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gesjvokmb.sHtML

Java: private String name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyrxyael.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fanxiaobao.xyz/Article/details/giceutzuy.sHtML

Ruby: @name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/geppvgjqg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gakayxuyh.sHtML

[G04] 定义方法
来源：http://blog.fanxiaobao.xyz/Article/details/gorpazrkg.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/gjallsdtk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gazablrda.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsghqmhb.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxtnvxvd.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmujuuhv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gzjiphajn.sHtML

Ruby: def greet; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gmgwflnzx.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gzhcbqcqc.sHtML

[G05] 继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrthevgn.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmazbwfg.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexbxknzs.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvfasata.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccznrate.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/galcxcjhq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdargwska.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjxefclk.sHtML

C#:   class Admin : User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gonpakypn.sHtML

[G06] 重写方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhpshze.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fanxiaobao.xyz/Article/details/grucryykv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfuaajuuk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggybcwtjp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/glsloenvs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqbfqucr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fanxiaobao.xyz/Article/details/gvmkinkki.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fanxiaobao.xyz/Article/details/ghwytrcoi.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fanxiaobao.xyz/Article/details/gycvqabrd.sHtML

[G07] 调用父类方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gycrxkbal.sHtML

Py:   super().greet()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzwmqjzi.sHtML

PHP:  parent::greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gqupbbcvd.sHtML

JS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzirrssk.sHtML

TS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/glopwemrq.sHtML

Java: super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gkapnitbd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fanxiaobao.xyz/Article/details/giqmdnypv.sHtML

Ruby: super
来源：http://3g.fanxiaobao.xyz/Article/details/gdediphvt.sHtML

C#:   base.Greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsoclagi.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golmjpqjj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fanxiaobao.xyz/Article/details/gkimnvufk.sHtML

PHP:  public static function f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gitciwtws.sHtML

JS:   static f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grfylrcii.sHtML

TS:   static f(): void {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdiyuqxgb.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvexowuk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gaujntuby.sHtML

Ruby: def self.f; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgjjidbb.sHtML

C#:   public static void F() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrmwhkbb.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fanxiaobao.xyz/Article/details/gqzvazqdl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fanxiaobao.xyz/Article/details/gbwgyygqz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjeqhbebz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fanxiaobao.xyz/Article/details/gahuzqclv.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbysgvjlj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gkscsswsm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbroowniv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlkmyken.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gpysfaauj.sHtML

[G10] 访问控制
来源：http://mobile.fanxiaobao.xyz/Article/details/gnywxwoso.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fanxiaobao.xyz/Article/details/gefwlmmey.sHtML

PHP:  public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmaqpuaq.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasyekhmh.sHtML

TS:   public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqnvuyee.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fanxiaobao.xyz/Article/details/guzggbceg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/gdekiqzff.sHtML

Ruby: public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gmifxefwy.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmksaspz.sHtML

[G11] getter / setter
来源：http://wap.fanxiaobao.xyz/Article/details/gnvtzyzbw.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fanxiaobao.xyz/Article/details/gjqbbwiwc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleolcpee.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsxokjno.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gadyrbndf.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gccohrdoh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/geehwxmjq.sHtML

Ruby: attr_accessor :name
来源：http://blog.fanxiaobao.xyz/Article/details/giizmmmps.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fanxiaobao.xyz/Article/details/gouwpforu.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsitnxfek.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/gzkmnoguf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpcjsdklf.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxieavvbz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gutcysbyj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevpsaifo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gvotgexbu.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhxfnhpy.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gybbhjxbu.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsqtpsju.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzjiojjl.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gemsmqaxr.sHtML

JS:   u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/goyxdtxlw.sHtML

TS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/grpzibawn.sHtML

Java: u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/guzxsuuew.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuinksby.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fanxiaobao.xyz/Article/details/gpenyjznr.sHtML

C#:   u is User
来源：http://blog.fanxiaobao.xyz/Article/details/gaulnjfzk.sHtML

[G14] 数据类 / record
来源：http://read.share.fanxiaobao.xyz/Article/details/giwprmsmo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyuutymv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fanxiaobao.xyz/Article/details/grssllniq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyivmgxou.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fanxiaobao.xyz/Article/details/gxlrrtsov.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbeiqgxb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghizpxjlj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fanxiaobao.xyz/Article/details/ggzzevtwn.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fanxiaobao.xyz/Article/details/glipdajid.sHtML

[G15] 枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gtamohlxs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcuqegtb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grzhcivbp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsrjzeds.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gthsayydu.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fanxiaobao.xyz/Article/details/gcdmmtlbl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fanxiaobao.xyz/Article/details/gnqqgtgtw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fanxiaobao.xyz/Article/details/gljztamej.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/goupjdkbw.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fanxiaobao.xyz/Article/details/ghjswcpnk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxnmmalb.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjxewatb.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyxrjkco.sHtML

TS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/glqqwwuav.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxvpcmlz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuhlryvg.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtiixsvm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gewcyusot.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gutsmhjgr.sHtML

H. 异常与错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqnildmz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmxwyckuc.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexngrukn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyivoozrw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgewpave.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuqwsypu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/grmgylomp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqjrxvyai.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gysmqwfwd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzwcxown.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzyhjhpq.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjhvhvtk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fanxiaobao.xyz/Article/details/gfwwravut.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjxuammk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvbjqnsx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwkwmkbd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvemsuzdm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gednuemqm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fanxiaobao.xyz/Article/details/ghfqzbvbx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzsqyyex.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvomerkd.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fanxiaobao.xyz/Article/details/gamhihlut.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gagxlcwuo.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gwkfpobtj.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/grsojrrhc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gelydsulo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fanxiaobao.xyz/Article/details/guwknkwgs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzizoqdgi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpglzuucc.sHtML

[H04] 自定义异常类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbzcisdrq.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gpgwkydpv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmyujpzaa.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzndjpaj.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpzojbtlf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmvzvhvdu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcaeddxl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbchgcymn.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjkkxhzgh.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyvauruq.sHtML

Py:   except ValueError as e:
来源：http://m.share.fanxiaobao.xyz/Article/details/grfylxmzv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghcubextx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grspjvasf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmnrhgdo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gezuhzohc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqcraxjy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyupoode.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gglisiwdy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/genihrfdw.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/gdbxvknkz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gypkavctz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gfixbpdqd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gdldqifcx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggicizjcz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fanxiaobao.xyz/Article/details/giklwdffh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gapwfqhoe.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnndnpba.sHtML

[H07] 断言
来源：http://mobile.fanxiaobao.xyz/Article/details/grnkmejnc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhgwyrax.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmxuxeob.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvgezzye.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gujqjuxum.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gbymadvmn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fanxiaobao.xyz/Article/details/gomdsgcon.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fanxiaobao.xyz/Article/details/ghybiuhiq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gujoefcyh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fanxiaobao.xyz/Article/details/gmelknvbc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsntoohds.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fanxiaobao.xyz/Article/details/gommtpsuv.sHtML

JS:   e.message;  e.stack
来源：http://3g.fanxiaobao.xyz/Article/details/ggwihiqun.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmvcqfcs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcgjfyae.sHtML

Go:   err.Error()
来源：http://3g.fanxiaobao.xyz/Article/details/gfjpqdbas.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyfkylqo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fanxiaobao.xyz/Article/details/gsmattcpe.sHtML

[H09] 带错误码的异常
来源：http://wap.fanxiaobao.xyz/Article/details/gadmncxty.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fanxiaobao.xyz/Article/details/gzrvlkuks.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjabncpua.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fanxiaobao.xyz/Article/details/gjarkhmsp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcthrfpfj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geihcjmhh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyllmibv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjsugkgb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fanxiaobao.xyz/Article/details/geqwxivyw.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvnjmclz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fanxiaobao.xyz/Article/details/gvepeepoc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fanxiaobao.xyz/Article/details/gikxhpyco.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fanxiaobao.xyz/Article/details/gvnnxvzgm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqfdgiik.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fanxiaobao.xyz/Article/details/gqydnofrp.sHtML

Go:   defer f.Close()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjkmusob.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fanxiaobao.xyz/Article/details/gpowocops.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjulumwt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztwdoiyz.sHtML

I. 正则表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gwiplysnw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqacffveb.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjldwbzed.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnpywjmo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gygcxiuuu.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrjzwmvs.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvkkkjxd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnqhulzh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzexuoisw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfiyiwjf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkektllqq.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxckrjcf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgktvtku.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fanxiaobao.xyz/Article/details/gxnlvshdn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gobwywnml.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gagofbgvh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjajpyvj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbponzbwt.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkrviymx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopofqrir.sHtML

[I03] 提取捕获分组
来源：http://3g.fanxiaobao.xyz/Article/details/gisezcjbh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/glwyprbnb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gehhprywf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhmtgteh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gflfvkjht.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoxnkkkn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fanxiaobao.xyz/Article/details/gikmbekjo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fanxiaobao.xyz/Article/details/girtjctqm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fanxiaobao.xyz/Article/details/glceggxzx.sHtML

[I04] 正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkccjeiti.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwhuoroi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfizugfw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwirmkrru.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefvfeumw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gedaojvsi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gqpqwhcsl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhglxofu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvetbbntk.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgsijqiv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gewvzrlhr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gjynmrkuq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzupmudvr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnzwyzck.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gstsskixz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcldvexq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/grllmelzw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfaztvps.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fanxiaobao.xyz/Article/details/gstmupcdm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gtwtsyzsf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkisapxm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/gumpmtdti.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fanxiaobao.xyz/Article/details/gnrqtucws.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gmxpycqdd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtjjdman.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/gficflasw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gypczpixp.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fanxiaobao.xyz/Article/details/gpqkekfbg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvqeqfoo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/gztwwmuth.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmtnoama.sHtML

TS:   /error/gim
来源：http://baike.fanxiaobao.xyz/Article/details/gihdfbsxh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fanxiaobao.xyz/Article/details/gcoycfmnj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fanxiaobao.xyz/Article/details/gkfkeyvsm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtecnqeco.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fanxiaobao.xyz/Article/details/gqbvuzros.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fanxiaobao.xyz/Article/details/glvgpmgyi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkdkkvpi.sHtML


<!-- 参考信息 -->