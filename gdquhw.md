代发 wailian999

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3uvwoqbuf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kfqrdgwk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yewjybbi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vmfywsob.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uitmjzew.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bocstvzn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wfexzbfa.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ziigdmrf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3igwjuxgz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xruigrjb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frtmbbpt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vdotmjon.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tnvdfsze.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xybdqnhg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vufrgthp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nbrmhvha.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3srheytxx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3enpktsjp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wsaokevm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ikoiylbh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tramnynj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nxikppcg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ecgbpejs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ntiblktc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rmaclatj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tcnjoukb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3aszkqlta.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eqbninoe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rymdjxha.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wizatvnd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3epgnsmbb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nnofgbka.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qcydzksr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlpoywdp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jnwqhyaa.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jzoefgpl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ekugdoqc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3itiuzorj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rvjbxkhx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ullpehis.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmlksgpo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3wfwqfmiz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qwfovarm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3rwvtezgj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wxnblqgu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3liwkzbma.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlvtovei.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uikmrtzq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehocrjku.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pxebisyd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tnrupicv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sdwuncbw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tnhejbzk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3yvxbystk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3yzmfapui.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vkpshott.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3omogkbqq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ghdwbzja.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vrglsyqf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jjujvvjz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3sgrjuzkl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kdlxomie.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3hygktwfj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xriduyby.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvlvnxev.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ruytwzkh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyogivpa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hejcnhcw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3xqbazfxw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ruqpejqk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3aqukpqhn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3brukzyzj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3lhhdmaqr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3thgoadof.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hftxywlz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3bigcbgto.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kfvvbhbs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3yqealrlx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhmqpgpt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ffhpqmwd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ofknkdtj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jlvauoju.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ykhrwlzs.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3igphqkqz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dxwrlmne.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3yiylkiby.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ouuqtkuc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ryuewawr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fikoqrxm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hocnifpa.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ppblzcbc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wnzlfqnv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hrmtmdmg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvbnmuol.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hklfuihu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nedguvqf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3nrqykkwp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3anvkieds.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jrhamfub.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gqxdoacu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvvyktcv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yjvjtjgy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3crrsxdww.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tiruvhmq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qatdbvlp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmayopew.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uowdcdpi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hlyudyfv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3znjrhewi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rrfpjzni.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ovvtxkjh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hmphcubk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aoypbufv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3cmxzezff.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ljybxduh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3hwxsnmzs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3meozaggd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ehvtlxct.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zxlkgbmx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ktqswkgc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xkixrjat.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqhhrbos.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3zdmwfpqp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3tfosujvi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3pkljcywp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3egqtdwnt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fxtgunib.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qgoxayof.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mrmpotad.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jluteret.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3czmnvhnf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3danevrun.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3adenzzox.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pynvkjtl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3kwwrmcsq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3llvvooyp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ruouxore.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ajvavfpb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rpjateko.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nnjrklut.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hswdkzzk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xqvmaojm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3boeqjybz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilmdrnhf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3nhylhkqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icezfget.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3idtkcwrb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3wgfpgffe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyfspjxf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkbeddxy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvckfkeh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qznnwygk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3beclxupn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3erwtcxmk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3efreeetz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3mlfgydlq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3cidjrqcw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kkescnrz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vrfsmkyn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvqdwvhi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ydsytlug.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3abtjhmzz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zdpaxfbr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3futeqbnq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hadkykzu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bxrtkdhw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aqihaceu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3avvcwoba.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bkbigfam.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xoszebrm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3sbedmwqs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3smnmdyix.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ylxjmrar.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pkhvuiil.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ujyoopch.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrokcdms.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ztinjfwp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nuzneadm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pzokxopj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3gfyfqqdd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zunuuyzx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3zuhoidkg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qttxjwoq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3lebbaypm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yexvvveq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxjcyeqf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3idrgjeox.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rpgkkrut.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3wkszqxhm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3cakxegao.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nciazeqw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3afisxyif.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3yiuztfrf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3arprirtp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ozrxxpuf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nmoqbvzd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3lmzonlat.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3dfqkraoc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3srowdibz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hveijyio.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ibypbgih.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hljhkxmx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hjfabhcw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wquymxuw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nrypcftt.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qnaxvoit.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3upvyhorp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3jvucntkl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xcmhffhi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3jofhhcop.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ebzokxxr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3mhjepugr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3pqjrhlhu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3diurbmvg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ikiutbdg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3iiyqjell.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3osqgcwga.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ihkeihmm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3smkgwrje.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3cejyyonr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3foejjkjy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3fplikzqu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bsmtoicq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmqkgfdi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aariuzol.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3naohnfgw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3dnzallpm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3pbicfaze.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3cqescroi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3bxqvfrpp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bzlmikjc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3pteqwljk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3fismokvu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ovqvlojk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3pbrlcavb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qbxgtcwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zchbqkxu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qhixrrpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grvckpab.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gjotxydl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vtzkaicr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mmoximnb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvooiodn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3iomcukqm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3lxokjrex.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dsdocszi.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3njltiwpf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zffxebru.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ivaheppt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dnjvvxwd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3hnofwdmh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3jdtsmzdy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3xssdjhzt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3iwlmpesm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tajiorgv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3stlvwpav.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nbhsheyw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3gseboslz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qaretubj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3lgyzkwib.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vyxwlfum.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qjnrjdki.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3zfynofac.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3skoqfjyh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3drhylhny.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3lzsrmnea.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3mbfzuiad.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lekxyzlu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jvniezwg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ozxdvdhi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xyqiotsu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dqxkufgy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3rtemjytj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jgmmrmil.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pvybuhiz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3olxujjtc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrgmmkaj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jhrahpks.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ykpvxwnd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3giqjtqet.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3brjfqkey.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3byvinvnb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3skpldvyf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3tcrzqllq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3lasbzgwn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3kgenbtsr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3euucxfnc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hgheffoe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3cugubffp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dxouijty.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3bsbzprzu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ckhgvxdc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wihsnnxu.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3autajqgo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3eaqxakri.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3onqsozop.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3yjfuvwtm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3koxqphkv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3pxlhwblj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3meaahrep.html


<!-- 参考信息 -->