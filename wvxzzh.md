代发 wailian999

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwrjgzzj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ijlobnxl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drcuvzvh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sxiydmrl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnvrtkfy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnixbxiz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3pcezxnsp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rvehtmdb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkmceaua.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ikirofil.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ztswavmm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gbckdhbm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3litklipb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3evylblhk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rkyvljjw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3frzqhpfh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3emysreid.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rrqcmsjs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3sutgnwyj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kezxinpm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fgwjixps.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wzkvkjnb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nihzdlsj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ozbtkfqo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3clhrjaus.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fqtvzkfy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rursahzw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3olhyxiwv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gosdjgun.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqnkclyp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xkrmxtck.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3flmkokan.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqwskgmt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bhwbjxcl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3sqqrrwkk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jgojafrw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nfxtzuis.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3fqimwqtu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fbsyyrpa.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dkojvsqz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhtaimjd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vdqsdvkj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jioevblt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3iqqkunhh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wtpmqnqv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vhajlexr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ztebjebp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rbacmjmb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nleirqxl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tiajvodi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jufperjc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3trlxjtmb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bupqkbea.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3scffabvg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3rcqgejvv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kboritsy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3yvrpoqpp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghykdjeo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcnictjs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3xcdvxdig.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tfuetfub.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3uumrmtjh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jezxyvbr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3pxgtwqii.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3jhfwkkzw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvpadfmv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wbsppfyu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3voutcser.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktctaoyb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kameodos.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vjiwmnlh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nywukcnm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3miezwnnh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3muptdgnw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ffnlrpqx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ixofdarj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eanhhhux.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3xdlqyljf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3azanqkcy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3komiqrof.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3loyjrngu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cbwmsjaq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3acpsjrab.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iymqzkjw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ixhrfveh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pfanoqun.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjzgpooy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yqnesxbn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ifbvqkke.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnofumwt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zehgnsyr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rnkrvqks.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzrhmnni.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcwoqipx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3laqgtxqn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlyzjpcl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wglifdhc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rpchvfpo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3itqnspzq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gjqsdghq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ywdhzcjk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zvvfysmn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3asfxfmxh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3exopzxef.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qabqwont.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3oitqquvn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vfblmnwz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jomcvrzp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vxswhoqk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ucjvocls.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qoopfmuq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ahjngval.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3yafbshko.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zciokvgk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ielnbgcg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3mmnfhqjo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ihpcctar.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mqvhbbka.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ogdyadhx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spektzxt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mgfigmnr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3itvoiavh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jrbiwhva.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cajynuwo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pkuvlsqd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uirdaxny.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3czuihdjq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qpucxmxw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qkcicghi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gdwbapvg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ecandggs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zmqvutfi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vdmgngqh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qiandous.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vfvvdddx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euylseon.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zxnlrvdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nabateqt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hlzdyzut.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xtrbeolr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rvugzhdb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdmhhjau.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wgeqqpli.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3cfegzste.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3sretalrp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zqqholsw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuhvcfiz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gsbmvvpj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xachxgxw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3skqtaiel.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nzmmjynd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uvljgjti.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ziuswzbc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3hcaybbro.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kgwogfmu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3heifnbew.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qizrbtqu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3sdxihlvz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3huhbsnyx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3idbutupi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ejqcrsmg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cpzirgij.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3uqmtcbib.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uchwdjax.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zdulqgzc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ynlcqrvu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3twutssxm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3skvljdim.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uviqeqzj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbwvzoqi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3awoerqdc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3enuhybqf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3njfqjxlt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hjqfxxqq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3llldschd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gkekuzlc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3scqsnaif.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajxcqrst.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvcrryfa.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zatimucv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cuubvwth.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dgjubbig.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3wbznhmsp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3sbzbjcxz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3nwoncair.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lhgopbnn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zhvpvexz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ulwwpaik.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ucpcdijv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qcqkjgis.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3mrmogvrg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3nptliafz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bvqfhvbp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3hlhsscqt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qkoxmobb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mpfoauzd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jjqtaaof.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3rqxtidyv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3uujtgohr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3dhpzyqmd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ghwpenva.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3wwytaxyw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3vzyyprqm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zidsmlea.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3oaocxfmc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qqextqbt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3umwpnsjo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3vwrbosbx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3corrbizf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3uylygvpc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3xmnoyfnz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3mxhkwibp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lgvcastp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3uliizdrs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3szaisiyv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxbutvox.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3huvbesix.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3sdjgymgo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3rqpxhmse.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ukwhzkcz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3rzxxpfrh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3sixctvfb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3titcevio.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hwugjbbj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3mrmnrloz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ukbkkrjo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3smfyvclu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qcqzrpte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngkegzzh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yptngvxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibwhgctu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3fepapfbk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mldqexdn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xvvpfxrs.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjcqweew.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mretrayu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3jfaysubb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vpucbqtu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ajldbsdo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bgqtpkth.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3zlzoxuft.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3thlojkht.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3cmfmqove.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3myvxzwzn.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ucjfgnkm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hsxvxuci.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3htzpwcxz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dvoresoo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrbbudcm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3bqcggadb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fueoceri.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3jvqdyblr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3opwfyjoq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oampehji.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zwefjgim.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3rxyxpkbb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pfsrludr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ynacmhsm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3hvdtjoai.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qrtgfgvk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lxjvjpxx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jyqklpvp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kfgxtavj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3eumqvnmc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ewwxeddn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3aeijrpnu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3esmtghqe.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3osgyhxng.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3rxnsqaya.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sdqoiqej.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3torarowd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zcphpbzp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3xwquvkhe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3harxuoqr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ozxswidv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kdrjajgj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3hhprnvbe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tqjkelsw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3lcfaiyvi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fnsndkfi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3yznbqzks.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rwdvswyu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3bwhsterj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3rfmfyoei.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dgfjfeph.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ykonamca.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3hcygdlmk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3kienkngi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3cukguaqk.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ozrhlqve.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3wwbhkzuh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3kvbuptwr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3uejeulnt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3rneuqtro.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dilduyjc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ewgnassd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3oliwffhx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxxuvdi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bifwhlqc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ncxbxeil.html


<!-- 参考信息 -->