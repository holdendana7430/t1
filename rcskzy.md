代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gssyhksh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dyiajcvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkngfcya.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mbrjrxoy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3kzzpdsle.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3yagxnoij.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojviqhpa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fopjnwky.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wbayejob.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nwmrhfbh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tfnrouwi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsqitfvp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3goacdjqs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bsdsmzzm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmcyweqe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3unwjsztl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ioyweztv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fuadroke.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ddlmromj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3nfgxcicn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mteopvle.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ghbzomaz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sqwbtpxr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lwmjfnux.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rzrkgpvi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ccxyxriw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3luwmyjfu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gffcoagd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nmwnpfgx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gjcnlehc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fvpkjlvd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pehmklkt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugpnbusx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzrdaxu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaxsaeyd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gvkjwyku.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3difjmgyn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qeplbuxp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tzlcmvgd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3bjsjotdo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kpwzupma.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3stwzoxan.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gvjfeqil.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pzkuexwx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uvrijdyk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3iefhqfpa.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cuffevxa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3uqlyjsiu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mheyityn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rwuneibf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ajwzurqu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwphlqtm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqswasyw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ricylqak.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gsnyuzpj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3srjnqvox.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3yohsabjs.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3leamaqwi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bwxodknx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ooaqgzgf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xyiqcwgz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mcoshxkk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ffkkbgyc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3tnldcsar.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3eticnqek.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xzmianoa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fqbzjkzk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xptibaxi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eauqxhxh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gixpktqd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydmsivyj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rutpimfz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3soxoeoxw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zilhusea.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3eflknyrc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jlkwhkcd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3festedjz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3unfiptid.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gxumznmj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kdondsfn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kqjtmfnd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3tydwtbxl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqsusqfj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imnnghbu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gboigpae.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3pybxehzy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rcgswsgk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fjlffxjd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cdpknaat.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fsckcjda.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zwxrugyx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qboxmykb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vexbrtkr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wtdqakht.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bgzehone.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3enjtszlh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pdnayfax.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svpxcvyp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gagjvvfg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sbzukncf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3uoujnoxg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3gcptjbvc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hvaxoprm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lfiuhpup.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fccsidfm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kszhkhrq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jvcesdrj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nzkdklmc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kculzidi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mcqmgfae.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pwrfnbuw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3glczxaxj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3frtezoel.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xtubskiv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rpepvfhx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3boeyhcxb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sfteewip.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ysquploc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gxybajyk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3taspicnp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3huqemkja.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ttdwfcae.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3peyajqad.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3oflksxuj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qtkoqbdl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3wvrvkxle.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gtsytgkd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3zfqaqgiu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3votpjwjg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qvqspojh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ztghjqwp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hogdmkaq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gbsuxphr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3istfrtfp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vwxmnmna.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mopmfiix.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jkbsweik.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iydygtxh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3eneujdgz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3nruqasdn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ypyrswxz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cgbeathr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ivqdsadf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qydeasfq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fhbvvmnn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zmertkvc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rvqnshgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rofqcpeo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3avzkwfco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdtgwjsc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3akhelcoj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3oqlfadxg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cypagyvl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qxptudzi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3edrxofpt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3joaraznq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lldrldzf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zmzjjimt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hytpcnvg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bdfrwphj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3jdfevqls.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xoacgoic.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rwoakaxz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlhkuskd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3isejzgvx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3tuqjpzlw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rfxaaxmf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mmhtuydf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cyuchtjl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zoacxcmi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dkueatge.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bijfxekv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bghivrqz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3guyfodjy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3luuqaark.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3htlhcyha.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tmxlqipt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpcxwwaa.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ifewjkwy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jnzkvizr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uumkhkhy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ivuotlty.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zbfuabxl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3klhbzles.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xqxweqrg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhzorjim.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3jxujydnu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3cpktdxwr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3dojznfzr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpejdhbl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3drmvzmsj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3duzgxpxa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3yncpuumn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tnexuxyw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rukhshje.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3llpordlj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3unfljixc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mkrefhow.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3irdhjhed.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ovhqrrfb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kgfpyolt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3klihyaja.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jfjrnkta.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3gufadypi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rgfjjkxu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3adkirwyx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yxnytcvh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cwccjezm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bayofype.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ondnwdea.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3oylzvmdb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ikeopoyo.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3apyxscfx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3sshpkejc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wkgaggsb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3qtkjfzpv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3rcnlcmdh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xwwccico.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ulxcwbcw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3cjyfoefp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3vcijdiyf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xbqatazv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ydinqfsd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3yskrqauy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tuezvknu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ijeeikzh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3qvujrtxm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3pjioymjz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wyrjopil.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3shrybukq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3aweoicgw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3yfsxrzvz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fsmpqxiq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3jhkzxdio.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lbjtezft.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wztrsgdw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3nrqgbdnu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jninmcpg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3rjuftyxn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yojuylzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwubbjgh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3lnsalaeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtwphvvw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jqpxkumo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnludnyy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fiqozsgh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbzxzelv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhgmfdxe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3aueqgyje.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvhizhqk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gmehhypg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yeepvuzf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3tiptxdbf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kxuhnnva.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kqkoqpll.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3wtcnrufv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ztwmbimg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3dyscginj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwphyoni.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3oqhsghej.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dzoroyhr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3htzslzuc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3houvdzyv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qgvvwhgw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iveivfux.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3hsdywiqu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3fmsmdjnp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3qmqdpxpt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3btkfzkjt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3wufuqawq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bdhoxjtl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yhsmjtvf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xawxtmlx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tuxuaick.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3rijoztrm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hcfanjql.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3etfygkfw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hqcrxcdz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pdrpfedz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3asdvjqdc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xvvcjbor.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kvfziwhh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dolygqjo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wtdwuasw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3akdqkxfd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3asoolllr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3enzhfebh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3nrchewah.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3bknysrdt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wkgebeox.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3fojegsmy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3iyawjxxw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3rdolrhsa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dhkhjicq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3bbbhfpaa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hixdknnt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ypvfxxgq.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3lveqcdch.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3xvfwcqit.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3jbqujprh.html


<!-- 参考信息 -->