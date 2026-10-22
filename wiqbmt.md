代发 wailian999

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yixrnnea.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pzmoabya.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2iuczgznx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2deyicmin.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kfdibjpa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ighjyxtb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rsyflxsp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lfaolass.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eptfxrkz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bosgzgkp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mfvddtvz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ptbcblst.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uvzfmhlf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vtxlmswi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zuhyopoy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xdoibmyx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vmiaopmn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2msxlxwcb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wkfwiued.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zsezbpik.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ziqozxud.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2obwtitdv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vfozuhsd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tipbvwvm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nwlcitsu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2exxlkdaq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rdqxjjvq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ksbskbgq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2unlkmczq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mhiczghe.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2stuxtnvp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yijjhxss.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lsbxzwfr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2spnoypye.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zlietnsk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bvhrrijh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vzuicczu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2goqfsoik.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vdygsfko.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hotqxsnz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fxwhrnui.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kbqkyndd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yzcwpgjm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sdbjncyu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dfwivobh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zjzwhfdi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fpypalid.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vfwlmdfb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hzzttlwp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rbwedpjb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2sqtrpnls.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xlonhgsw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2llytyxzp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qnfmtemo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dbsicmuy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2mfurussw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2nnazujcp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2doohxpdh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zjgmobtd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ranwxstm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2mpqhdloi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hftuafev.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbxmwqgk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvayvspy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ugknhzps.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xggxzgox.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qruffdgj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jcriqqbo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qbycgtuy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hxoiahpr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2umcvqzsq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2waomgswd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yqgcgcoe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wczeunhb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2orurhrpf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvvjmyia.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2faebqpxy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2cdqnwwrl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2teykbcrc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ogwsjswk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lfgddojn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xggmkcqu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kgfbcppc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2msgzqmek.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tcdkmgob.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ffcjkebs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tmwtzalv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhljrjjc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vetqbytm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2crexvmos.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ydspdclj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ylssawct.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2bwcyidgu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2orhdkqyi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pvugtdwe.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2brjiqexf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zudubdia.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iykshxfh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vosissyp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2brpaimzo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zpztgbyt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2exhbmqdc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2laqlseav.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kqvpxfaq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qlpnvhna.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cvorkbyv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2phystyor.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2graxxcjm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hoasypmn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2unduolwo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mlegrjtj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pvbxxhsx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hnjaqsfe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bdzbrfwi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2pzemhpda.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lejzuhpq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yuwgqpfb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gssuoaha.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ryldlmye.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ighccfus.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2bmjxubok.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zcmpakkh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ohzjdxwh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2atbquitl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ogwetoxl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bxoaacuw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2cocezdzb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ycjhpatq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bhkcmkcj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2aapdozbm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2kynqrrtf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2efrzuequ.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2izrcwmkb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2goplgcju.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhpztoy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mvqmvzht.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vwydpdvh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2buqxjgdv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lhhdkwbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgqbfsnb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oqmaniwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwqjzkfa.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nymrmfxb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ocwatowc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2efblrlfs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xodiuglv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnxcchwh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vvrmyenb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2juusnbiu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2owvdbyto.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2kmgcvtvp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2cijlsyon.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hamcsovc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tmpfqkkm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2whqfmjse.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2awvdwskk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rgttloxp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hrojpsmf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2olzzkpmi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2spxqniqr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tnqybcoh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qhklneua.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hvemgaqg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nvtqgntu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dfteaboy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2whwmjwmq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xjourzmm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pczxzjai.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2stfgjbyb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fvfmzkni.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ntomdjwm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2aaqkboiy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hvmmsaxa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgcvdxbg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cofjwcoc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fyyjytbv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2blaslgmh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2arssnjeo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vkqnogak.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rgoqsekl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2glybdoyb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enknmloe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fnnfxkzv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjophcaj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2yolyedcx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ucoulawk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmazdtbw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ihhbiybs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vexqkvty.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cfeuqylh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nwvtmbjr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2slypiimg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2vagqwkvb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2grzokjxt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2fhhkzpds.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2varghukc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ewzwgxdk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2waxjztvy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pudfygnw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hogbojoe.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mwebmyex.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xjvjrtsg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qtksojvo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2uiixafjc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zbwhyoqs.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zpyicevp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ksimlylc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2notgazyg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2kxzgorjt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rbvewuag.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hvggdrpu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ejnevdya.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2xezfrnwy.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2avdenjzf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2yrynxyvm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lmscyemc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ybcqjebq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2oktinvct.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ufxicbfq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2irjtfqqr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gdppplkm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2mplemgae.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jmuhjzgz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2fofzdhvh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2xfileugz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kpaqoahl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mprnimpz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2quvymces.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2cenfnskq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2lfiytkzm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ocpycqzd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nvhndobt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hugvtula.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2insayfzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aolnsvsu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oujbxtgs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pmanmbyr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cokvxrvu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xkkfsxck.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udkbspaw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2txhnvpyq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2fcbkpzop.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ctceblej.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ccllhtuv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kzhinzwc.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxqxzuqc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hxpweiev.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2pyaqpsva.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cwroxieo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wgewpbib.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmlejziw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dlyrospk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pbblwlks.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qxyhlfsw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkoxtnup.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wcksxuqp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rkqpmfxe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2lhyumvqk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2puiljzhs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2qtohajte.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2srobvznp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2fbseujhf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2gdmjonax.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2frzlymho.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrbeyyic.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jsxmdxho.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mtflzddk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2uctqianj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vprdxfoi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2axldeuus.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wwoanqyv.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2royzlbdx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2uagzvllm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tuydmhem.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2iffyeztl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uxhgjjax.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zjthaceo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozigjjco.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hoeknyiq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2yigmjhvf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zvcrruib.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2acqcfplh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2lryhevxr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2uixtpeyv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fmouctqy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mbiwbivh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2cymidglv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2qbukskmq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mmywkwnv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mlelgidc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2reswbuys.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2esiglncp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2rkztjrxy.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2twdxrwzh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2gpbzwpcy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2zcdwxacn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2yxmoxxne.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2qgqygfwi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2njbqghrq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2qhpxzhaj.html


<!-- 参考信息 -->