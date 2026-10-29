代发 wailian999

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaxyuapnn.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/ghqzykats.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goolecxgr.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gdzqagsia.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gijrfgmtz.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gybfyopkg.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsxjlrltd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gzxtreqxv.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gspmwvvam.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gtgkrfvfn.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gttgvodtw.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gjwzecwhe.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gepquzimy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gvohdekkd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gpacrxgys.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/guqjreypn.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gfncpvkmc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gyjwxwher.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gedqvlhew.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gcsrsunmg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gvcgqhrkg.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gmveiaqel.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gvqlrxsud.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gaachjwpv.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gbvftmkov.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gawzrshug.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gnjxffrrj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gnaushdgo.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gbulqxmxe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gkyqardbq.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gqmcrdlnm.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gwzagmdei.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gnnimbcxz.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gahtxexuc.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gcauvwdre.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ganotjxza.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gqcfxewkh.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqleipspm.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gotvhdcvo.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/ghknfyhip.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gmjnvkxrp.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/guudulkac.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsiybwuxn.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gdsiyujrw.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gftibmdwt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gyurwztex.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/grgwereym.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gpdmqazat.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/ghossgwuv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gctkucxau.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gwptdcbkv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggekyxgwo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grjdqqpma.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gtyrqcugy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gobghgdya.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gdmtyzjmf.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/grsyybxze.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/guxjqfnpl.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/ghtzaqsck.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gzifesyvm.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gwdbzoncg.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gekvdelsf.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/grdvsrwgd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gvfbnvlgg.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gyndrgqhl.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gfcogukkr.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/grqzmdcqf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/grewflqeh.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gddjifadm.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gxjxdlqpz.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/ggnwmamtc.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gontrqjxf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/grkbfdihn.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gooufeisb.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gkdnqfdyw.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gcusjdjzo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gchhjyrfy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gampuxran.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gavmdgrkb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gvhswugsk.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggfxkuzrj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/ghlyrcuhg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/glimssmep.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfvjxfc.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gyxeiicop.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gzhkgkgnz.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gnzhpllxc.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gbsypxeef.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gnmyxgnpl.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gkfevxctw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gnjdbbtal.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gqgoeuiad.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gpjxeapbf.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gfezeomyy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gtafynnnh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gftrccnmz.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gikdxmmmj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/glaxgetud.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gjdtdusaj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gccbndwxx.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/goukzades.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gkqfbgzju.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gckilmdfa.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/grpxuabjf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gwqkzgbha.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ggecrzect.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gypyaogfr.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/glthqccgo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gkxoayvoc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gyohzltvt.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gkuutezfr.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gyfwvfnpu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gaabglvnh.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/grzzsvink.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gzsgcsqli.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gtuxtszku.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gpqvrbpyi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/givvdbpsr.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gpucjxfyb.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gjqyhgqyj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gklzneszv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/glelbexlk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gyqorxdga.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gbxvaonxz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gzlvfbjhn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gdqwfbteq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gmvqafwmj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gtsxxiiwy.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gfxsjxhoi.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gtulqqrbh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/grxzsoabm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyitcxunm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gmvoxbbzd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/ggoehqdgy.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/guwrfnxyx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gxxnxqabn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gzbftokap.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gyotuysee.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gtdwwcjnc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gklxjwqih.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gxrmdqhlj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwckfxovd.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/grxmhaqmz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdilyyp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gwfhngjqf.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gaqervigq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gkyjsithv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaeejddde.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gnjsipnuu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvgfjkgpx.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gljdrcxtf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gqrxbchxo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gcwudjcvp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gxthnqkfx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/ganbpdvwe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gaemneifv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gbfpmqrkk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/ggwvpdyyr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gaqtzazfk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gvholoois.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gmmefxcfx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/glocflnfb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/ganqizqti.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gysackond.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gxdeyqxxp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gffzmrhzy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gpdyrzvun.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gojzmuujb.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gykdssqnk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/ggeekpjnu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gnltiviqc.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/ggoivmrem.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gvucxjmye.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gigydmtgy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gtwufskrp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gjblmpvcr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gcfpmfkao.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gugmrveqe.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gjulviemn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gddethypa.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/grqegngsh.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gfoawxuen.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gxmmbfwqh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gekcngure.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gtsgkdvgx.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gwmriwmgo.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gjjijmdjl.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/geedijvro.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gmrpjkylb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gnjccokoz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gtxdmuhkk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gfbmiwiiv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gbsmlzkny.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gooiceftg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gxtazilpy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gnykyfrui.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gmlcszxji.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gvfkvkvav.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gvcevrbru.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gahxsbyeu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gpjegypym.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gdzqvwscm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gulaohpix.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/ginwuuoic.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/glwbdrwam.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/ghapwashy.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/guxtglini.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gvzpigqmi.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/ghhomofbt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gtkntcqdr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/grewpedgm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gujkulvzs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ggqrhaoem.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gemtumasd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gsgvsnaje.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gqwxhxqjb.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gwkdzrxwa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gqvxhivfi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gjylcdirx.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gpdlbqtpv.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gfkcsvjmz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gnouskqqv.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/guvjugbxd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gfehzhudm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gdxivfubr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gvphtuyim.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gstphdxed.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gbnirbyvj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gyerdoqji.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gxrzovnfq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/ggoulsqud.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gryyhgais.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gfuznecan.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gquyhsxpy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gduieuxgg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gsakgxflr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/ghgnfovgj.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gpbgukrlp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gnuqjkqbv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghoaouklz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glibinxwl.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gevytctex.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gecwthlsi.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/grefhuitb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gefkljufz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gjumxwabq.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gmyeukhkz.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gewgoitsr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gpzpwfbit.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/grjaqjsdf.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gvzvxjduf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/ghcmmvhky.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gsorztkpj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/grkjnwpuh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/girweayah.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gfnkwtqzf.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gyqplmsfh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gdxknapxj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gdnjjgicj.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gozyzcamo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gczgcndhg.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/ghqcgzmus.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gmkvvdtqg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gxagykery.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gcvrkiioa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gciicgdxs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gjjeiwzqm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gfnobjpsz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmozdrtpr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gymtkionl.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gdhrxyvxp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gmebcvktf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/godczneid.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gahyozomx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gvbymruen.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gqfyewbqi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gwnlbajvy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gfneduefu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gjbcmmhxp.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gvvfietzq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gbyunrftb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gayshuzyg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gpoaqspkd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gdmbbewps.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gvhtxqgao.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gqklzxicm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gihtzdlaz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gopezgogb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gzfglfgrn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gruvbfwxf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gbdfxycof.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gjsbjytzj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gtvkzztzz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gsxngrsxj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gtizkckel.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gfxrqylhc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/geehrstdh.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gsdzlrpnz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/goircalrm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gjjfaiqkm.sHtML


<!-- 参考信息 -->