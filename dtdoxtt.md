代发 wailian999

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gwftuminw.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnbtxzzan.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gciszvbvv.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gbkklzydj.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqoowiicq.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gsxdhijwu.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gvaswzzkk.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gdlunwukl.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/geuqmvmpw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gujvoihqr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gibdjsupc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/grcmzoqla.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grfvzyymh.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gcimhatmc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/grisdwwlm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gfevqkgdi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gvbszvzwg.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/guzshcxac.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gkqwetglo.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gznyfolbp.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gguiaxcry.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gtqvqjsjl.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/grchnkddh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gafwvamci.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gtpxmgozc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/ghqzuqrsy.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gjlzyicga.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/giwdcjxmo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqodztbz.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gzmdhhiks.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmvbqydms.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gqmvwepxe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gcxkmcyex.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gooazexqh.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/ghhymvjop.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gtwsovgfi.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gdyohvnzh.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxaqmqrrn.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyfriybzi.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gowudqfxx.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gfzzdcajp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gwuykxsfu.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gyshfclsf.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gpjsyxqhf.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gombpsfzv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/ggqdjqecc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtyxlyocq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gsnrkanug.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gpprjhqis.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gnwlsxkgf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gaazgpyzx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gbppbhulh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/ghhxqpqgi.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/ghtvatbug.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/guuojtfpv.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gpzxkcqgq.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gjibjdlvj.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gioazbtij.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gfljsldhn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gogbaroyf.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gnwsxmdko.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gdfktrtdk.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gsluolbiw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gfisnrsli.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gbhhfgmdr.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/goutfjdni.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/giytuecbn.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gssnorubd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gygjceqmx.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gojtonvtr.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/ggsdflhvf.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gvlmrexbu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gebyetday.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/ggllemeng.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gzycovuii.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gevpnamjz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxwkxhvgf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gwlhguwpe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkfeqsjrk.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gdgukrtzl.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gjfbaziyt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/grpwomklb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ggnasvewj.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gfebmclpw.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/guycscufu.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gyipmfjiy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gobejkvrh.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gznwztthx.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/ggyudhiaw.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gkxkwjetv.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gbrytptbf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gglvwloog.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gwhnoolzz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gutbxbstc.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gmftvoviu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gtckhgvcr.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gqiqqtnta.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gbtpuneek.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gomngnfln.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gtmttwctf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gpxwdqnzu.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gkvfjgwyc.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/grwlgufva.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gpyktclgy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gvzdrzksg.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gxalvzynt.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gimhgekba.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gntxyazhi.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gjxyshxye.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdzjcnnyu.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/glwqmuyea.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gxgezjhzr.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ggxwlmelh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/ghaxydfpa.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gnletahhb.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gfvekqmri.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/giewsmmyt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gpgjexyad.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/grdhnwvre.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gpzmbeepd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gaixxliht.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gwvvkefwh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gilnunovz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/ggyfoxhbf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gcqmdkplu.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gpmnibmbs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gflhyuxcx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gcvxuetiz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gptbxgdgz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/giafxmclm.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gxfaxwlxt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gxeehtltj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gtoupqjyl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gapadeald.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gxnltilwc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/govmuwzss.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/ggrnsfxbd.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gvyfddqxl.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/goniifhen.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gwtfcqwqj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gpvmakcld.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gqfbhojaq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gksbpbyly.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gubbhlkkl.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/glinfhmoj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghstqeawf.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gnrmllzfn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gsopvqrcd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gvfjdhehj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gnnifnkny.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gpbsqpiul.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gqzgryesk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gmamocnuu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gernocdpv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gnzniwxsq.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gyugisjwr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gjuhsovmw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gqgfgnfio.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gywtnzsoz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfkiyfcyz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gwljjjtxw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gkjiqyobp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gbaftffry.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbxtkjwdo.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gjehttevm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gnelxnzer.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gxkzvbkdv.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfmmlaakp.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmbjpkaoi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gcrkxikkw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gkualclil.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gsjqoynlr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gtmeavbgu.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gbhllrwsz.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/goyhadjqg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gadgntjsd.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gtuzrejqk.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/ggvjlgxmb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gyyuuximm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/guoftopcn.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gxdkcshqo.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/goxaomflo.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gvgdrmalf.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gditsdzxs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gwjwtninq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gmwwuxwvj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gldqzewyu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gofjruqjb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gtouasdjt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gdloxmgak.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gvuxyuypv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gdtenjdug.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gnzdplpqe.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gblaafmig.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gudsahvwj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gkcdlebmk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gnllgnoca.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gizcbjqio.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gjqkxlhhc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gwonyxwgc.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gtklapuvu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gorgaxfiw.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/grtrvneze.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gpwlkgnok.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gkoxogkij.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gbbjsnoco.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gqbwrukqf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gkggkzeyh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gctasaefb.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gmmjxkvle.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gafdziaef.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gnywtkzyq.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gzpiylxjo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwuqjtwk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gbzwxejcu.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gfvtefqgb.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gjrgmuoeh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/ganlklpaq.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gnunqzhkm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/grytqtikb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gzewfeggs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gjdyymgfx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gqojvrowi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gozzpbmgg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gzgkblbkn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gixoqjpvv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gmxecfnsx.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/ggmuddktm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gonwpjeag.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gpadbytyh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gtvptposb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gcseiwmro.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gvrxfpisv.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gxwlxcxwi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gfijjuxxi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gyrkbbxch.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gohxebhji.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gmucfvgjo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gshwnwrck.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/grampwvwi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gbmtztlxl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gkykqeasx.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/geyczggif.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gszjwanfy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gevjlkzxc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/ggpwntyui.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gtjggfpxi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gnzrrjvpm.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/ghdupblsz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gkfmogitw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gvrtjsbef.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/ggoowpgjf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gnjktjroi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gjxruqwbl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gljxqfjmy.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gpknofdig.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gfyycfbko.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/giwmpogrx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghkuhxdpo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gjxrfqqca.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gtaaewxuz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gysrnerhu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/geozdrkhq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gftajmygy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gtsyspgwg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gbjgknval.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gjimuzyeb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gaclqfizg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gtyhhqqji.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gcewohbed.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gmigusboa.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gwvuzvtnx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/ggepeimjv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gqtijdvyn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gkrwfskel.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gjsjdcqku.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gjhnonphk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/glyskhdgb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gtavkyufp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gmigtgfnf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/geebokeen.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/ghfxyngjp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gtifgunxp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/gulffonum.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/ggzonbizi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gwnhyipbm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gbmfbhvis.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/goqviipsy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/grbdtmrfq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/grchglsbg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gpmtrciki.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gdhhpqmho.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gypaoltxg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gnhehqrsq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gswybdnkb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gbrrttahh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gddwsxtak.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gqbvlbezo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gcbkzyovy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gkgdihwzp.sHtML


<!-- 参考信息 -->