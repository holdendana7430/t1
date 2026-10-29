代发 wailian999

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gtxzikgap.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gzldclhax.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gntsygoiw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gzixngvvb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gnciuvraj.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/ggwncnizn.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gboczyagr.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gagwdmdov.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/ggcgmpkfi.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gejyvaudz.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gzosrpizu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gkhhqnqlk.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gvsmxgcen.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gcbcsfiuu.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gbrtjcevc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gipnepbfv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gctazsyrp.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/geiuqmcug.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gauhfunqx.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gehaykoie.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/ggjfzugrp.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gjidynxqt.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gohdadlwi.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gtmzodlnp.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/guttcxbry.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxbdbxmmj.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gsgtihapw.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/guiwneidp.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gxuhngwvh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gauzprrsb.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/goyvfhwad.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gcupiosrc.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gzxqqsdad.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gadoozhxx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gerdvwbxa.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpykomjko.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/glpliuwwm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gyouwmqdy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gllphawpb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/glibabprr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gktiznqpz.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gpjpfdlgm.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gofttdkom.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/ggrasnxas.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gunjpcjbr.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gquzfxknt.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gjuryhvfj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gzgnvenff.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gqxyzqtby.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gmefqkrjo.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gqycsnmhy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gewzcxfqr.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gkdfcatcm.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gqvbqdcig.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gewwwhvvv.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gmeovpfrx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gfutxqrhv.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gcahghumq.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gigxdfohy.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gdnqckofc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/glzdytcau.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gkqtxmcrm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gvcjxvfdd.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/glaenfxnc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbnujvrvw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gxtkcpzfo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/grnmzgjtl.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gkccjxfjr.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gbcpdzgof.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gzbiroieg.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gpaujhrll.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gdflkkgqx.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/glamgxvds.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gkmfsxjao.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gaimunyid.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/geaitbkea.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/ggnojlcov.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gmrhdmrbx.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gvrqeqmtz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gylawpgkh.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gypsbpyro.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwlhdfvzc.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gvilplhbg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/glqumuedy.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gzknobpkv.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gcdoyicnp.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gdudhpgks.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gvnukbwkq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gutinbpoi.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gebvarncv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaoudmbbk.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gbepucvje.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gwnfmbpbh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gsosfjwnt.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gcadtnxnr.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/ghnorkvka.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gvikfebff.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gcerymmpn.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjtuencve.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gwykmeayf.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtrztidwi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/glyeiupwt.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gkdnlxvuf.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gzqspivac.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gvxrqhqgj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gyspuzyzy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/ggefoizdl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gdmkuoxsa.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gaoaneokd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gopwcjuxs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gohlronzv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gqfjfvien.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/guqvovzbv.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gmtqxogir.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gidbxnnnb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gbxmjfkgx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gufvcvvwl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/guegiohbk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gwkbrmymd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gdlxntgxq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gzyhrabyy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gwaxgddzu.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gioompdve.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gvcptxyfq.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/galnwxygm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdjpzmaqm.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gwmmioran.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/grcrlywko.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gwrqdhbra.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gcgybeqgn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gdhjjtdfb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqmuetnul.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ggqykoump.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmucdjfpq.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/ggjzuhqbb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/goqjdorim.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gpffeskvd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/giobcssrs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/ghzzngyau.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/ggxpdbwzi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/giqidpgfa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gchxbipql.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gtrhdkkoh.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gppbfuwzu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gxnefrvia.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gxwnfyelb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gcbutxjkq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghgavjbwq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghxygzcwa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gpwmqnmje.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gwmbyzohi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gsacutgha.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gvtovhjar.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gttxkpexp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzgdrqzwb.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gmvgiihqb.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gvaliimdl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gjlzgtgab.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gveglbasc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gknuwypol.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gnmwlevvg.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gdoerrrqj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gkdawvogg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gyjwxqhhz.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gbdbguqlq.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gzkappjwg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gusgbawqo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gpymoqpgk.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gssdtpugd.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gceljzmnl.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/grpdwlsdu.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gylppoaxn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gweqingqs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gqevqbhuh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gnukowkcj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gugugxvaa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gchniainn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/guzsydusz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggdgxszdk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gcycoufbm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gzfhawkzs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gojvkozev.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/ghxrpekqz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gyavqfwpv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/ggchlclel.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/ggsqgdzpn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/ginyvfibb.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gonasxgbe.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/guoidnckd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/govmkgswj.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtsjscdak.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gdteieseq.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gthywcanc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gmygfcdfq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gpaxujbvj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gcrrqicul.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnxfalfgy.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/garxbdybp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/grflsyrxa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gkgkrxohf.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/glqrjdknu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/glxypzaai.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gotlgucsc.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gjgszhyda.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gygbuwmmb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/grlmwmzcx.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/guqepxngd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gpdxriesd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gglcqgajb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gpddvxtwp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gkofwlmfb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gjsjdyuna.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gsshbqrds.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gswbtgdou.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/goslmgjxi.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gzijitnfv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gupuowggy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gvzeyyqab.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gpwsttiha.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gjmufyidx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gfutswkgx.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gpzudfdaf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/ggmfyrzib.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcgbrysct.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghdnelqxo.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gcxwguglo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gemlzhfmu.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gexqikpoi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/ghlomqpwt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/grzxlonah.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gaqvqjczg.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkjkiqsdc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gffelnkyt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gfdwpdpve.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gsgjieyga.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gqhwokvvk.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gpbifvjsj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gpfiipmah.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/geyrjiqzp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gowoahkfp.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gpdjcvwot.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gwgwatemd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gdbyzygpx.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gsfmxkcth.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gxbcuvzjh.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gbbhhtkhk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkkjbuwz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gpzvnhxsu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gqiiewtiz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gwkwsypfi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gobmmzkcs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gaistwexr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gmmqffezs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gexvhdngt.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gcsxolysh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gpgsmszxn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gqtmkzhhc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gjglniagn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gvtflqxem.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/ghepmettg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gkjeiggvc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gtovhitcg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gkoimrkgb.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gdcfaiwmk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/giwfifpjg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggjkyfmkj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gmlokrjrv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gwgqbghrq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/genxvfynw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gcjqrnjbx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gqlxelutr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gpecznnyb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gxrxzsqqs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gdcemcvpm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gyfrbwefs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gxhkmsolq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gdviphlfi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gbtjwqamn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gsnxyxozd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gquqwvamy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gzfeflhkd.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gmzixndpu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gmdzjidru.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gsuudctud.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gwdakogwj.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gvaeukiti.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gttmfwdbr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gksreddxy.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gvnojmedz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gbhwsyscl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gursxojxu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gcuknlzct.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gkpzphkvu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gdmaxfopo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gaqpdcorc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/goqgnwcha.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gfplabyiv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gbvmstrnq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/giorefcrm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjlychoau.sHtML


<!-- 参考信息 -->