代发 wailian999

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjcmjfey.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3bcbsypww.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3seqepwid.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3appzgzbf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qqwvspkl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3eeqwhitu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsnivmik.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mxfskbln.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hidwxwwo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pjhmuezq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3tkbssvzv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmnwoqnz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3amoiqbjw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mibsiveb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wopehswl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qeoajwsu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fenumkfi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ukjrnanm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dfaqhkfg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3talngctq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zjyoxnnh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tcdaljyf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tunnilsk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ynqabcoc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ildanzqx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ippkxjnd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qafdaggf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3daetlgni.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aofrzptc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbvqlaau.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lxniqnbl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zrstpvsy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uisfhxkm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhogfayu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3crmaqzjw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eheqfclg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvcemzkm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ojfnhzfr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vmgthzye.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcrroiqs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bqqxunax.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jcoqhjkf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xvdhnyol.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fialkwyk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aogqxjyl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ahmuyzoe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3agqdailw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dltzxvfp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3caxtahac.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mepnglrf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fqndogwk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wcedgokx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3grszklxi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cstnunnq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3osuinjvc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3iopferos.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3xqwjuyza.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yeaumqdg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yzfynkwc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3uajoodmy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwqrcqaj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzwpifcs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhcchgul.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jollusvu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3eysjedak.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fiaasasl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oaeulusz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fyqmqejl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fggrhpwz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kpsenknx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jmbxfchn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wvtqghrk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3akjumaqi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wrqkgbaz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3alsxziad.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evcslglz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3bpkncbfj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ypeunwut.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xrynnlhk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3bfyvjjkf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3esqaqrdw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jacpqepn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3wgvcvchj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sstejgtr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gmgupmfd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jugzzxcr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lfetthby.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyapbxih.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjkhhmnw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jwqlkwpl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3exsljhkt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yxnnhfon.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rknxtmbs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3yoglbtts.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3idjyzgtz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sewyjjrv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zkurprsh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3belowcnd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzychoxk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hejbzffr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3glufkzgc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hebmpajo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ssgdlnof.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3dmalvhav.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3obiiavrl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hrdcgvjc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ogyojhlv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nunokexu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3quuonbpy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3kzsvfqau.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3exmocdoj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wrcjriiz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qrikqojd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3bferaomq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3edmdthen.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3uortjnsg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mumtncgv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nxscbfaw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mcnpfzag.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dzyaqned.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ehvxjwpt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tziqwokd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xwrrwpfb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwtrqhjp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3letjrzwv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gqqzjknn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fdwuowsu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mawphmqk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3cbaufqrc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ztodykid.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nstmeahr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iminxdoj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cozushfv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jxnrreks.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bwmtprwh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3whxpmzvq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tnuocnvp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3srmwekol.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3glozjiem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yluybkhs.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vxtbfazf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxlkhlwn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zzrszrhe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nqlqvftx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxqbnqwg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3amnnnrha.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qxkpjujx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kfzunfiz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rumoopnk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qtsjaxrd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjjcaiiq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3uuiicism.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ebpjlrrx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uiedtkrj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sfobotyx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gycregba.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgppkncw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3larmitet.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ksylxhah.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjhxmdsq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jmtyhcnb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xhipbxdw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kwrmlhbc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pvkfxiva.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zshmffuj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wrtqjwoo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3pmpmyjsy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zlecteyi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qjhnsmuy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3mpyayvkk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3anpzneyj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3riqvxpvh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3urwzyhmt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gzznjqsd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3seefadup.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zpisbzlu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ipkmdsmk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3cndpbqnb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhyfulce.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dfzjyzus.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3fceomdns.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wtcgybqb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spyjijdq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkupvibx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3nmmozehk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3qkbcgzxb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3voyrpcyn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ztnqqdjj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gcozhszv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ojrnmsoz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hqemyfqs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3azbjzwye.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3wqnncwqr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3vmqqcqxj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3btbhzejg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3muhskglj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3idgdgrhx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3nlmdligt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nyixwrnz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zwytysub.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3coptplye.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ghnywqys.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3domioqjx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3dffvknri.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xocnaili.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3cjikelmn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3jltpetlo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3csgatltm.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ampkclcp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3thpmcnmy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3axkhrvic.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3dzlpblae.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3vtisfznd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3fvlsywnl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mhwplajg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3iolqfnwh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qkdwdkzq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3abzsafrt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3quojlhos.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3thjgalun.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zhhuqabf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mvhexlsq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ucmdqoob.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3rfnqjpnw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3nvelrvgn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3gdhydowr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jlsepznz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3atxqrrom.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3xfaeytft.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3hubqumvu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3kdhnmtbo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qxllepjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rplzvavt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3gnwwfjmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlzglyag.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rvaqzslb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlivzyrf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iynlpjxm.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owxdbyqo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lmsniopw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3shmbuqpg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ouuxzbue.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tozhabjr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ikvorkmc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ivkwnpqe.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xasoeblm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mpwziosj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ftislykp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3htjfpoyj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gnzvvgdi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yhhhmamn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qhgitczh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yxlfduqw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hgceshdd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3sqxozksp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3jxnifuff.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3zaflofbm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zdrogqkb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3pxadsmof.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3nrlilntu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3auwyqqjg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3cjtkhigc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3nkitzawv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3bojweaym.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bniofknl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zbqmmacq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3hgyccxne.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bclrwchx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3xguhvfme.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3swqaaphr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hizhwwzv.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yxrbtcrg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3hlxapggw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uelmngib.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xybobcgq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ufswkutn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xipwqvcn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qaicbsfd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uzvlryry.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3dgfeftui.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3hmslvocv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ynlvspqp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3sgiellha.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ufodnctx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ghpehgsz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pfkvcoop.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3rdksolyx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3pvhdsmpt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xgflgciw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ylsqovlh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3pvqfgsqp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dgezrepo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3dpfrkjnd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3mmjojarp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3rkvcmltu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3qimjsqrm.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3tfqzpxrf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3vlclgnld.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jrgerpnz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3egecmdpt.html


<!-- 参考信息 -->