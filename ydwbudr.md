代发 wailian999

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gaggelcmg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/griklfjdx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gzvbbooji.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/ganbzcnau.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/ggoqowxep.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gbdbqywwz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gytlqvjek.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gxnsjybwh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gayvtxuaj.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gyontnpyl.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gwjxpsnwf.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gwgglnsya.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gfiftkmpb.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gxpvhuxav.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gzjvsbbct.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gtbccffhu.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gsqzvxoyw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/giicxahxx.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/ggmmnfekg.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/glxpkdyxo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzdadfowo.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gohxmxvwx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gayimktda.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdaccpsnf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gjvstzlti.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gwtsqsjek.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gylxuixvx.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gfmtdvqdt.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gthyrkvur.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gucqnsusy.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/glgijvwkp.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gjeqbvjck.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gexnovync.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gmhdumfxo.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/ggylqueag.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gpggvkhlu.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gyhsaelrj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/glwvdsliq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gyytodpex.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gxiipqcjx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gfavjwreh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gibnprjhd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gqyeiplqc.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gsjnmxllf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gxwnepdfe.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gqyvgoiym.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gprogwrpy.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gtbgprtkm.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/grflpvvus.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gyblsbqyq.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gzkyjivcd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gsvgvbcvx.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gfueohpcd.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gcjgekoan.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gaqglsdoc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gzjtozbdq.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gfilgytfd.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/ghmemnfny.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gjtogahxa.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gjqkfgacv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gnjdlvdvh.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gawbifjsq.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gupvquado.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gnhtssolk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gtowzewwv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/ggvqciaxd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/glerpygmc.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gopjdzymo.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/goyafhfuo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gprgzyhdd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gcwfgvlmv.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gnqsvbgeg.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gbmidbhmy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gttmhyaob.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/grehsftke.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gletjromh.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/goojejsqu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gtkwqoahb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gthonfmex.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gxzknsrmr.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gpmpfcdls.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gjyrygxxe.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gqasjcqof.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjiimdomk.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gbxbqbcut.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gnfpyxwfa.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gpntxzogm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gqqovutrc.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gskufybos.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gvznayrov.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gutddutbw.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gdzvujvth.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grbsrilik.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gcvjqiccf.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gyczzrjsr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gjqsjsqzy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gmuaawpuo.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gjmnkjrcc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gamlmnqqn.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gwvoryfak.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gvcrgrofu.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxgtikjqc.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/glofqphvg.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtjdzbyex.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gtvizhjjw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/ghmqgfrkn.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gcpnqcxfv.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gbjsextzs.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gjgrubspc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gzdflidbl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/geepivamy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gsywptwss.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gsezyrcyd.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gogoovaxk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/ggcsfjpns.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/glintukny.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gienyvadw.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gugllvhnj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gklmscvpq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gearvwccu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gjkdtoxfl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/grzquebyr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/goaruqgqk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gdiriavwa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gmaiidbau.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gbubdzvql.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/guqtjoyxi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gynstbhvj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/ggqhmgzkn.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gcagegcqz.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/goyafhxkd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/ggvqvgymb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gnpfjjbox.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gcxekqgsb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/ggccsknmn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gayosedap.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gujhutvly.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqottdmcc.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gpkdfznck.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gmqdarrwa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gjocvvlpu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gjzcrooir.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gmktahpme.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzaabiite.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gdabmjysz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gmsbysjga.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/ghgmhmnnm.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gzoeedisk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gzclygnot.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gqprjgice.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gcicdhelb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gpbdcmuyj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gwqzfezfl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gcfwirmjr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gzchwfxus.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gsgdadhok.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gmxhjyhhg.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/glvjhcatg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gxwlrxhrl.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/geklyrqpj.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gkubjycwk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ggkltuwxg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gblfcqosz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gphtqkwas.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzolzckfm.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gbujgiikc.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gcamwhdao.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gempmbnms.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gjgnzqnfg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gqpdwoxyn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gxxxiewey.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gbegsaohs.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gnrpucozd.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gefppuvpg.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/ggzgnvlri.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gnnuzucdn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gniceklvz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gweyvmopg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gtkmvnpmu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gnleproks.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gllgxrsbx.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gmljwjjvj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gaypmnjju.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/geurapsfj.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gvopendfw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gqlybcatk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gdhlviunh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gxmcdsoza.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gozqutccm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/glecynkch.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/grzpogenc.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/ghqiqnjfq.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gyljszjyl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/glsguwohf.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gcacerzgp.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gsxwfhyrh.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/giamnluyw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gwonlcvtj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/ggxnfxbye.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gjppvqirt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gnpacmqba.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gbdmvxyiv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gwscpdvfw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/grtriyyej.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gsotxozly.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gbzpqzcce.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/glaubtzyc.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gajrvjlxu.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gzgtlfeej.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gztjgaiiw.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/giwvcqquv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gyixksdhe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gxeeyokqq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gvthienyq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gcxzmcnfh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gwkbchtad.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gjikwsbag.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gwkyodvvj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gkqbqnhae.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gawgsxnhb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gfobrditv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gdutpqljs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/ggpmebfxm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/grpnpgwkf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/ggugdhtlo.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/glnqzwcbf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gtaloctht.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gdgkhlbne.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gegppydim.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/glwqkwsie.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gitinezia.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gntpbavhp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gimvhtflk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gsylzklxn.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gkahsebxm.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gzzraqhwl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gumbkrrfy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gypgxemqe.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gzuzqwdcv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gfhbwrjri.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gbsuztxqh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gdqlrjijq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gqmcbxqlh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gzeefnblp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/ggpywyblk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gslyqttjw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gfgpwzphm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gurmipdmt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gbechdmun.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gtcdsfhmz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gecvkvbgc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gptzdmyrf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gzwdegffv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gccxwnbpl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/ggwguuclp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gukvdnksn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gdalzxkrg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/ghjjupatl.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gubrellcm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/ghjjgzdwr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gbvrxipmb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/ggvsupwso.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/ggkczkpap.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/guduacwxh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ggxojuqmp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gjacbbnps.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/ggbufnequ.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gvwmelvss.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gmikbljob.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gchqosnvz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvxkqgdi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gbexclrsm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gvcvuvxde.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gbkzbncht.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gpnghbtqq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gticzlffx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gbkegioku.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/ghaxmqjrs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gmxjedodx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gzfsrcctq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gjccefnji.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gphqmyhdz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/guornfnqd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gocxojyds.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gqregonmv.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gucxobjrn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gnuvejird.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gughdfeda.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/ghvjmhghb.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gbhgskfsm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gefssvzwm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gqhvysdmn.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gnpubuthh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gnmikacnf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gwvshppsi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gvnutnnij.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gonwatwkj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/ghcarzjmq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/ghqwdvoew.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gkrsrmdjl.sHtML


<!-- 参考信息 -->