代发 wailian999

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcxlfogo.sHtML

PHP:  class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnugdejn.sHtML

JS:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwnlqvjg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdebsrwt.sHtML

Java: class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeuyimin.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/gimwyrbjj.sHtML

Ruby: class User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobqncrde.sHtML

C#:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gumyvqywv.sHtML

[G02] 构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfdjyywr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmnmfwrf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjynewsln.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafbnufmm.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fanxiaobao.xyz/Article/details/grarclave.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmvabqwz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fanxiaobao.xyz/Article/details/giejculxi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkejtces.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjutrchvm.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/gcwmgfeic.sHtML

Py:   self.name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobajeswt.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gymfptsfo.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gbxtgvrkp.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyuuqfwj.sHtML

Java: private String name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykfxjqem.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fanxiaobao.xyz/Article/details/gncujbntu.sHtML

Ruby: @name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuemfsot.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/grrolovuq.sHtML

[G04] 定义方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcmgqcxm.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/gembcvlkf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsqnohctl.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeegexnp.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzbcwhhuc.sHtML

Java: String greet() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxclabhua.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/ggqurltsn.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpgmeehg.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gquoocrjk.sHtML

[G05] 继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gaybyyeph.sHtML

Py:   class Admin(User): pass
来源：http://3g.fanxiaobao.xyz/Article/details/gsbgtoswo.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gftzwpknu.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/guhjsyzwy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gndgjnrxd.sHtML

Java: class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggqydztml.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjtrzemw.sHtML

Ruby: class Admin < User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gywbqghgc.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyikfeqd.sHtML

[G06] 重写方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrbhvrog.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grogslato.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkwwclwm.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjscupdc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grprpzrym.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfpjtecl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fanxiaobao.xyz/Article/details/gllqbwdtk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtvwcalv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fanxiaobao.xyz/Article/details/gqbjdihew.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcujfqhda.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgthxbac.sHtML

PHP:  parent::greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqgrrxnr.sHtML

JS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbpxvvka.sHtML

TS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gesvhbcal.sHtML

Java: super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/grkajohyg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gamujxqvg.sHtML

Ruby: super
来源：http://mobile.fanxiaobao.xyz/Article/details/gknpxnsnd.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gdugnfpql.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsfosell.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fanxiaobao.xyz/Article/details/gbctwymsz.sHtML

PHP:  public static function f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gusixrgdv.sHtML

JS:   static f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gunpcxhjf.sHtML

TS:   static f(): void {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsphdypg.sHtML

Java: static void f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfonlgbr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghigaeuno.sHtML

Ruby: def self.f; end
来源：http://baike.fanxiaobao.xyz/Article/details/gwkosnaux.sHtML

C#:   public static void F() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhjkkstx.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fanxiaobao.xyz/Article/details/ganznxzsm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fanxiaobao.xyz/Article/details/geofeliqb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwnxorrr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhkjwzjk.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gahiowyfb.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/ggagzkeml.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwildbdl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fanxiaobao.xyz/Article/details/glawbuclj.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjqyglyv.sHtML

[G10] 访问控制
来源：http://www.share.fanxiaobao.xyz/Article/details/goyngtdny.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeuufznr.sHtML

PHP:  public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gulwmcdlg.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/gkozzfcbg.sHtML

TS:   public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/goybuzmtm.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fanxiaobao.xyz/Article/details/gapnfkuaw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fanxiaobao.xyz/Article/details/gclyobryd.sHtML

Ruby: public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqhmaulm.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhozouoy.sHtML

[G11] getter / setter
来源：http://baike.fanxiaobao.xyz/Article/details/gzhepmyyl.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnqcdmwr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnmqkccfv.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzatmnrvx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdjsilby.sHtML

Java: public String getName() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfxbnkymn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gayciagpo.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlwmzvts.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnefxocg.sHtML

[G12] 对象转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grecbfsux.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/gevvctwrn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gunyeycud.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guoahcgis.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwmivjrz.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwfwbaye.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqybwojx.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gdzijjoif.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fanxiaobao.xyz/Article/details/grrcypmzp.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gqzzlxpgd.sHtML

Py:   isinstance(u, User)
来源：http://blog.fanxiaobao.xyz/Article/details/ghzfxcfwu.sHtML

PHP:  $u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/goyfrolsp.sHtML

JS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtojcsfml.sHtML

TS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyeuievu.sHtML

Java: u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/geoozknni.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fanxiaobao.xyz/Article/details/gnewwuskq.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gynxyehjg.sHtML

C#:   u is User
来源：http://3g.fanxiaobao.xyz/Article/details/gjdjgoxfg.sHtML

[G14] 数据类 / record
来源：http://blog.fanxiaobao.xyz/Article/details/gpbcfmbup.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwomqxsfm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fanxiaobao.xyz/Article/details/gcgzurman.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fanxiaobao.xyz/Article/details/glbkkylvv.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fanxiaobao.xyz/Article/details/gwwquzkty.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafwfzoud.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuzxetbu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpqqfbuf.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fanxiaobao.xyz/Article/details/ggxzodwiq.sHtML

[G15] 枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsvxqhrh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvlmckict.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghphxzdrm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fanxiaobao.xyz/Article/details/guoluuqub.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guszbwhtq.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fanxiaobao.xyz/Article/details/grmjdhkhi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjecrofwl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fanxiaobao.xyz/Article/details/gopwehvwh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvkokyww.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fanxiaobao.xyz/Article/details/gpygquojo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fanxiaobao.xyz/Article/details/glqzbmoro.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqldntki.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwhkbmqx.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwooayaxc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzouwtbkm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fanxiaobao.xyz/Article/details/gccfoosvs.sHtML

Ruby: obj.instance_variables
来源：http://baike.fanxiaobao.xyz/Article/details/geuyizvbt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/glcvpvcdu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gazshdfkw.sHtML

H. 异常与错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gprcbhtle.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnrxljwp.sHtML

[H01] try / catch 基础
来源：http://3g.fanxiaobao.xyz/Article/details/ggspdleln.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfxoprha.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugjcygqx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gdkrpcyth.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/grtryzerz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/grkotbpgm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gafirausm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fanxiaobao.xyz/Article/details/gkptrtxfq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gegzggdoz.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlvyzriv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyxcreef.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqlvaxdd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmzhittp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlweqspz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyimxfvif.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fanxiaobao.xyz/Article/details/gkbbsgsyr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fanxiaobao.xyz/Article/details/ghlgxznxi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghnejvwtr.sHtML

[H03] 主动抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgpkwejw.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fanxiaobao.xyz/Article/details/gfiabcjbz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkclgfybe.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gidszidls.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gixvvfebg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gsfrurolv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpyjqfnx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fanxiaobao.xyz/Article/details/gkwxaeyfo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gfuqiecua.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbohufmky.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fanxiaobao.xyz/Article/details/gmfewkaxd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrnpigse.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guozfrsky.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqzkbiqg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvkrkrgr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqckjpusa.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwimcoim.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoexmied.sHtML

[H05] 捕获特定类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkufbqac.sHtML

Py:   except ValueError as e:
来源：http://blog.fanxiaobao.xyz/Article/details/gwagugxbq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtespmnzo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmjjuccyz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcblfyoxz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvwwembdy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fanxiaobao.xyz/Article/details/gbmdnddbb.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcgllaxd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcjquath.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrzngxue.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlncbugo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gvuynxstj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gonlpeiap.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/geisshbrk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fanxiaobao.xyz/Article/details/glirjwxtv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhmedgww.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fanxiaobao.xyz/Article/details/grcgqmdnt.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/glkcwzvmk.sHtML

[H07] 断言
来源：http://blog.fanxiaobao.xyz/Article/details/ghqiprzhj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fanxiaobao.xyz/Article/details/glurmsahc.sHtML

PHP:  assert($x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/grgintalg.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqokjggk.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/giwoqdfmm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fanxiaobao.xyz/Article/details/gktkctacr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fanxiaobao.xyz/Article/details/gycfmtgww.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmjnlmrt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpbvvtgf.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fanxiaobao.xyz/Article/details/gzbfvciot.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhnlstsu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fanxiaobao.xyz/Article/details/gqcahiheg.sHtML

JS:   e.message;  e.stack
来源：http://baike.fanxiaobao.xyz/Article/details/gmdrknned.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrtpvvtx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fanxiaobao.xyz/Article/details/gezaxhbll.sHtML

Go:   err.Error()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlsuohqo.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvpucylr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fanxiaobao.xyz/Article/details/gspqnctmd.sHtML

[H09] 带错误码的异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gggnvurjm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjfuudpx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/ggfjgjgum.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqpsmrth.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgbmsjcv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gickeosqi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gctqnqluq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fanxiaobao.xyz/Article/details/grsxrpbtf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/gmltreldn.sHtML

[H10] 资源自动释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gtideribw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/gpnbpqzqb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fanxiaobao.xyz/Article/details/gamhglwgi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyoljmvf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqtirjgs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/gvofzlqdt.sHtML

Go:   defer f.Close()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxtzcguu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfrhzicy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnrkyqdr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcfjowkj.sHtML

I. 正则表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gposkjnyp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcswdixbd.sHtML

[I01] 判断是否匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtzwrprj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjipzyvdi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghneujpyv.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/glypstjws.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbpnumnqx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fanxiaobao.xyz/Article/details/gniithcgj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gswoybcep.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcizkxaye.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gjzhlnzyy.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/ghdkzikkg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaigvvpqj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvcszkya.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fanxiaobao.xyz/Article/details/gkqdmyoxu.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvndkyaw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqrqcwfb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggnfhekyb.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gvkktgmvk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjsnhwju.sHtML

[I03] 提取捕获分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrggrqfj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtovhbjn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxldvjpt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gkklczyuu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gknvnorfv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/garbkezpf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gthpctcac.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdyyuxga.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzqgjuvn.sHtML

[I04] 正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtyfsusc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gqnhxgwil.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvwmfdwi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gcnimsusk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/giezklecq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/giectrwsj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/glttutgaw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/glwtbebym.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gypwufrub.sHtML

[I05] 按正则拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcnhypzl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkrswrtef.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gllvoxjai.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gdsfofpzs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcqmdlkv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkffvgfxm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsnqxsrt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gvxgpukch.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guladkrwk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goegwquyc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gpjmrhwht.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscbtygpw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fanxiaobao.xyz/Article/details/gvwimivbq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwtjzybu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gzzjkuybm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fanxiaobao.xyz/Article/details/gjabdjhrv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gjghqpdnt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gzdeahfbn.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhnkztkx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwayozhbu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/gazqauner.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fanxiaobao.xyz/Article/details/gawaiopju.sHtML

TS:   /error/gim
来源：http://baike.fanxiaobao.xyz/Article/details/gheqyybqm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsfkvrhl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjodmuou.sHtML


<!-- 参考信息 -->