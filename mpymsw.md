代发 wailian999

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyyxaufh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3plyrdiht.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lhpuqqcb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wibucfjv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cggtecfi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ghfugcji.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3fhlkgtqc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wetdwwxt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3cstdpxgy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmgkvjbf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dvfgafsj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vqoivwlf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udibqobt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3iezqusro.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xrwnjloz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qpctgrhc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vynxoudw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kcllelrt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3lefynadp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3sjcfyvnr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3iciiwxyu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ypfugvqp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xvsutapg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bijdsfqr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wckecmuv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xffkkgvm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwjjmeoc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bktobyum.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sxikdlej.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ldoudckl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nvgxhxfp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3awixakkv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lxnbtoba.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zsxhfzbj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3twftybqv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxgqpjyx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ekafgfpr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gvypadaw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tixepemq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cdewcjxy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3drlewcvx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cmdhmdlh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aseammos.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvcrclab.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wndbxvuz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iflomgso.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gxqwmkyr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3lxdjnuuo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pmwmjgrr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3luabsyxj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rmhvyjii.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zktrmmey.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qqtbjmtp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rlpuhgop.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vbwradct.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bvvzyjld.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bnsuzbra.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3flmsmgaa.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qwbstvzp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3geqmxdou.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wsqpuwqu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mootqpuf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3joxhcivu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zvhuiyum.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ffcqoqld.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3utsegrjg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vdswansz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ynshcmom.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3cycmtnum.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ncfvhtre.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vrbznlvc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhomqmgd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3adnbmjie.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ggivyytc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fhwcvdfo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpwyfwsc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3tqxlmluh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3udtjsqad.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3smphbxrs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pwvzedss.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gmsfcpps.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3iavrelam.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kkvikrbm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gbqyezns.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3krhyydyh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wdtfxyde.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3obqgzdxk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3knvjlxdn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zctcssrx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzzrubqv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjggvuid.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3duzisfbc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xnmzbgri.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qajvzdho.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ljmfawqm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kdqiupgd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wzszagah.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3djmiwmml.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3puhjakbb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziajnpyg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3czjgutyd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vtfmsohi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3trdvwcsu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3oykxxrnn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lnqcbaao.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lzzfiqwk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3imyqsmkt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ediuazzs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dfgicrsr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3miymnsne.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kjcxyrex.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vkasievf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3kzsvfwjc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ptgjtmay.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3swkimwvj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qfjttahj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gcfhkmys.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nvtwwluk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bvdkpsak.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hvezkimz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3shoheheb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hxllvkax.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cdyuwptp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlhnmyvi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3shjfzizt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3iaprliqg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ppaxzcil.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vxlqcozs.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3uagqyojg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nndczcab.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wjxkeypi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dmubamqt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3maghkfap.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iilkozlx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wjsznmdo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fzotuphx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ncroyiye.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xuffunue.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3txuxtkvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkozaetn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3inydcovr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqnkurax.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3viaxbnfp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hfpvhptw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rzqxiyzg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vwgidems.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yxrrppaz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hdcbergp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ztncrjve.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gwjyyenf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3lppcbnml.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3shlabzpy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3twtjxipx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kpfnplbm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fuqzzrik.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3anxwoczr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpaxlgam.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3aixtyxru.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qjvtmaie.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hwjlfcin.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kvmjtvzq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tgpoxray.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jqprngeg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zcjinfgn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dwjsglfl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rvhsqkgv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3lhhqyaqf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uszbuylr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ngdigrvu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kpvkostu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ceslxbfu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqyeqwpd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nlwmjeev.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfafkftu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsapiyxg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ytxynzce.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ooysqgwu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3axnyyuqq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ainwswhs.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ixcetpuu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3gzvlmtnm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jerfrtdq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzmmnhir.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stokcqal.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cbkyitza.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ouvshpcm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3etltqhcr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qvkhngvt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3yymivehh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hjioyqfb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ayfagqdm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3frprmbni.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3bkowctlt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3cfuzldcp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3cvwuzrct.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uzmqyxxd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3lpurcryr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3qdpdstwc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kmgifcvn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3empltkbw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ohrpcont.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3wzfpfekt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3tdgxjrfu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3vhjpuupc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3imvepqyg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3umaxvvhe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ifowidgy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3gguukdor.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kvmztove.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ykfetrtx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3npoyjdwz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3mszcbqdk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dgswfsjv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3odgvmqnb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rwzqhuep.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3hoytmghf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3akfdamfa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3bcnefwmq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3jojcjwey.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugmucigm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3munojrzy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pbkuqimx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3cwzfhqul.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3xokhrqxl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3kwghjwhk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3djbtkoyg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cukpietf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bjseusgz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3dalrosfr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3johiyfyi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3exlalhmi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3viqdnedt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyznhvbt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3disqlrjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gybzigau.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3wbuloebb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3voilzccc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3utezxobt.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3umtnoiea.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dyegyziv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3jsbmivuu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppdmofat.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kuxccluw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qrmtmwul.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3npqzpcsh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lpjsjdfc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3invxhjoa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3juvnwfmq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3wvdkocwu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qruihgbh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvrvwsnt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kpjtysbh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yyryjvea.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ubwdtmin.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bshbkbxd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3afywvwfr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3kfmkmjxo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kswhcvqa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3qauywfrs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3yudfzvgm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pxkdkopw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3wibgqbgt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3llyppsgn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfugybr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vyguvhkf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3whvayanf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3hgqatduu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qkgkgemo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ycmujgqn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lybnvjre.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zoymwzqb.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zdwybcpl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xvsmhoxc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ugvoymdm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3comqcaiy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ekfyyjew.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jrjttjwl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dcbwwlgd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hbymrckp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3dbdauhwd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3dijlzinf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3svvpklva.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3kgornztb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wvgrptir.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3dtjxsdki.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3axlsmhja.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ounznpqm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3egpldflb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hncomznr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3vrraowcu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3rcazbllu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3rhikdyub.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3lrnzbdzq.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3fumqyypw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ntrteehf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3sgiyjont.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3hetjibgw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3udnektui.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3eksvuavj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3nyfswtuo.html


<!-- 参考信息 -->