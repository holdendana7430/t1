代发 wailian999

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxwpmqzs.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cukljhml.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3peblhanx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zjouqjho.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aslmhopr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3tecvektj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jawngwzb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvpyfusx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ixywztjm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aeworuap.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jkkzshxz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwcdxoyg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwvpehxy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3yozenhfp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3eblenimu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wshrebiz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yxbrlzrc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wvqfkiww.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nwuzbjdy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3blghluey.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rlxeieio.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kyujxgjj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jotbpxbd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3aernxvax.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rwxnonxa.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3piigvjqc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dagldrmr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkjkfuhz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tgeyuaea.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tryrijko.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gpfuuqoo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dfzyhoqo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vshebfnc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybabipfr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hbperwpo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ciacjjer.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojuxjmws.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fnbdjeml.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vvovshpa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vwomunco.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ndvwemuz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3asmukpxw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueltjuzd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jvbaxsjn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3umlkjagc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nqhmvbwx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3oqeootic.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfxihsaa.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3bpupfwnl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xdhmlohm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3okpmaarp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3onqozzov.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vuplbosz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qofrauaq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hkcjdvml.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3rxnloepb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ejiacupa.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lqwrijha.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bzngbssg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3prwjnouj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pueczqib.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vmoajmbw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvqkbose.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yagolkeq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vinittix.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3myuhgjsn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xjnrjdcc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3oejlwnat.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jmrqoykk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pobhjvaw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3xwypzkiq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mohqumyb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rycvbcbp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3rsncrfhe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fqrsfxqu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3nezssvma.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3afoucpio.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qovwgzyd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fzghznac.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3emkkdops.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ssueipxp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3vfzhrqxq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3psgywwsl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cjhlwsbh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ekxhpsuw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mjbkxhab.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zwtrvogt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gqunfhqo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpdlhtnp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgmdskvp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3plwgrzei.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gffzcsar.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3aimdgitg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wpbhdaqx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fhidvfpz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yecxrzfk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pedqhdxo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uveqgirv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prqsqrfu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khbnsotd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tjodeqel.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vnkyntgx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hbaksgjf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3pydrcsxi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3wegvfwzr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jfmtsbua.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ouvsbxqp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xpnxozfb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uahfdpbt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3axetazas.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ilxcrmdd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bcmaacqy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hpaogcsu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zmcmbqlu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3csobdvjn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3edpiuwcy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zczucpyh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3soviahmw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mecrnwxq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rgwhfnek.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3mnqftqak.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xhreshav.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sjcbtggq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3xbqpibrn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3izlmkhda.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hrwkcyxs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ehkrrcko.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3urftoizk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3hetpddmg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3luhjhtdi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3cukgdwwk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3agxkyqsl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qdskqqvz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3apdikghg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rersooxy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3rdaomhqb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3pntpwxep.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3trsoxvfk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xxiirfxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkuppivm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3bniwikwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlynbaow.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3tjalpykx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cocyxyby.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwwezllt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rpkuqpgh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixbuuxif.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxezbvwl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3oubyoclz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxlavnik.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrhexllh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3hwiaviwc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ivpixztg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eonnslih.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ogepefnb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rcorjjwc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3reryppyj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wrdejtdk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3rtmqorbg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxgrvkuv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3oyslkuwk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3oheherub.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hzpgjnjv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uvidkutr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ohhiwtpq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gjjgbruk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gvmvfisi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ltcauwmp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xshqjxrk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vmsajskd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3goslrlys.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lbwtrncv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfhvzuqj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tfdjhcxn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lingqdty.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3dcbzocce.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3gxlfvuzm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3nddixjrt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3xgjmrlji.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3tuigbvmo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3eklaklmj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mvsdtylt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pphlnhcm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qjhgpcrk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jkzhyufq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3iqwmqojh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acptldsb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3iviylxkv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3grhdouxu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xzxvvuke.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eaprvusj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3duywwnnb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3cmkgbcva.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ioxxhfgw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3pnfmxuiz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mrvpcneq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ifylldnz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lcadovqv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gxqkyzdf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rteceycc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ffuebery.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3uezmsqhc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3rcatdpsq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ztmisgrh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bcjmfabb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3vjpwksln.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3jnlxgryh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3nvdnptuf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ndiqsyfc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3vtrqioom.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pyfirzme.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3cdnueygc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3mvlffdam.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mbgvdjep.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3idgjgxsi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3doqrohxy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ptirgole.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ubxcmdle.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3xdpzbtjq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzfjyzor.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3groreceu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3rseejdnk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3twqjktnk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ipblawes.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3pcbncoaj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3srjtvsdr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bvnpchlz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ptzwfccn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3qehsrezy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3pycmnviq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xiondwnm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zymoijmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrlatajr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3bueuauff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unvswcwu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qncqvqxa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zzxftulm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ascjaroy.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nehfjjcl.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfagecfl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3jlsjxmms.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3obrxwihc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hcsnaklc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kwlseqbh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3iudolzde.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjpcfzup.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3dgtwkycw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3wriqiedk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jwvfamwn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jjxfoqgv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dbnxbhgj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ktwooflr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3omgmrari.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qvqoreur.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3vnctuskk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3qtznfafp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3qpmhgcpp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ayhtbwwr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gfmzwnys.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3isalkalm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bwkihbqx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3oxabdmmc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3oagfzzpf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3fgeweoft.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vgdempdv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3pvkgjzst.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3hnobbuwv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tdepnrlw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hocoqgcs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3urdywhap.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3duuokmlt.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bclnxejz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3zfojcssc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hqpppewt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdnmnvo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rzfnzqkq.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3eempunus.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ayqdneic.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zoborhud.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3vungvqsm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3hzulhlfh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3promwjsk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3hfmqqksa.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vyrwdbmw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3dsucfnkv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3uotasile.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ukvchvdn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3petakpyw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xqqqrcbt.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3umfoghcc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3wqpzxwdi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ewvverbe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3xkculyvz.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3rbudmwfi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3tnnuugqg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3wliqrcgw.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ublwmroj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3xdwzjwak.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3iekybsyz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3pynnalcj.html


<!-- 参考信息 -->