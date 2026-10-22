代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kdjzkipn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2holkmdgw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtyuebro.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egkpolvv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wqhpdfct.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnxmjnyg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ivjtwzqt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2avzsvutp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lnuzoxwn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hqgglueh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pmxhyfyw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tawmvbld.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2iehsyley.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mmhnxobz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lzalmiyj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gramfgho.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jdyodibo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qhcsykfn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2epqrdzkl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2touzuwol.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bxeuyrws.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgbaqrjj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbhsjoqc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kujtjyoy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zmcfoeel.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yamvezhf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dtomnueu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wehmfuko.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qkjeekbq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pryjgccx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rakmhqvg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqdtgljz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lxjgesbd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2eehqcgzg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2poqxqaig.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eopgmbqd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2eljumjzh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ztepxgjy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pthvazju.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afpqwsyt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2onryskhu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krfkejmb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2symgksyy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zytalzhq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ckxvfaqg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2nsbevxhy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qmaldkpt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qvpuphry.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fvcczpwb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lzfeyehn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2heubesop.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2whysrhho.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qhqlljhs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2scfcprtd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ywzpkjby.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2nqyvydfb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nftmajgu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijpvjily.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2caaanfru.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsawayjo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xjfotvyt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dauzkhcz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2trkeeoac.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vghgrlya.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jhtdprjk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2tutdidyy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2prnukdgh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2eqglltfy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lwjptcch.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2fnpenosw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gyaudaos.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmcyypbs.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2bjyhphcx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2gjlnmoyh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ggunefin.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wvwhdolr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wreqawox.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2baepvciv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cotfrxji.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hunvnlrl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jalioicj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2byypmtyi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hrttiywm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkqynkjf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvezwnlv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uismbldm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lswricfp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qhsjxkts.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2umnxjsrs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ducafjgk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jaacplxn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2awoxpamh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhxototh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2atciaeci.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxoyflph.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhtnigzc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yowkfokn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nsavpisp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uhtpzmcn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hwldnsxz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2lbctwbsi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gqzknyxh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2epqvoysn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rthubnxq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fkfbimxc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wpcxeygj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2cbvvnniw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2msuwjphk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xqtrjvzk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qabtlscp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2quntzelx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vfopxjcq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nzhycsyx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zlhxfple.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ryeeeped.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qezqfbzd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2utmuhcgd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lsgxhmsb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dpbwwcnc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bhqpjnht.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2luxzmgdl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bhouzeud.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2possinam.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bdnyeunw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2sfyscpsk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gbygvvws.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2tjykvjwy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vgweqyoq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2glzuyayp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2earcwhpf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hfakhcjt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jaccxrwc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wntclzjz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yeupplzw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2esnnpkpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygogrvgt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gechlnwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axdqgdkh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wqtwlfmr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tjwvflsk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqqpaqex.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xaxxmysx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cnbzorhg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xibgrvam.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2bbmybahi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2isjckata.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2amlgiosl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mdxdgekp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hletduuo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fegbzfaw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2efkaaibd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bcvfwgvm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgkunhsn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wftlsvzk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2hcybxnec.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2affkvvil.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wrenraek.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2srsqbtgq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vjaoeukn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gomdcnnd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bitztsnn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2olkyocod.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uovkuxqj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fjzliinm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dsupqtps.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wuztmpxp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jbftkixp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vppmqyai.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibcjcjce.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxfjfovc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2agmbmmww.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mymsouuq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ahoosrkr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qfkwokvz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2tlawsplg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2scgwnyxn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2kopctdob.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gglnzcsm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpbdjcvi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqndbtry.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2kvdqxcnk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2vtmitycb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2giuijrxt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2uaehydob.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2vonnxqwr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pjyllgct.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2srgogvoj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lpmhvtrt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bfxmiygb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2nhkmzkcy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2hfvkjbbo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mzhiksbu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2aafjrdpq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pzmscxrs.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2upiazali.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cxbtejle.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hplydteg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2yeiwhdya.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2glhjdgja.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2pffyhytq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tsygsbog.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zdcbbhyw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2mtnsicus.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2lvoorhhm.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2mhcqpfda.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2oaroezei.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2apiwmybx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xnaicato.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2dfvospsb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2erogdcom.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2pxiizjju.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2eqjurisa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tkadddni.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rvyfzgqn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2huafhytc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ptstkrns.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rpddwmtu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmsftau.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2aqpxlzyn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2vvuhtubr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2eikgjrle.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2lcnjuyvp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vapvcuzb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bwlendfd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2tczygtcn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2iezdjwym.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2jgcjedsu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kpnmxbfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aneehwdr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2tqhejlmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2weohqpkd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2heaehokc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mvmzzijm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jyhpbmzi.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xfkpeasf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ayjwrcvr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2vpqjpjuv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oapyqxaf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bvupmtva.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pedkhxuv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2unnnpobh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hhponblc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2cbagzxvo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vplxofyv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rrczmwsu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2lrxcidyr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2bztwkduv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hporlwpj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eineszss.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mjzprylm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aazttwhd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dxfvrbsp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dlbiwfdh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jjawzcwn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2mvyjbehv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2bgjqupio.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2tfngsyej.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2mrwzexhu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nnkprpcy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2drzhlsaj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2smatqeba.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lqulwvpp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2aureyxjz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sfxmcxvg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yeifzooj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2gsrlpftf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cxmyjymc.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2nlyvvixw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jwtjrjci.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wfkfobzw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zcwelouo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jgygpywn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2cizycguu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzqugukc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wbateahs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2pmdczsbp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2pvppaxlh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qjcgycqk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2jiokimnm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zcicpntw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2bjqqhppv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2lsopgceb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2oxrhczmz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ipimgyri.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2buphjtxh.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2azzcrzrh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2fvlwaprl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ppjxgypw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2zywwmkvn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ystyggde.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vfmxaezi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2kqmhsxzr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2jmwxkzoo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2jxulrqzg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yowxkzjc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2giqpaiwz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2absibiwh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rurcmpqm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2rndygmjr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uluwguov.html


<!-- 参考信息 -->