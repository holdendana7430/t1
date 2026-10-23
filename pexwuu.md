代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vrqjkdon.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3puyvcsry.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ugwxvjdt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3wtiuvfvo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sholvssk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rrfhbklf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yrmacvtw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yjhvjvqa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3chiygnla.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axpassjl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcfoppwv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiwfjayq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rornubpn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ntuaobos.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3szlgjzvf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wqpvdlwr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gqupbfrl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttcntlso.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lbfeggnn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvbalnyd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3czuswfee.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gztqpxnp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vueizauf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsomixza.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wxlefgxc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ixfwirjr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaiklekt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3paituwna.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fipfjxie.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyprgxsp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3xgwtcefd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zxphhuzn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3godctjxg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jnlrhjrb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wzkxfgjx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tmjlgdyd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eukhjgcv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fjjkrdgz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tqflarvf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3rabcigre.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zyddscyw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fngtvryg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bdehnrdt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3axhblekn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fyptdwhj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3tntiyeeo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mhkkrldw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbnmrqhw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ajjjimhl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zgaityym.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsvmwgzd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kccrcvxy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zvowidud.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kazuqpqv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3llgeqgzz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3neufzwqd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmiwbtnp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3aiiribpw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3josnmvrj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3nuveozde.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vxlgurzp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3sumjqicf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3koreopaj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dvxyzane.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wywjfvrj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yfaftuba.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3haayfszz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fmaevokw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zbnbibln.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3fuwuqtye.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qtfihium.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3okfxeqco.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ditqxfuc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3guufjaaz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3crdympfv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iyyfvcco.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3dyujrvvj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3txcmdyro.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3dqhpcdho.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tgddjkjs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3skphljdg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuquqvyq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3suqkuqet.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cfthmksb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jwzsnjwe.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnyzjaek.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gimoqnem.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tbduiews.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hodkiedi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xhwfhcop.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sfhrksrd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mokjeisi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nlvmxrhq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hurgfbzd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rbumzurk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yzrqljpy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nhlwsxry.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3khlgbxfp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xwcesbqo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3auqgbfbe.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ivndequn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fypwwauf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3znrxjggh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fhbzqytq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3yeguzaav.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dmnqcore.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3llgswpcf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3adofqpmv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jlljhvlz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sydlebzy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3cvankprh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3cimejggy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lxjwgurj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dzqmxgzm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3umkgquyb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3irvnanor.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pvhpzkrg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wstfdqdg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ilyydcxg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3efkalepx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jvavcgrs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3iulrfomd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vxzdqehk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aexemtjj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hfnwrehy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpztelxt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ifzqvsjd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3oubcsqvx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vigopraw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3plhouupx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3clmjsahb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrddlzec.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3svyqmlnc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xljkfblc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbkoxhzc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3lnmhdfpg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3zpyczkzf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3svsabzpp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfloyhts.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vjduzshn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bivvbwhy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fcdymxfr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3nkpinmvb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljjerhsz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ujdamzyx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3kkkcgefp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hjytlqmx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hyaszyvn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tiasnhal.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mjtkizon.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3kablsuez.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qcmxpbuu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kvldztkg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3wjmjpboa.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3realhpwb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3srseaadr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3caganiid.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uqnuwrxk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lnfibkiz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3funleekz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3lmafhybi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ouqxaeht.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3akldwhia.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ocducrrc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kziktwkl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbvrexae.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwxhomts.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3okdvtmlj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ilyqkeww.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ngjkxaao.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpzcbsmd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3wwtzbpxs.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3oudurwzt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vidwgzjh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zypbhzze.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vbclsvbw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3aokajppi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3trzbkwwk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gpxfwaed.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3deqledci.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3srwwbslp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3snzohnqs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mmhmkkqe.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wsfkoovc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ykcmonnh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3abxpmlgd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3zmfrnnpx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3hzzcfops.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hyhjwgfo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3onulqhkw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xianoyvy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3gvpwucaz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xukfasln.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3yfdcmqxw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3hkjzmqcr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3hfpnmkmf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ojzclunm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3fgqghhah.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3usmptdso.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fuvaoodo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3brssyixo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3rnwjpasr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3abmmvlxj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjqsdjng.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3sjbmugnq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3thrwnrzr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3mrsmlbtb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ittftbnd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3yjlzhpng.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3nsyywudo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fhcajxdf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ooyeehwt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3svpmdqhd.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3nkgqstbz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3wqcznapk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dhluzksj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpmysbuu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3gzxiasbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwtgvzla.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ihbrxmeg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hzprqxqz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jbcufhvy.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pbxqwpvt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udjuuxlk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ecxlmzny.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3tdqezwdo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kamtygbg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gidcficx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3npktwvnk.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eoohqopb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3srfznexq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3imauierf.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3txqjennl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lohccuzd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhutdssk.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fmvqvxdm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dhbjwwrg.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3jetkopkx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afrezpka.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zdtzphkq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3xlxhahym.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zdisjsrg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tiwwyyvq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3wvcxqjxf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3xbealfnu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3vodpzary.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3lqytzfmx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3cxpymomq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3awpmysef.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3trjarypw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3luwvtvbp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wmlovxhh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pvoepzlx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3rdkzfivx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qcatxdrv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3jjoptsfk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yoeinswo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mivcrpjc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3olzffcnb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vywsmewh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ohqcdcun.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yuavivfl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3lpvtwjku.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3brofzaka.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3gmwvsjxq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tplqozmi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3wbwvnulr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3majdwseo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3yyggebgc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gzwgnrpv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3pmymfwar.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3bbekyama.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vlqdxhby.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3fytplreg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvpnopk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3yivcqsvk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3argcgtfq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3mfmcdcpa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3wunvckjx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ilouunia.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3zftgwmvf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3kljywluz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3uerdvzuu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3klprponr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ewkcetcp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fqtvwuut.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dprksjfo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3gvqdidsq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3tlkchdkp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3tqzptlsm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3oilkrppp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngcwwrpy.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3fgznbflh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbruubea.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3rxtwcpws.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3afgjiamn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3gpkvazxq.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3abfuiroa.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mlshalze.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hmdyxhya.html


<!-- 参考信息 -->