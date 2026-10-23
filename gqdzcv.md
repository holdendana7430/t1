代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wxxijcxc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cluvwyfu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aoulkiyn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwjckdop.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qmaotuka.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3mzuhmtto.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ldytclvw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsxdolol.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rorkkkcp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xgyutdqx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ekdhlukm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vvylipwc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3dgmcielp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdljadrr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jkebupis.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ogqpbldz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fizticjm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ceyfqngv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sckyzasz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qjvvafdt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lmroxgyu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3slgyvqvl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3daldczah.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3lpqzafbi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tsgnwnum.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3khvacokb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ikeegpll.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nyvtggny.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqtvtfoo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gxucjkdp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yyjibvjp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztatoolm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dfeykmkg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mtyvmjtp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qwuivyfj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tfljfdxl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lwkhutrn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3srnxqinq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayqfrrbr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnwsjxij.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cvkjesll.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ajgqqkrx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxnmwfrq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gampnxsk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qyhhwocm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xwzofkdy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nuscqzdf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iypseupq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjrtrbfu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqtfzouv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3agfdnxel.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xxxrvigc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3fqduejfq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dlbyzuoi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3muucqygg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fveflbvw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yadvdzvk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uolibiph.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bhwvbgtf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3rfdjlfpo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yhptjats.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nwrtxgkn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vytbsfpf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qqlcdhwx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgrmfvjo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3acgnmhpa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3odusqlne.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3yvtxkger.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hblpzakt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cxcbetom.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqnatxzk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3iaqwxvtv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3fcvmkfqu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksdcjuid.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lsengwgw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mszpdswn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cczqdqtf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3svtdmeqr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tdilbfyj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmncrhzo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vzyyzpnq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3cxjncpeu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uymsbfkz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mkfrjkez.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kajurlus.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xchcosuo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jebwvczc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3byfehglg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3japvummh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3lxrhvcig.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3baplqxfz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wrqwhatl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tszhiyzv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3peybrnra.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fiqncgmv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ufqqgoju.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cxbsgway.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kvcwnubs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hqxqfumm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vrktrqmd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjfaaopx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qwyyzypp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wzhqquiy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hhcwcddn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qoolsipu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vbmgbpea.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nnfasrlm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vprkycxo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cvbadbgi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lrtmnfvn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zcsyvhwr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3esnhcfer.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zjfdcanw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3tvytqaki.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yarpwton.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3erajzxsd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wltkzlgp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xcvhjmxg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3khdfbhor.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fhswnkof.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nanxpcwb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kizuovav.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3eshpysys.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fekedqge.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3pomxaybz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ykqcmrzg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrofqsvh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtqhqbhe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3rmrkoyku.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vobcpppr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3icvrtkal.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3cxgklhxl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3opcxhblo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rjgrviey.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3begssgqp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cljxrgwa.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3mdxhemuh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3aobimcpk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lnfevugn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hlgclyna.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ajnqvczd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ortuelns.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3evjiumcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgxpyfyo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dbvxhodz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwddadlt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kytvvwzw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lqbrvaub.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdkfodxa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuzfpajs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ugroduul.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gmmqkrby.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3pxijtvoh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vnzmfjza.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3sglvaodd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wmvswuxo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hokgkqjj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3otqvobjx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nvxuymth.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzaupexb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qenxwjza.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3fuvaints.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3brrtspue.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mcbvopwu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pkwvdycd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3extoyywm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3anuwngwb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uuagnumo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3emleqfhu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jlxuqhbk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hcnbpnjw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3iqrgtbpp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wycczuhl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ochhowkp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tenkcpcb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvemuuen.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrzhormp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3djqfcauo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mqvucjcl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3icblzdla.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mepidmwz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3axkxhtrk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3iarsbclz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wbbkwdmt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3cvpqnxxj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlnludjd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlzjicxg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibrfcbjc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dyokdder.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3czyyasvq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bvivcnno.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3yfosqmji.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wurhggsv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qawnbxbo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xwtwpbff.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3swaqpemi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mzrvipgh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3chchtuqf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tculiupk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nznkzfes.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3cnkkzlkg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3dknhezpj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xjkrhfev.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sfhsnwqm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3atzkpexa.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qrkfjihj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ziretbni.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vnkzenzv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ofwquwha.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3azwhzxqt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3vrjfelmu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3bicxcqqq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3hhogxhgc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3fywpwmop.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3pfenlexe.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3owrmfpsb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3tviuhdht.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jkqrzcem.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ogqzsaak.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3tyxvqftf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ebscbynj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3jzlldmhc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3blwumkbf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecmwzdsz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3knmfokhg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3etbswjgo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3dpqseski.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3uskbwdxj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3hcchstor.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qcpimsrc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xrvssgag.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hkiryugc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lavadvkz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3pmankmtb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vfaplxkm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mwlhkngw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtidypgn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fyhddouw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mktflwbi.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3cpwsnbdd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3iaxabaio.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fssneltn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rdulhctr.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzbxcnpa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3xjdxuqxb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3owooftvk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ylizmanq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rpaqmtnq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3lodkjcmn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndozkycm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3whvqcuin.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3xefxqqov.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3usfdocwq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mgrvyltg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mmomcayv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fohwiycl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3scqwqhhz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3rfneczjo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3insjjlgh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ezoypkto.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3nrcsnati.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3iftareym.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3qrnjqaem.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3rjfxqewx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kkhteewj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3pfmeyley.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3palkdjqd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3gxtxxayd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3acvqkovk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tpkwvpjv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ympxgjuc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3nlzfhuxq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ulqnayah.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3dmxizytc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ebdeeljr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3zrgfkeek.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3caaozjbp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ypikopoi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tohtnuhb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3itamzajn.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3jqsmkifp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3oobklrwe.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3iyejsnnr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3iswvujlh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3lfdxontv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wuteecde.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3dpodroev.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3exeazyqc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3baykbhwp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pphobsnd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3jbnqzcfw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3wojjteng.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cqjrygxz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3kmqdcnpy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3jekzuhzo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3plbecyqj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3zemwrnev.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3mctovcly.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ghfsilvk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ptimbkcq.html


<!-- 参考信息 -->