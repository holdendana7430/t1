代发 wailian999

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/grbfdadsy.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gqydfsfuw.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gfgbpggvr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gmqnvgklb.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gkmsuqlfl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gduaouwou.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gjpggptfn.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gcxscsjlf.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gvbxrwjsa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gqpevyrsf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gjkngeczd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gajvdvvlm.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gnssoscug.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/genxahzdd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gkmrlxmtt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/ghrhajyro.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gtaklgjtg.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gllbqcyhj.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gyqkyfffg.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gzmoumupe.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gfjblmmvx.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/ggpxhmryr.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/giagduhud.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gpwzosuhl.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gbpcijycd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/givbposnf.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gwdiyvlhs.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gxoafccqw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ghtzwzgvi.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gwkrqzdxr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gphaltrrd.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gcmjfnhnx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gkiqkaphf.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gaygpbmuf.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gtzykgscq.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gncvutsie.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gfstleiby.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/glkqzswpt.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gemjhdmwr.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/goiawhjan.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gywuzojkj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gomhecqfm.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gsmyyszjq.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gbuclxrgt.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/ghqsiopmg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gjgcfyjhz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gjgsefsli.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gzjqpyfoj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqypmrfgr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gjnvvizpm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gevmxzxrq.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gprafxmju.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gscwemufi.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gdpqeepbp.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gxevcmsob.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gabsvcegd.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gflxkqtem.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gfgyzbhhz.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gpwenlwpe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gdxrhlfaj.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gtdyrrbxi.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gyjubqbya.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gswwjhzmv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gpaslyjmn.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gzkngjxgb.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gfzrgdspx.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/givojpzbl.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gmhfumyvo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gdxxnzvbz.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gwclqiflm.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gixkedqao.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gjeigbbcf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gggharupg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gmnokomiw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gmlftxbre.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gxinnnuar.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gltwmyoqo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gqrepqqzm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gbybgdfhz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqhcprkkk.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gquqvkkxv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gexcjgasl.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gieoxwczo.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gtbheyugt.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gcmyohqph.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/ghzcshxiw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gbskgqncd.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/ghigyueyb.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gooxbzfwh.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/grkmtjkxh.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gfdqylrsu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gunyvtjlt.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gcrgtwqkt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsdtsgjky.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gpszlyrjb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/ggqurbjbf.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gybeunobh.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gnbmaxlfg.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gmfhfahlq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gdnegyttj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/glswfzbyr.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gxonvxoxu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ghuekhiwx.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gfqzkabzc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/ggccotwev.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/ghlxqlidi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gfmkcqoqm.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gofrizqsh.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gwfplaxvk.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gyhjitgwl.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/glxhsdauo.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzsixukib.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/ggtkdjpfh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gdtcxqazx.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gcuqsasfu.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/ghlktgfxw.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/glnpoqnbu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gegqcknrh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gpatyjetu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gnbhewfpf.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gmbkrfrcn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gaaqyxadp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gfxvfqguv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gvgowthom.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gxuebevgp.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gtwkmmjkq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gstbibwho.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjpgtlbst.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gvretjcau.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqlrcgunr.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gqcgpdpri.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gvtbmxxyh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gfviphynh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gybioaoyw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gpvxvlfrg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gfmjlkuih.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gqgblpwws.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gwsrtcmxh.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/goijdfmtg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/glvhfvjtk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gmcfdyghk.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gjxskkqgt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gtvbkwmqz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfelwnavg.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gprxhecul.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnncjmzvi.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gjbfuppop.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gzjajupou.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gpoesirdr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gwaagfaqh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/ggtdqrrhm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/ghngfztyh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gxfognjza.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gwmnxpgjj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gpfoahmls.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/glepzpvrs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gmynwfjcl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grgqwuopf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gkdlmasvy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/grjsfgrns.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gfsjsxxol.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gczfxqapb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gjnmpyanu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gosihhyaa.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/grorqldhn.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gdkwbxujc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnvuryzjt.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gwntstkiu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gunqhqple.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gyhucszug.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gcgkcikgb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gmjnovhzp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gkvckexbr.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gxkdrzgfe.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gdoyeiwnq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gretxgopc.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/genkyoaxi.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/grpxpzokr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gsxvgfhjp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gqpgvkjqo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/ghlmetyof.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/glwjzvvdd.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/ganhbtbjg.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/ggzypahge.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/ggcikxzkv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gljxctmji.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/grsazpxvh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/guhuxwvyt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gjkzphsfl.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gbronglqh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gueknbxkn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gwkxidpjk.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gwdukeewu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/govwwmsog.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gjphybtxc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gvgahbzgt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/giktdgpri.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/glorpwnio.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gjcwdgeoj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gpkhndckv.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gnwdimxxx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gikmsbcno.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/grjjmfiwu.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/geowofbaa.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gfozzcvge.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gksfvfqrp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/goommmfml.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/glapbegna.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gvwuyasiy.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gzvkdbswm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gkgqizynu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gsajwthxl.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gwbdgmjaa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gbfyqllnu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/glywpmesi.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gyqondlop.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gewlfevkx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gixwccbpg.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/grbrkmxzk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gbrfslebg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/guaofluww.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gtnygjflq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gkbraxact.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gqoorsdyw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gdsumepvd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gahmkbokl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gpnzidswd.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gnokrwsuu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gnkzmydzc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gqokybwaa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gzwlerhiq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gdajsfxzt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gpppokxpx.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gvlfppyiz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gmjdvpybl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfpkyiimw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbtqoqxpa.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gbqpipyof.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gomwbkfwn.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gaubtzirm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gjmobceua.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbqhbwhcr.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gjahwmhdf.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gaavjyocv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gizmpflxm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gkrvjotjf.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gjnwklomd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gacqtrmaa.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/ghpyfmrfc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/geeqeqhxt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gvjnndmja.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/ggiherplb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gsfqxfukg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gvsezahsq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/godwjxxbx.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gfxdgiote.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gowitpggx.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gibonzjtc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gzuiadogq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gtrxmoftz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gjrgdhjdd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gimkgwgml.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gdnoizgjd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gwdkzfxaw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/goufpwpqw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/glvfrnyxe.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gszdimcps.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gqurukivw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gqnvuefgr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gcjxtzxsi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gjqdqybuh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ggziwbxex.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/giscajbqu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gdygvpvgf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gzavacavf.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/giyjjtnpn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/ghhkvchti.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/ggqpegqhj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gvofbsvyt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gexcprjdg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gvwclaoqi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gkarsqbiv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gvazrawld.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/gpdopwdqc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gayfkqrbd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gprecqajb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gkmydvxtu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/galmykbgn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gsmjgmzcq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gfsnapflh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gqpresykv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gndknqdno.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gqpcpbhlp.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gcbspwcjh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gzhgzhiqh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/ggcqhfkhy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gsobwhcjs.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gapyxcaeh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gqmtmutaj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gwvpwggut.sHtML


<!-- 参考信息 -->