代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mkofxdmj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ntdxhhqn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ixcguyoy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wudjsdfl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qdekaipa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rnaoufqk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lpbcgimb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gjukjspn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pgvisruc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3pxvilfzs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wzritzwk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jsnqmdsw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3brwfjluo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fesuqgkw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3znhjgfvs.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vpbbhylw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogxmgiim.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dhluwegr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3clupkztp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3djkpnhfl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hplrcsvk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mprwnrqd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dfjruqpv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nwjlhezx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kmjoosqr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygyzllaw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiyalelt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dbwdhoxe.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyaccroa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3aeorqswx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3csxygaiy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qzcyyecw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3elkxxulg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cupfghhk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jnfdhgcq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcweepuy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mdeklplj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilyyxlgk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lzlkmkoc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tigcclyt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3imefckjj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wndoctrt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wqmkzuxz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pcqgtsih.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vakmavbp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mzionmrp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vitwcyns.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3brlpprkf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mqrcdagd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nujvupvw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mjdwrkdx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ntwytoyk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpxvbhuv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxddpiko.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vuqdnmfk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxabrzbm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hclvlrsc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qwfmspuk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3txmisiuk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lxtluqkh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ryvachuv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cevewxtz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wpwnrihl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjkocwox.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3yxevesut.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wqpgoiih.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ziydrvbh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3juzkvpfl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3yhrcutwm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3iwztvcjk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gwtlesht.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lukfzdny.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bwrvqera.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gofoflnl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3sfiedzds.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jrtizkww.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nogkpfzv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3smefznor.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hbxxvcgu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfgklcax.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ghdihoej.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3niqjiuqo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ilappdqn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hnuxcwjb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ulzpfrvu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ooqpqgay.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xhlikapi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lvmsfdln.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3akczvang.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbxzwbqe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqmtyigs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gdjpgfux.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3obabqfed.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cpaboosl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hxauhseg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hqfqqqlw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cgwiefuf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kiebmtqy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pwrznvlu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nalaytox.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lkbbonjp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zjgeqwac.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3loqsfkid.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wpfufdsf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ywejzplw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rtzknjdx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3wjvwbgun.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3kujdskqb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3guvesutr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3scwxwbbu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tdoeiguo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hatsnijk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3nvoarvgl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3icfboxja.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3krvdimbw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jujtugya.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nisfaqwm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mqezdret.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vsxjwuxf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vlqlkske.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dyhsfjah.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zwbxhfwv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ippyyisk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3obkngxlc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ssmzanaw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tonfpsqq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tymuynqd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3miavjfdp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3evxmwoou.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ynwdiseh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3osfptaov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfgdxddf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ipxmnscd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xytlsllc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kwirxzry.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xuvtsyrw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3oxzaudlf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3azhodsok.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3arqhyeqy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbqrbmgk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3dpgniuxv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rmgzvmgu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxldcbpb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bzzezila.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3uznrgcca.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jncixwhu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3znfjftbs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3idqxmyeq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nyyuyjep.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3faupnfrr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jrposdsy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eekeajsu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yakgxted.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3yjltkjim.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aodcktlz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wdtwinzn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tconbtru.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ooawaabp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3boehcgvb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3grqtbpsa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dmkczvti.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ryzsydyk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fovgyphh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kydggxzj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kejnplbe.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfctnbzj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3weldwghs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jzeembte.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xfuzvtfi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekdxhxyp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3haqrmwxk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3jcytwxsa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3nizydirr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pgqnganr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnadibtx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvyfdsml.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ohjhbmet.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3cxcpkzbh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndzbldqc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3zwlpvhde.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3axzjafef.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vfynktto.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qwfutcfc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dtdrlqwi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3twmfacdp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3zkppfcfr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3eeownvgy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vovfaziq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3cpnnjlty.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ghhfnayp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uifbkhnm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uwckqfir.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cvvfusqs.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xghxvguj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3vnjpsrvt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3itgrnzay.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3smrhaoul.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kekthmot.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3cdoeguea.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3cprpolxu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gedwroyo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3kbursuiv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dftkzgze.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kimuvias.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3byhbkdfw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jcucfyfx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3znfialmm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wjlkowfu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mvwpfwna.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3xlognhhp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ovehrtgv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kzzsfrxe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3raysjmvt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3jjtbilxq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3uuytqlun.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ezfivqon.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3etnkmlng.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3bupykjft.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mbltmthb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3iwnuiswj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3nysxglhh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3dcnmhrsq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3bjupbmgm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vnvbbeto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezokukja.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ibdmunjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkheumae.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3elkfafnl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vwjoztac.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hqagmqeb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tqamjpak.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gohnodpo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3soxjdxob.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmjrhzzj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3tvolnzyv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qfdibqqx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3giplrkrz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcedoplr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3jqkuhvhn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3dbkmckvm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3xqbcmwft.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3blfofksq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3llbmfefy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3garjdlep.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3glmrgwkj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3mpxrrxma.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3eblsampj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zwnybkud.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3rdzcrbwg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ahdmqoxb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gvvlqzhe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3nrkoeorw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lqstsbxi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3dojmkxoc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kqsxxsfh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3trejhrkb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ijyjjsbq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3muzoewwo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yteleoyo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3enqzonnz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3wqkagqsq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3vaydiiey.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xlmogssr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3znjmozqk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3dkkywznz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ljzfpuuu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3doynlygw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fedfuykt.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3dnspjsek.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hxoepmdr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ikwhpsrf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ogrdhbcr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ziorvyex.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tssyfkog.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3llwxiisz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3apveyioi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ffrgzrco.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nncddona.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3bonmzhbz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3jhbcmczt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bhvemovx.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3yebpeldu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3ssapecxc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3jskmdnme.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3xcifdevb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3bgzfteyk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3vtuwthqv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3cotehtsh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3bcjkzmuw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3cutariia.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ezvsqxcf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3duvgrdyd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hlvfjmix.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qjeeaqlh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gtllldnk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3boouztww.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3zsqdbpgl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3dzcijlvz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3wgixwntc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypibynwt.html


<!-- 参考信息 -->