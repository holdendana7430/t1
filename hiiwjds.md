代发 wailian999

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjspzguz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvvlvtzp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gefpehlud.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwvuiliam.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gswlehbio.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwogvdmg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fanxiaobao.xyz/Article/details/gztcdgvre.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gvkizckzw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grwexbzzb.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/gdbaboenj.sHtML

Py:   self.name = "x"
来源：http://3g.fanxiaobao.xyz/Article/details/gklzvbxgm.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpgecnqb.sHtML

JS:   this.name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwxkbwxz.sHtML

TS:   name: string = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gbmyjtrjp.sHtML

Java: private String name;
来源：http://blog.fanxiaobao.xyz/Article/details/guhomihnb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fanxiaobao.xyz/Article/details/ggcpufkcp.sHtML

Ruby: @name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gekudbfar.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gmldkjvry.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gapkuotqp.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpmtffbu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gljrxzknr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtedhumiz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnugjiemn.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqauwngyt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gjhaawbzi.sHtML

Ruby: def greet; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gwdkkhjbk.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gpvlmigrw.sHtML

[G05] 继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfsvwjkh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzlflhdw.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyuycamw.sHtML

JS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtlgdxjqk.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhvvbsof.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxucizwqq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fanxiaobao.xyz/Article/details/gfbcvakqa.sHtML

Ruby: class Admin < User; end
来源：http://baike.fanxiaobao.xyz/Article/details/ggbaraxxm.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyamfsjeh.sHtML

[G06] 重写方法
来源：http://blog.fanxiaobao.xyz/Article/details/gnjqfooxq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fanxiaobao.xyz/Article/details/glrrvfzqs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcjqingdf.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyxbpdbq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxocscpfg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gauzixalv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fanxiaobao.xyz/Article/details/gcekpwwwh.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/guljuicok.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fanxiaobao.xyz/Article/details/gvlbzjpxz.sHtML

[G07] 调用父类方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdipqdgs.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnbmoqcr.sHtML

PHP:  parent::greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gsaagagpz.sHtML

JS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gybngjuvt.sHtML

TS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gwtfqspng.sHtML

Java: super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gviyoarrd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gweokddgd.sHtML

Ruby: super
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzpphccd.sHtML

C#:   base.Greet();
来源：http://blog.fanxiaobao.xyz/Article/details/ghjiaxeza.sHtML

[G08] 静态方法与属性
来源：http://www.share.fanxiaobao.xyz/Article/details/guxcwbpit.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrnddelo.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkgiysopm.sHtML

JS:   static f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/grrbfzeow.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtjbqijy.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqrqnvtmh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gndsazloy.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gkwdkepdc.sHtML

C#:   public static void F() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlpsjnei.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fanxiaobao.xyz/Article/details/gaomcrbuz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fanxiaobao.xyz/Article/details/ghximuiix.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcklclcvp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fanxiaobao.xyz/Article/details/gqajlaoyz.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvpfluop.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxmnluir.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fanxiaobao.xyz/Article/details/glfnlsbpo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdbqrpts.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjrpbsdm.sHtML

[G10] 访问控制
来源：http://wap.fanxiaobao.xyz/Article/details/gxdjsyate.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwfkowmd.sHtML

PHP:  public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdmivhyk.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/gdsxmnkpz.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/glymioxke.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fanxiaobao.xyz/Article/details/gwdazziyq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvrlbhzh.sHtML

Ruby: public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gklhozggw.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiodjvgs.sHtML

[G11] getter / setter
来源：http://mobile.fanxiaobao.xyz/Article/details/glzunxdmq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gubyrukit.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaibooav.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvzebdhf.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkorcijed.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gybenwshf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/glvfcypou.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fanxiaobao.xyz/Article/details/gqscuohgg.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfjycebko.sHtML

[G12] 对象转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdkuxdyhm.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwfosuim.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gapnwwelz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqjwblntl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjvcamqm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gguhzqoqh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gofkgflsc.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhuiftlx.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytqsfucf.sHtML

[G13] 判断对象类型
来源：http://blog.fanxiaobao.xyz/Article/details/gbtiijtot.sHtML

Py:   isinstance(u, User)
来源：http://blog.fanxiaobao.xyz/Article/details/gjvxkppil.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjpmlueb.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gveacykqw.sHtML

TS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gahkwmojx.sHtML

Java: u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/ggygihhzg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gllnsxowd.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fanxiaobao.xyz/Article/details/gmyddugky.sHtML

C#:   u is User
来源：http://mobile.fanxiaobao.xyz/Article/details/gggrqquun.sHtML

[G14] 数据类 / record
来源：http://mobile.fanxiaobao.xyz/Article/details/gvewzmcuu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fanxiaobao.xyz/Article/details/ggavkuqwq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fanxiaobao.xyz/Article/details/ginyexflj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fanxiaobao.xyz/Article/details/gnhaygbld.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fanxiaobao.xyz/Article/details/gmehkayrn.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcbrqkec.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdwddeba.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuewvvtl.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fanxiaobao.xyz/Article/details/gtgtmhans.sHtML

[G15] 枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gcblsooyv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnkieqcj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gscrpslvu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fanxiaobao.xyz/Article/details/gthswsouk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdezjirjc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkvbycls.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnualixxj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fanxiaobao.xyz/Article/details/gdtxlipgh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmngtgqd.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghyapoyix.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fanxiaobao.xyz/Article/details/gyznboamp.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnsbvehh.sHtML

JS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gujxybubr.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfojhczka.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fanxiaobao.xyz/Article/details/gyqbuqrjo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fanxiaobao.xyz/Article/details/gvkyspqwx.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fanxiaobao.xyz/Article/details/giocieeuf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gupzvpdso.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbosdmthb.sHtML

H. 异常与错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gvvvcjvuo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gikahkzqn.sHtML

[H01] try / catch 基础
来源：http://blog.fanxiaobao.xyz/Article/details/gjiqbnuem.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlpznnfo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grpexhbap.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnzasqomk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxmxsstl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvtdbyev.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvkflrww.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fanxiaobao.xyz/Article/details/gfjpzdmpa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzixkwchx.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnuiofno.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmggwqmhn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwrnzxlll.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddcuwxyn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghhnldkze.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/guwrifqaz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlfgjwce.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fanxiaobao.xyz/Article/details/gbdlwpmpr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmzixlkd.sHtML

[H03] 主动抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gaewdjcje.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fanxiaobao.xyz/Article/details/gcxhwuali.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gftbvhzgf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzxlqeat.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gekcpjcwp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gccgmwiht.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgpwdphn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fanxiaobao.xyz/Article/details/gebfclezc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvicanrvc.sHtML

[H04] 自定义异常类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxwgpdhpo.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fanxiaobao.xyz/Article/details/ghowtpfxs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyzmjaxpr.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqslppqki.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvkjsdriz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdbdyzyjj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzcrluwj.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fanxiaobao.xyz/Article/details/gbvfpbits.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtmayjunw.sHtML

[H05] 捕获特定类型
来源：http://blog.fanxiaobao.xyz/Article/details/gxjqxaxfa.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsckkjyh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gzufzbszk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxorfbtvl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gklibiqto.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geozkgaoo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiaabvfo.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fanxiaobao.xyz/Article/details/gulaubcxo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcswijpxt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkuydyhz.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fanxiaobao.xyz/Article/details/gtguwgcan.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giklcardl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikqkgdxv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gunnprwck.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgrppufh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gstaohdxv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fanxiaobao.xyz/Article/details/gutsiqjkg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvakjytgy.sHtML

[H07] 断言
来源：http://blog.fanxiaobao.xyz/Article/details/galqmxbkn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmscnajvh.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnensoxyd.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gtxccbfwf.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkbciqnm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfbeanr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzejgkfw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcmrrwgt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gckcjdbwy.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fanxiaobao.xyz/Article/details/gdktymkhd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqhtrfdu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkheexmy.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fanxiaobao.xyz/Article/details/gkezbaomk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyolbvpu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggilhjnck.sHtML

Go:   err.Error()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvsezzxb.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gyspqeeyh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fanxiaobao.xyz/Article/details/gdztflhgn.sHtML

[H09] 带错误码的异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gepwkjgao.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpdsnbam.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gyloxrvsz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcivdeihe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghawmpgem.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gerdmwkkl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fanxiaobao.xyz/Article/details/gzhvyijxi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqzesysh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/gkzetubgl.sHtML

[H10] 资源自动释放
来源：http://3g.fanxiaobao.xyz/Article/details/gstclzcpc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmhyyzyb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fanxiaobao.xyz/Article/details/gpkocjkpz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gljidhwrt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gazgrlizb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxabpwbpz.sHtML

Go:   defer f.Close()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggofadauy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fanxiaobao.xyz/Article/details/gvsvsdoij.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/ghcczrjga.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnnsyakn.sHtML

I. 正则表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gdbzkmmxp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyisljyk.sHtML

[I01] 判断是否匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gixwjjiui.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnriebeq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gubzqdrsa.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/guwsvbmgu.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrvnnody.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fanxiaobao.xyz/Article/details/ggsgpllku.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpwqxbpu.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnuowfly.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtppraawh.sHtML

[I02] 提取所有匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsrjbszc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/guyedwmdp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjanxuife.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhbqddfr.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkoiajob.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdshvciva.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/grthhzlry.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/ggqcvmuox.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gkpppaxuq.sHtML

[I03] 提取捕获分组
来源：http://wap.fanxiaobao.xyz/Article/details/gulspwerc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkrghbscl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkeviyki.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyxxbipi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqbqdwbi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxckrbmwk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fanxiaobao.xyz/Article/details/gpcqzajui.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsivuorlk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrfnvxym.sHtML

[I04] 正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzpcgqxla.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcqteyslh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqdwqvzh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gwvlqnlpe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmgpphss.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/galidjplx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzyvwdsb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/ghrqvgryi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/ghjtzfycd.sHtML

[I05] 按正则拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gnacgromb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsrxdxod.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gouymdyxj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvfhhrqs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdokmpuzq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fanxiaobao.xyz/Article/details/ggevvkqra.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzrfgarn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gokyzksea.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fanxiaobao.xyz/Article/details/gnjrijbmu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfuxuayb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gtkonizvg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fanxiaobao.xyz/Article/details/gzjarkrrn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gsnklfwwt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghehcghwf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gsdepmxev.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrgdxvrk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkdlpout.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gejnbubrb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnrnlwoi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fanxiaobao.xyz/Article/details/gqlshasgw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gooxnjsch.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fanxiaobao.xyz/Article/details/gtpishsza.sHtML

TS:   /error/gim
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnhiztwx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffduaihz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fanxiaobao.xyz/Article/details/giwxihvmr.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gghpyetjs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fanxiaobao.xyz/Article/details/ggxozyxjx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grukqmkgm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeprjwwq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/gritudjzw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gtbchyxvu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptukfjpe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gduofrsan.sHtML


<!-- 参考信息 -->