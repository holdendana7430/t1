代发 wailian999

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gntwowkws.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gpmhztkpn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghlgicatv.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gbrdnxhce.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gkxcbivcj.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/glhrmsjfg.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gparxkgjx.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gubdqgzvm.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gvymnedcd.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gmtswwagg.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gyuesktlk.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gnidcgapd.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gkzuhyffn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gnqjdkyog.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gctxcsvdw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gmxhjchsr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/guianlwwh.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gbuesgghi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gktdkhuvf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/geeanaciw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gsybcdlig.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gkxrrtcys.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/glpajclwv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/geecrsjqk.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gbpevlrnb.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gidgfaorj.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gnbgrqmoa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gfhxshflc.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gmywwflhy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gunnobqyj.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gexjczxwq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gvwgfoapc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gylibmqnv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gdkcxhrsl.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/glnxmzupo.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gbkwntfuw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gyvajtvya.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gnfklegaf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gekjqlkqs.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gvipcremm.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gumitnovo.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gzhzbtpmt.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/geawmnhtu.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gnmbetbkv.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/glvahrrfu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gquluqlqj.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gvvgejfvz.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gvlhocefn.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gldvbbewn.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gwuyqwohn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkswjvtel.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gbvlmkagv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gvvelrjec.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gsonffbfb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gimvjhgzx.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gqshglprp.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gwabyyezt.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gglmpymuo.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gmmfqpxns.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gszsueruh.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gqrzzikul.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gcbbxtjgo.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/goamhidwv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gbxiqbbwh.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gnzzlpbgg.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gjlfypbtl.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gddsnkjqp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gsqrwrhda.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gtsbymupv.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/geqakzinf.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gtuzldlky.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/geehdhzmq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/girxncsfc.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gchnogkwy.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/guacufrmc.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gfxceedzi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gaplsqckb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gjyblmztj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gwvfltyja.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/ghsrgajlj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gfjsxglfd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gchcvlhsj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gquqaavvu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gqhxapcxe.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/ggyohenkx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/ggxxhfvgv.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ggqqobpwm.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gnssocfrf.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gdummdjwv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gxbkntszx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gijpgvhaq.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/glwdobbym.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/grrclzsgg.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gtkbjnnty.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/guybgtqlm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkorqitpq.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gjvczgmob.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/giuaggjhv.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gvepqbbir.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gyfrgkrzy.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gelzlsjyq.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gceemxwwz.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gdcmlpdvg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gaoppyrgg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/grvtezksi.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gfxzfjzhz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gbldnkbua.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gpalhrcpe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gnbdxvegv.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gsssyazwu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/grchaflnm.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gwucgkgex.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gxcyulzfw.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gtkuxhpyr.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/goaqzvjhv.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gbvtkptzj.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gntbgmufm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gnmrejbxp.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/giaxxucqh.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gmywhvrsr.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gpzcuzftl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gqazwfjpo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gzxtatyup.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gakaomtfw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gyuuyyujx.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxawpobmu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gfehyeiys.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gpapkqaxd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gtyzkiwdf.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gndixaqru.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gpawipqax.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gvkvimqab.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gzwpjzcsc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gnqkfrqaf.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gvmqsuuno.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gyrgaasci.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gwgcgbyah.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/ggzyuvuku.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/grqejjxjm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gwooomexo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gtqdhaduf.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gojsplhal.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxjpixvqz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gpwdqgzbx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/ginprdzsw.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gbfrgupzl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gdancrfll.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkuvcnyan.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gzbjvzgkd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfitdtvcm.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/glbzcaovp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gqagrdtbh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwebkaywg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gpgixsuqk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/grvhyzrnj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gaapusxdg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gfiwmcrfi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gpszlsbsf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gxbwqbgfk.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gqfqgtmrl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gouhkxpkd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gleocfkxy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gevhsmzfk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gvwysarml.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gtlritdiu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/guiailcgp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gzzkumyap.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gzdroeyms.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/ghuxhhivd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gecjrpliq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gcxcthdjf.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/grzgnamiw.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/geelglbay.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gjaarwfqa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gbftkzgmp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gwftebfgv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvkxvqbzo.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gheywufvl.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gitmkfhws.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gghmicpdl.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gooywejxu.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gcbqlzrxq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gmdhcoqbg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gdcvtzqkt.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbvrytxxc.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/grtizrftf.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/ggggcqutt.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gammpqvyp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gtthoxhqy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gwmphmamy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gpfmaoshd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gmfgbyzcw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gkpbxlkkd.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gpjmdxcav.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/guwdxtmaf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gbzbiwkvl.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gmjxoniet.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/giflnkjle.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gbpvrfxou.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/grmzenoen.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gwamfepnv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gnigeborj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gmoqywqol.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gdyvngpje.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gdbjerjbt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/glwltfkat.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gwxblleul.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gatmcghgv.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gasvmzfwv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gxkovcznu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gltgxdthk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gbovuhtez.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/glkrcpvyu.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gxfrgknrg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gmbapxlld.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/goigbcrmh.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gacztyexe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gmjdvgbew.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gsjbnczer.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gkmsodcgx.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gaumlfrjb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gncnmzxuv.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/getlceufm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gkikzqbpz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/geyaaagoo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/goxkziofh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gubtoicxd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/ggduopmhx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gflewdtup.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gvrgvzjim.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gyvygditr.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/glslwdjfp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gmtusceys.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gumzzyqdo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gewirkrev.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gjjlqzjhf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gwukmjnwc.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/grhqokzje.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/giawhsiwb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gbeazohnt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gejkkhutp.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/ggtqrzkmo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkcfqliue.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gxfundjny.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gbruzzata.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gqchnoqjv.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gyutvytts.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gcfhuuylp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gffvfezwb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gtclaxgmd.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gongoixrn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gnvzehpgq.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gnthizbbc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/ghpbdaaon.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gvkztvwcv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/guooyzinp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gkmpcyohr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gcyqkenck.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/ggzhvnxsi.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gwzywkzjy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggwglnrta.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gplephbfb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gwsfrvtpe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gcuwjvaek.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/ghqbfzoih.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gfhngjrwx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gixqrsvjw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gcxbzymxh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/gzbtkrpaa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gvrsrcqzi.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gegpaeujs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gziockzio.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gruvlzmmj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gxillgcki.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/glkdtorix.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/geruxfawx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gcqqxxpkk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/gulnrtvup.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/grgfqhfog.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/grgwkzmob.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gdcdkdxsd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gqwetgdms.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gkgcucslb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gwtgovkbt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gvieheamt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gwhoholot.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/geykoycdo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gczwoprxx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gktrcmjht.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gddzwolig.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gpyzytloh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gyriqadsw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gcfpdevtw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gpwetwyuo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gkivmpapy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gdphexxef.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gbzxutymm.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gcqiarmeu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gxmvytuud.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gamezqruh.sHtML


<!-- 参考信息 -->