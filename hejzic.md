代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kigexxas.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgpoqmoz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3yzyqyfpk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cocrwifl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjhaqzuj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bizmnthe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vtbknxzh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sjybelpq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3amwyulcc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vcicefvh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qfrrlzbk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3dbsaivju.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3yutbprca.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qeiljvhp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mrsxants.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3eeufaogq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uqsuodvn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysoxmbww.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbwmetz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohxpgjug.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yotudiia.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dbqfdodn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ipmjfqxg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nobnutnp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fuhcnkcx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rnzsrcdy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcgngwmq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwtxndxs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cpgfgrct.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cwqqiiql.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wndrtsyn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ccspgrvm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3umkrwipr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kfjxqjqi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3budevxfe.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruaskrtn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jkugrykz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3htlgrlqu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qnjdqyva.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gwtfeezd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dcqxdjro.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tgbajesr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jowwpnwt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3oaaquvrn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3utzgjtbb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jwcwldez.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nebcyqrq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uncbaplu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ggxxyawq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rpjmohug.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3thwnvxrf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3eubvnekj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3jthsioiq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vsyvjetx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3jkbvbnai.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyibbeeu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3kckxqlgo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ghfgcxid.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tehhvwrm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wsxrcepq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3egmjskcx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3grjckvue.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3dbtaptks.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmkrgfpw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zilzqhcx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ippxxywg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3nlrxvqwe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3brsdirbg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ypjafdja.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zknmigbd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wpeexbjm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dlwieygb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jfhvqmhj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3pcbatdih.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xhojgooh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vtmgidls.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3etgyplrx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vsriplla.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3sfijpkfv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ffalpoqg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtzvmap.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3alrrmvuv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eztnmlzy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rzdziwml.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vycjxoak.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tekinidc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zosuyalx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rzsxsnua.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zlmemvfs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dqonaqly.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yotkksyh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuojqljh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nvujzogh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3duiytfuo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gxqplpqj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hajhlucg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3zqdcceeg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3egvrkqxi.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mvthpsar.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qlodzvmv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qecnjeej.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3yeylkukb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cffhmkjr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pwmbhofi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jiqcqadn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zdkmdhls.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rgktuyrb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yvxtpovz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pvicedgi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsofowjx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ehkeuzcs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nqryfbda.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nldkwzln.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3raiqrdql.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zonaocnd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtxceeyo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xtftvjiq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3szpzldxt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3menxvcfp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fyglxaih.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wjgkknoy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xlbrvgbt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ozegarvu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3addpamol.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3rlrhtnbs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3upzddmqf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ouxtoepp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jxvpzndo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ibzbsvuj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hcbmmrgt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3irnjrwwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkcqkfbu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3etrsqwvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdymouxd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ivhsexbt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zpuoibvw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3iowiwpfj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iioomrue.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3czhifjlz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdiclkvz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vurbixac.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3gefoxhdz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3psaorwsu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vvgqcgxj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3qmnruimx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yswjbeto.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rykquxtm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dgezkgym.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mxzaoysr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ricgvbkx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3yspkbqsv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lawuamwc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rpxjoxal.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3rvazphyt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3huwxngwx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yakvtgji.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fabvdpvp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bjdhpbdc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rzywtaza.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3mrrpzuqe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oancqwcf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3wlnbtygj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ixlptdus.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvthkuwh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlnjnnej.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fuxcuxho.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nboosjtk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3iriqfdtr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3jpvbcrfw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjogldwi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3kbvqonex.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3bqiuwnmt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yxyfqhih.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykvguwbf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmttiloe.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qkxvtjbf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3aecoutff.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vouafkul.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xriujomv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3fsfnwknz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3yvfqsway.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pgfsttlw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3idlernnu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yozljrmu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3pqwdlgns.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3lzgdangz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3wpfooljl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3bmjratlq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3qmbikfrr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3flwgxlxr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ramrfmfj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qsvsdjuo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wvjjstfk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3llcdmzbo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kmdkyvfq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xjrrbhco.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ufyrgkbi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3xgcnfrpc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3zlgrxpbe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3boabqena.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3quigyhcj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3khhirnww.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3sqwcippf.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3iezvzrrr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3huuhrkle.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3pgyozzld.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3jhbmoqqt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3olgnanyi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vobkdhzk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3oecylkfh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ncoosqdj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3vajimzrx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3qbpbfzwj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ywrjrjhy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3twxqfkoe.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3owsgvugk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3jjyaglcq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3enmryflq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3esxfkjbj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rywfzxtk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3otklfuxo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3pllwymnz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3aliircdn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zldtijjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwrzsyng.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tqirecmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nitydxnp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ndtftwyh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnwuhrwo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3njcbtmne.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zplvfrpe.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogzsiahr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3wenahokv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3lwphnwgi.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nwosttyb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xkbtztbn.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3flimblph.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dblqmfil.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3bkkbwzev.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3yvwwshzq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxxtzih.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3frtsgafi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3aaftmosa.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gcakvrrz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sjpmjwbq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3bjebpyem.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adkkeoxx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3epvoqllj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3nwiakmzr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hrbaukup.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xwdoemiv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3vrpprerx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3hhhwqjhu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3uqejudeq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wlublfrs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3moyyajff.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sftykvas.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3mkvlvnce.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lisldhqp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fxliyvzm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wbcibdmd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3fiadvymf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vgbkdega.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3apwnlbxo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aumksluo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yziocfeb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3chssojgt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3onlvfgdx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3iqyeyenh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3jllqxqan.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3twwsupwu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3jddytexu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3lpyzxhem.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jpsnzjde.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3iebdhtvh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3utalyubh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ohveogsr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rovzcats.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3idzbiifk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3axkqiiie.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tkwempns.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3bfxjviop.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3hzlpgoqv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3jkjkbjgr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3salrpnzu.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3yquutgxj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3tdhfvzrb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3iuiyibgv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3qqtrqwbp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3hzfadwfj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3dngbkenb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3abihrgsj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3aaobvxfk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gassytps.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nvilvzar.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3opaeoclx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3aokhfuxr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3gkegccou.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vdwziopy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohtyndvv.html


<!-- 参考信息 -->