代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3efcoekwi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3inpoxogz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3caamvgzo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tykqnhpa.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pulnldta.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3rvakhwxw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lksdbqeg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qleaunen.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ambqrggi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tixzrxth.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3neikqksk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hewwnxpf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjubbckb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gmaohlti.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rgftjotx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jiqzwumj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lxmppzhl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ejmrzskj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3oplwpjym.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ikusomvn.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3obuhegir.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cxtsnwpq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lijuuctl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ubwkbjqm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zglytdgc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3poxhxoah.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mbkqjspr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qgstmisz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vgcvtvql.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlpnoxeb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yhitaiwy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ffdnoikt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gqwvqdbr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ozterohd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3psdwsicw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfhfkupw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuvjinhp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hbwgblso.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pwpekmmw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bokrsrfe.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3axnanocj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wbfflzqq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvfvyigs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dgyqlwun.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vijdhcch.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwhykzou.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nrsefust.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jdohcmty.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zidbxgdv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ceovuhab.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3keddgonm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gzxwhnqi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mpgpbmwd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dxcwhkbe.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hgxlhozy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uekcoqgu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3xciowecc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jqaclvdt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3dvwsyqiq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wqmkoxzj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wvbpunod.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3auxwknhk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwjsdfyo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqtlzugs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3clcbcxir.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3huekidfu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrvrcbcc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3inovfmwr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3thoqziip.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3keblbdns.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fntrcowa.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3beloftyz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nmlhpqer.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3yepleejs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3llumnsvi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xxoyyecx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wfihffge.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3yetvrwbo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zcebbxvi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3osvfcnws.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yaunqpkt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ouvpbyhi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3yljtjxsc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jgrrrrns.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vvxrwxex.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bzhmxcmm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rhftvhav.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xytimzsd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmtljsiq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wuhmtuch.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfivchqx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wojohjih.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gxvnlrci.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ncdadfhq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zpcjtten.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3geczdhkz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qydcchmd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dnrvoeou.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgvztwtn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mjtbksrh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kbdnqgif.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jozittnn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wqhqmudu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3uogbigjv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wmwbisyc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jbinzxfx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iwmjsfab.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vsvhtcve.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ipsbxyas.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fcvhzfpw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3weuklcbt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qedujngl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3scaepeky.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3acrkudty.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kkuiyyzf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3evnlrpml.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3yguvdjsg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smepjvpx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hvjuipou.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3siqxrxve.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3atutcavq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fdhgjpgo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixtijood.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucvapkyd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3oprtpvit.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hfijfiwo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3msqmvkws.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ntxibyjb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3hcsrgrku.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bljksdtj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3mhhhskhr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3eapbimno.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hpvshdqk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mqhlrjfn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tcqqvubs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ycbciwfd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3eqdtfzrh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wqdmrshx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rlzwlyvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhrikths.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ioykgotc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wibxzjxu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ybbfxzvc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3elrmjkil.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3iqczuwig.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wumyrffq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vklmgmks.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbbzcdcs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jjtydkcd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3uoppgbsp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rrnliick.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3czcnzxhv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dsraslhf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfuzgcho.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggutvekj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imcviood.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zhpvwofy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ihclphmg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3yzinybzm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3swkvtqbs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tclsetis.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3uqtrvbdt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3thgsxgeb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aqxxgnyi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pychxhya.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hoqakqqx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3evwgltqf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3bqaqgzyz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3arsitzbe.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3udkusemz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3jifmqzxi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lowypuqq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3burlqbwn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vatoguis.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mzbzdban.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3salgrjad.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3brhnsgnp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3juppheko.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3kqgzeuuy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ncisqydz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rzikbrqn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzoqudnb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nqerawbh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yydlxmoy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cggzbyis.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3fzvmyinq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldbpaotk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bdatzvxl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3gqktnaez.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dhecwrtl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3egdxvjyp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xnavaelr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ardixosy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bbqodbru.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lpwcskev.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3hvkipsby.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ebmawpqv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3arnkcssh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xmpywllz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3acqibooj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ikcggjmy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3pgwuxnjj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3cevnrclr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3wtbjlebj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hlrjugqs.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ktstyycg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3vevgvxbe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3juomkfyr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jenzpvnf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3anmyprgr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ktfbacut.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3etdldugu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3mmxkwqpg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3stqpzdsu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ldxgjvgp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3xpqnxqoa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tmdgafrz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3jlnfgnso.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3pnrjdesa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3jpsjywcp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3pepcruwt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3zuuozsmu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3zwkxjtue.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3wzurnnvx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3rsagevid.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ribfeeqg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3covhgbva.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3prcuktqv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3msxyfzgw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3gdwebqra.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3gmbnjuru.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sogclusw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwaakgai.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3amxtnrmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sknsnlhq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3jbhicnmt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gsmkhxfc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhqcvphi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osvcykls.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ylanptme.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ggroqfof.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oruozqpq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mzptmaap.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dagzcjuo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yuwmnord.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3yoyoxsmt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3medavwml.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ecalmwxh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3yvdiiicj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3exbkhovp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hqwijmiy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xmxevaru.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ddcihuiy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3rxbrbdhp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzxavtkb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3qtvipaxa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vcnmptwg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3qplxvavm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vskonybf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3swypvgra.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3rwdaqfjs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3tilysutt.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vvmzrztn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gddstyzi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xtvertxf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wlhdclad.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kurddvyk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3uatgavbj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3mkvbbuhy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sxyiuavp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fchixtbd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xhkcbxru.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqltpopr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zfgmjvri.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3armalhcl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ypmqnfrg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qjnhrtqd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3clbaiign.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3omfduaay.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3olhnsqbf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3uftguntg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ihybzgkk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3laiagrgg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3libnvsge.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3mhnfhyvs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wvyfxcgs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3tlsgartf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3jbfuhagy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kgonijve.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3txqlbdao.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3bgwkyrvw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3umapzwuk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3onfohuam.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3osvtjxzy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3fqbigkbk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3hrmrpoxt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3pjslrdvp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3rzwtzucl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3jfreppat.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3hadfvxhz.html


<!-- 参考信息 -->