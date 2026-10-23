代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nnbcxbhr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kxpbitqd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jeksdsim.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3shefxabd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3lmmbbsej.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mhbtccrz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gltkoqtx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oqckanan.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3amlfozij.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3akxldnct.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nliqpgvf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3evpypozu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gegmsmmw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ozbwysbl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nacchypv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nablftpt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qpkhjmvr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wswhrofy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mlzqqcqx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rjzgmfqd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnedmxgr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hwsurpst.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3evhgfaek.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3inppjdlt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3akqtbooi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dkrfxoyr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ibomhxop.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bckmxtil.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ikbvyhuk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnhgmmeh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzklziun.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3imyfjtme.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3banaychj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bwphkvvc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kegkkuct.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3iakzpphp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3viyqibmy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ygmmgkjd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gbccetvn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tnbvtmeb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rirhyeue.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3itnlosmr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3dzgpngcr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lstvyfwj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3usbqjehp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3bvfcbyat.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3sgojeqrn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fvcbpzrg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3doqsdnhu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3clrzzaqs.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3phebzniw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3erdipmzx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hyjvwjtw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fiyvoqmp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dmpzfinh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3eruwszab.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3smfevskr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzkmpmrq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjljeqrv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yaqqfebj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nndajpot.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hntkxqwm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpimxkur.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3eytsovpo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3skvmegso.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfsjhkds.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3yddnolfm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3bnotqdnh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifikzuqh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hgwqjrii.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3majbfusn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3etrwbwbh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rwoajsvc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3asmoniex.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oxotxbbq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bgtklhah.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kmyxbbut.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lmhzysaf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mfbihwjl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zprzdvhq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dwdxddzj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3axlenjer.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3csscglhg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qvksugbq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgfrrtos.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tumscpiy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bibywabr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3arazcwok.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tutwxrnt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3petrirhy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ciuospmn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3eykolnsg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tljzrcmy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3megfutuc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsmpyzho.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfnracrq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fjgigtap.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3avuaxvsb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3imzlcqlk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3lyzdhjlu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3efnbaqit.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xpxzdpza.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3crfdvhgk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zxfrkdrn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gfqjdpcx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3fnkmfelu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mkcaqktv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cypdvbeo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3armrmtou.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ghrermun.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3idpvyjfd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3bhotqqqg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3myricmzi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chzmmgtk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3wezfwcsn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3yyadyrrj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ygpwlpiq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qgcwxxty.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ttaikjca.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3raloeelw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wlgdgsux.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3iopdeynh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3toqmmufd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lnqsvomm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3kwjcgait.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bdaqwanv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cwhuzpaz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zacmqmts.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vwstgxdu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wstknnqm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jlkidnsa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3egfuhojl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3lkufvmnb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3sonclsdd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ifqxfqng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uskgptlx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tejllgjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjfivcwq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3sngwkqfm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qfalioea.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3svfljrpk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3madhwxql.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qlzwbade.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nzuozhbl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3abhxzsyf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3laitgbku.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3sjdrzeib.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3pfimcjhf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3jsdkijcl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ddellpcd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3izwiwzvt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3onbrjrlp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uiyehwon.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ybyixbwa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pmkdcjfd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mdgkewhz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3llgvevdi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rxhjntqv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3icckujjx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pqgzrown.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mvcubrcz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3knvwxydq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3cykljxxt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3sbeutzvh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3omrnyawd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3uhxwgzvh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pjatqoou.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ikuxbynt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwwyhlgz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lddmwctp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zltruolh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3phxshxtt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3qwbzhjvt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3svzbigsk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3fahzprdn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3bhyhulri.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3bcoktyzr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcvlkjdn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlncugvn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3yfovgjcr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3kbueiark.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3enmapfkz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ytdryvla.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3fgkrmnki.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pvmzoccm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kqzxslla.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pkvuqiuy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3smernztl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3sykvohvk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3zwgdcrqz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3tbvyomfg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3bweeodlj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3lsjsdkvr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3cnpedarr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rghhsntk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3aovgcauj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jplwrkwf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3brsjzunv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3wpgxahmd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3qkhiilwq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nhmspuzo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3cllhvcro.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3pizlbhwv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3hlppoxsb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3fwydqtwe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3goprvvdo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3drulaalz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3raolzlmw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3rchdczfk.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ajdyrxfk.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3zzfyikox.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3nokwtrnb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3dobtuvqt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3gfyyksiz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qwswkfxj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3cebfzhca.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3fghayduh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3dyjnptsn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3wamtncwf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3tiawwdkd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3sfpvirvd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3sogdavzv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mhktttga.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3sotlbnvm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3xmywpota.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3sjzwmlnc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3gsftwpxf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bshansbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcyatwwg.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3uazioynp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsqxpzhw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3inrkvycl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lqubivic.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3knsoeyyf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytakjkpa.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xictydkw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3yrjlebbm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3otbcvzdt.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hrvzdlbp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3debfgznf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bvyqudkk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fnabyfmu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qocgodfr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3lyittovd.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3wgzqplht.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3kynfjnmg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3regixwby.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wszrszuw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dcaidbfn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3zdjkydjv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3qmsxacar.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3umfxuaoq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ofwrdnyl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3lrkwxexc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3padwlmsg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3yywbmiox.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3lppcujhz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3momiuewp.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3eprsjwvj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kadubxcq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rrmauhpm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3gtfvktlk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3chhkarew.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3osmcanym.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3edevknet.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dxwqrzrs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hivyxges.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3rytuhoty.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jcdzwftl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iotynmrb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3icwdqgdw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3edsbntps.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3zzfssffu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcktmblx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pxhfqlmt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3otxepnna.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3makvzzyy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kqfbkjvw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3kaxrfeht.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3dfooebjw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3jzstklii.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ujdipfjx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3xartshwv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3sjynyqtf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tuwnqftg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3rzyeescl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3aspzyaiw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3tayfcduk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3namsqxmj.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3qpjznhpa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3bfohzuxe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3tituylxq.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3rzkwmkzd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3wtrsbxak.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3djigodpk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3uiaysdmg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dhoyylnm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3chubdrrz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3yxhlkdjm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3eldngczd.html


<!-- 参考信息 -->