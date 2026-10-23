代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rvnvmbqm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zwmzmjmo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3djtwcwkb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgepokof.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pcyawtxi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3vvbsmmhe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bmtrfuzn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aifpkqyy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3byqrmxtw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpcaibgi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kvkbtdsf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zsdtbkrm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fvulkyff.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vasbiqnw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3erfxgafl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3weytktcw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nvjkghle.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wrhqxofl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fnmiffxo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xrxelktm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tohmjqms.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qpmymixd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pmyytdfi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vsnhxzvp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yhohlwml.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzimwqcw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgniddqr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecdquzzs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3omkneeir.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bbaiiilj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fujaacvo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pnpdnowf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mmubdhsd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncdvvjwy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjimxdzw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhsfemkw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gmvchlnb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3scpwdjxu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cvybtrjf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3agmfetfa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3pqvyazmo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3qncbhxxy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vderenkx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjlxskgg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ssxhxxwr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpylcusn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lsjdkccm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3gdrdyytv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3unruussg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kinsxiwn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zpewkbti.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jtjjdrxl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gwamjiae.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xwpyykvr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ojyeybar.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3raxuvxwu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3nxigrtod.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zhgjzzav.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wvkqounm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xhbhxlug.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgardtex.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqapvsxa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwmnetqn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vbtmsvdw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pzdcgwgw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3esravzrk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwpqwvyi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nseprxzh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3yrjvwhlk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttokqkiz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gqessiht.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdggheav.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtusaxgb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kqgpxbuu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hbekbulb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3crndieeg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3puilgrxq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3giwnsbzw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lgowhnym.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xvkhatqa.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nnklvrle.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nlftasnp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xderbnkm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jalgfvlo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dlbvizwi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3sljqcnqy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3sxiioehe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkhcddyr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozxsnhza.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtrggcwc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdchftq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3emyxuwxz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3kcngfmye.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rusdzfmo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hxpmgryw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ucbkluzs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfsjzcha.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yadfqmbv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3abbjfxfn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qbpfkgyp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nyyandyi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ngyaulzh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zjahmyht.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hhwhnxzw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xxmuejpf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fektzdve.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ncuvzmle.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rhrwnfoc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hlgbtkzw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3nzegjglo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3idyerrms.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3copwzebw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ddqhnnsi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3uapfodip.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3kaezuoqa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3appcsfum.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qkfndocr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agjryiiv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3nmauqkeu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3mbrfqeue.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3jkhcwhjp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3leekjffc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jtrvkcgj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sharqetz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3wjktoteq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3heuhyfeb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bmxxgumi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jgfkkesv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jlnigdbv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nwrwnaom.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qyzlaopz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mikvqaht.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3pfaqkiyu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xvmnppez.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xszglkpt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hcfurmgo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zwgaifhb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rgxkfdie.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jndaxdde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxtkyyuc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fnamctiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fltvigfq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3zvgtgujn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3uqoczrsy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xokuvclf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3odwavqaw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gurfogbq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsyiwecq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3scmyjxvn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ahzqnqwo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwzheypw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vkkxbacu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vxzmcidi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fwhhmdxg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jasctnug.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxwevpcp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sruyljcd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3dewdvccs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wlpfccvt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3olpaeacc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jnteqvra.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fdhdazij.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3facropdg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jfnnyoci.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ohmqbuzv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3biebpvrs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zidtndfv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3wtedrjrs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jafmaywr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bslfxsfm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ipvdhimm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mnlaxilh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjvlibtd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3upyalotr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fycxogqr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pllmzfny.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3komowoic.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3wifdebov.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3dzxjdaqq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3xfgzyrrz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3oftairgu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3udlcshzg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nnysjqrs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3jirlxxhn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cqaivkev.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3scvpkxfq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3yermcrff.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3rohghzun.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ubqgwtxu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wwdwdzjj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rkwvhqdu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dpaetlji.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3pwmgaxgp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3maeslntf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3snphxcmr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3byzimqne.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ldtzutbj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rpukuwkd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vksffssq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xbomryol.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ffcwscun.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zqpxguob.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3rizybucp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ikqtyqma.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jsvrgfnq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3vcnahniu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3kaerewrg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3mdcynzra.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ldyzttwf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3kbnkdhgk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3wjrlyfeb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3zxsxumso.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qcjukgrn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3znwrzhfw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3pjzpsief.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3qiigaxrl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3rdrlxjhg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3mhumijng.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ymqnrnex.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3bkhfcxoz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qsmwdwyv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3umkqfrai.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lxihannk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rodfngbi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ommswdoi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3siytidgt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bnknlayu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lueupime.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3yxogemcl.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3fpokquwf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ykczcyhp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pkblcvzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lngxlhmf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3opsmybiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3siigipei.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jlgcrtwd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qolfahxd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yscdhuol.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3udzijzgt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3betrwlmw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3bxcgelzg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3soqhuogl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ikyfiriq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3esoldwcg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sdkjaqyi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jygvnouu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lpazxghs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3eczfrqoy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xbnztfbm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3eugebljp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vswrfzsv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pfijcvoy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vptepbvh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3mpohmuru.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxpxcbsb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3lkqlwalf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lutypbod.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pwdffutn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3nohomtqx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3jbevswmw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3bnjzpmwv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3pnksujaj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3obbcrfgq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vacjorpf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kcapqpnf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3sbddockt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3psukxtay.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3evfuxhqn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3qycmqlwk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mysbjltg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cciwyjfj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pzhghxmq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckscowhm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ejzdthnn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nsldrmwp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rzuvxtcd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3rzfpsavc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cfiqxdks.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ywlnzcau.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3veazevoo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3goyybchf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dbwvgpoe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ejmpgaba.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kdtldhhc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fvrcspbx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dvkshkul.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3aejrtynt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ypnwsrvf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mvfcties.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3vzebwfth.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3lxmqyeri.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3sfkkpsou.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3znbrvbtn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3owsmzogt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3gbdgjyab.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3zxiypbji.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3polqdhzb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3tszmmgal.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3kgiylsah.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3wldzbram.html


<!-- 参考信息 -->