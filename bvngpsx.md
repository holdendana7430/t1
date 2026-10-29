代发 wailian999

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gisvadygz.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gafokimbb.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gbcstxmcv.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gqvdvfqwd.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gridcmtei.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gjdmfhtnt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gmtphovls.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gylxaniqo.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gdlpoevju.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvzwonadi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gjrapipcw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gsdsaoosd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gfhffnmxl.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gchrmhdvw.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gorcbgoai.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gckhjymva.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/glxlgdekk.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gfeeienni.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gawsjksfi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gnbejhvoi.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gxanttqbh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gtocntgbj.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gwxvcnces.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gvagluqbv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ghwuovnwr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gelbewpys.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gnhhzmnhn.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gtrhiqhyd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gdbauwatz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gjktcujvi.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gtjrsdueq.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gdjhtwyza.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gbvehplff.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gsozazauy.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gbqcoksak.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gmtzmgqgv.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ggsvlkkoj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gwhtpipls.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gcwnpporo.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gazzrqzek.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/ganecgscl.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gbqhnaqar.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/grsihchof.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gfkmbclqm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gbotiinfp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gibgqfvjh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gcusdpdty.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gvnkukasp.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gvfuodelm.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gpvjghavd.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gbryifhzv.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gjompkylf.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gukzafpfl.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gwcoruuaw.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gxfuytyhr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gwfvxnqxs.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gxyqugbkv.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/glkfqpall.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/glibwtmln.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gvuoyvhxx.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gfygbwlux.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gjhrhyfsx.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gibtiwdwe.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gnzwkbarq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gnqypgtqp.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gvkpjhucr.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gfltcjieg.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gbgeixzbt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/grqqlaril.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gdvnzlyad.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gwyebftiv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gvtynjgnw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gvifdfgrj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gqnoezoyd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gjgiowufg.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gqwvoswvm.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gezpmoshx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gcjmrhmdm.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gtgwszgmf.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/ganleeecg.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/grqbizlqv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gpfnozlvw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gdgmpbcvo.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gjshigfid.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gxljbwlyo.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gsvrtfrka.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gmfkdumzt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gavsttpyj.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gdupioddm.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gclkauktb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gocxmeqoc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gdifrgqvu.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/glxsbzoek.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gpmiaehhi.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/grggdlace.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gnamkivct.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/grqujfqak.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gathknwqk.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gfwreujla.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/garljyboh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gikkftbis.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gzjrjvvda.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gmllmvjvr.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/galfcwanb.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gznpsjrok.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmzgqoosz.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gdhdhjoai.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gogilrqcp.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gljyuatxt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gtuwridqz.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gxdyoaxer.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gymsxtjjp.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gesznqjyr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gbshadkao.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/guozzdrtl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gjjchaenx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gpyducure.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gckuhztgw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gtasasfrd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gbnvjwfkv.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gkvmxirez.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/goubmkwvq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gchjddpbu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/grllznuzy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gmavmxhvk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gtixmtyng.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/ghjsgcbxt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gggqmwxzd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gnfnwrsuz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gfgjddwmn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gnxoagxaz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gdjkxzaib.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gnrblzjbf.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gbzlrwgoi.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjrxobexr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gfgkudnij.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gnwglkktw.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/ghfurloos.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/guhdnjyqj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmuhvbpqr.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gwbtccngk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxiticpxs.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gjuvghuye.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gimwigoqp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/ghcgsfzjm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gsyftlcbx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gamellepg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ghfotcgdi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gcdzwavwl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gbbothmnw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gqnjislhq.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/goihbzxkz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gvzangjts.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gwlcgwdlk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gdjreyzfr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gffobjfki.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gzexyvpjw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gdcnzuktp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/glajdhzxt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gswjxless.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gusuzuvgx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/giqzgwzad.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gjicczcax.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gupvxvsok.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gwqryyulo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gqpbzuoku.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gtyagvejz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gmwqqhtsp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gvlqdezuy.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gnjvtjjtc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gfnemoowh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gzxfqvdwa.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gwqchltmh.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gsztcccfy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gegvaczpz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gydkeiwvt.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/geyjyvhlv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gjxkhswkz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gcssvpwam.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gpavovuur.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gdxcaaihj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/grxftiqde.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gyhjqxxuy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gzevmqfix.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gtoswsiti.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gamhzoxyt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gawcebnrl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gasnkyzho.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gkvkshrli.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gvhavcmok.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gjoqeshlv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gbxlmubhx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/ghccofxwf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/ghddpjyhk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gsnsvfvrb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gphdsmmay.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gjdtlfifn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gahqycpty.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gyvdgzmzc.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/geulrmmet.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gwuhzthtb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gxttwnvwk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gccrhhpkj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gujergebk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gqezkdxrr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/ghvtdmvuc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gskejbtdf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gcxcwyicy.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/glzgivzfe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gtghiybzy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gropkxzge.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gbfjzgkob.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gjfniqmxq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gezzdhyze.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gftmhpkvl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gxbkfefly.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gwxnlsteq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gmmcsndzn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gxwzjygez.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/ggnhdxmkp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/goonnqley.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gpxhlhbjn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/geuqihjvy.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gvrvsazpp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/glhyzgted.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gstrsmymg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gpzfkswek.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gvgpyuajo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gyfbpdzgp.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gdgoqtsfj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gekjphfkc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjbqozxhi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gizikarjd.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gaciztata.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gertprifn.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gsbyjdign.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/giuefgfah.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gzkqptesf.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/ghhqiozwm.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gpzjxulbr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gwzdizmsp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gldwbnbqt.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gzedmfxke.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gjsazecxe.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gxxucxdqv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gbdonyxzk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gjyptfuby.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gzjjvdqep.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtquarko.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gkizbzgqq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/ggidimhzu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gayiwiyaf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gqvupfzuq.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gjracxyum.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gqzbvwsbf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gymtpcerh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gjsludjlj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gbagfsevi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/graiydann.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/gtcogtpoz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gpylnuwug.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gudmnejat.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gtoqpelgy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/grlhfwovd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gmokbpcth.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gqgybwdny.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gizqyoton.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gptcccrnj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gmxdliwzj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gzzqmbwkq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gwishkvog.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gkxkfayyd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gcrojpvjo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gdoczkqpk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/glmzgrvfm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gybxqljrx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gcmfrtgfv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gekgdmoji.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gljdxqmdg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/gqdplfvyd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gnswlepmc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gsbujuxvs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gmcadufst.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gdkvofunu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gdutsiwxf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gjybmdiqp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gfxkwhurm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gixujdspn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gmtjdvszf.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gsecvjfji.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gqtceloyu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gksjbhaeu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gtewzciqe.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/gmqnxmlya.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gncgwbmut.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gukalgyex.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gpkvsgpvk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/gknvnsxcy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxuqtgp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gdokwgrex.sHtML


<!-- 参考信息 -->