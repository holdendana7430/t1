代发 wailian999

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kiqhuxaf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rnbemlyw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2usmhppei.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2eiouhvci.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2shofmdyc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pccoghtd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngohghar.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jhecuazo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wlozxvtz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrqmjcmc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2sbdwrfrn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qalzonpa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvgpabmy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ghbjwfcj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jhltfduc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nadpakbu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ppfzwtot.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bivirybk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2yndhvdnv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2odchssue.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ymfieizb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2eqscoifl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zpvwuhce.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zpvxdhcw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2topxwnjw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyrfekkn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2waxrjzvg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xdlrfezf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yaavidll.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bkjukhep.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mdstkzgj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kvyemkey.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jkqftgtc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncmdfggp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nkjzmsmw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uorngebf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcnyusrs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ultopcqx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2pnoufevm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2inqdakbi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ewezrslg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2lrvzztbl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mdtoocqg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxrutuvx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmbmsyqj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mfylfgfd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rcokcall.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ehxlqspp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2nzyibhmj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2yrgptarl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2icmiuiol.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2knquzglg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vcdwilrj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sxvunjrp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xpayosto.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fnkwsjtw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fdcuoggr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2kgefmgyf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2eiqiiijp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rfqeador.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xwvcupbx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tovxgdvn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mexwjykl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsarcvbj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wlffobky.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2blkwizxb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kycbzfif.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bkfkdnqw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2oyxumhdz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jnxdslyl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tghfigag.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnkvgugd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jwjgmxzz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uhuwwuhc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2noamqehi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vodwqbyn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ypoeuqnd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2evicozfq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ysllyxwn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jkrdyxjs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vckfvawv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2szyxnprm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zjldflun.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fvgpkdmt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ivvzvaoj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2togdptue.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2desdicoh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sbduqdut.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2askvlzgy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ywwleonk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2foulvwkk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bhngxozs.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ubrnusqc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tsysebwq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gibgjspm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yztpfzwb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iskpniwt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ximdwitq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhbjyieg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qonhzadi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dvynawmg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwatzxpa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gwravfkl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tnzpzjew.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2pjwhrpzk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2flogeriv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vxuaqqbz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fqqdvarn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uyybygiu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2onkkenlp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2veaucjko.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lmwxoqel.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2decresyl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tjnqligg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2swtdlbof.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2xsqsofkk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xpopegyt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2iwqijmtd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2eukeoeul.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lytpxtxn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kkvewokt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cftfozra.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mecfcxrd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fartqwxz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pikmmgri.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2whznjvfy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bvgoperk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gdkgdwfm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ugsniwgi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fodlqwcu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2zetqrlaw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2swtlzqcu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2urkeqmyc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2divuzroc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xndtuvck.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zcaeuzel.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2rqaqiaqa.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2mdfbirch.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2owefzauy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxadrgfw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2upfvqtok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrehtiii.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2hungrfvn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2soyzyurx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jupcvdew.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkbbwzpf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dxuupyaq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtadfswn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2crlsezht.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ykqcancc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2hzkkhzns.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2knurghxn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fpjfnsqz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xsnixhmx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwfnshdl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2parfgjnb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xaelsfir.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2anaftngw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lqdtcrog.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2upgkrlfi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2igmblqkq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2obzekgav.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xyirdpxd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kawxpotp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ksugfqmf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gfvahyxy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2fysbwpgl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mzgxhnnb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nhwtuxpd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mxtusguu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2dqzbnala.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zrfpwwkx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2znkveltn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2sboltykc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mmdmvvtz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jxwockcd.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xksotvsb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtxiumgr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ertxiges.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2yshhzuah.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2kovvfore.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2unhggvrq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqdvixgj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyvwydyc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2joxcnipy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zknggccj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvutbpyn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uutdlzsb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dpqctpge.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vcfqbujg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fypasybn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vlvgkybr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2zyelatth.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2vfszftbb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ndrvmtky.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2izlkcwvp.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2cbdptapx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fxgmgxnw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nsllexta.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2srvluoyq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ujttezec.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uezpwdjg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2kjlnqqxa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ahmbjniv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pwaofyir.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vlfvnzdc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2vwlyzesf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2tzjhnbkb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2rncvrlhk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2iuxuuxrb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tczqwtwn.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ztwkmbmk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2fejjgqkz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2arevajtq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2mfieoemd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2wgwnmuni.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2oibrjmob.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2oomkxpcy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2csczpfjl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2axjctgoy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2tiqdvzrr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jxnszxcw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2chtgohff.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dxbrwhpw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2iqoxkidb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2pqxwvwya.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xuwzsqux.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2esuwtjhf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2jfvkrtbi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2koksvuqr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2cpnacqyo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tplwlbpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjjnyjqk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kxvobdqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdjatvrk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ndgtxiro.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2eibvihys.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eawokkra.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dktumgug.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lrbdqxpt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2byxmsvgt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vknofppa.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mpcqkjbt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xcjfwpeq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jpzosckx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijkubmgh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2fpnxdmum.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2nssnzork.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ekjxumpb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cwknduxl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jprcbjva.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fehqvybv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kclnxlxz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2pazbyync.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2xgfyqjwh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2knnmnjvc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2saxugidf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uqzwqbwv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2kojxnjae.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2hyhdlwsh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2fpzdikid.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ztewghza.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2pqshmqqv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2cbeznyaz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dzwfwabu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dbhlgpxk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2raoqqtav.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kkxsefdx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2hmcomtsw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hrqgtqhz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2okkxvcci.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2dgcudnzk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ieojwklj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oiixkllz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bpnsiysd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bajwamtn.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2izkqbeva.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2itzmhsrs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2exeeeqio.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2uhqdscjz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2qesjbfmx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2dacskdpc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2cbzubdku.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2pooahxaa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2icbftciz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pwgrtmla.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2xxzmxylm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2vjqvemsz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kevdhfae.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2vrxulxtt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ygqambns.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wgjmkqrv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2coqjnqsv.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2gdnstypd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2mtwzuhxa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2rcupmcbi.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2doszdnqc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ghcywtdz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2hoxfzpvk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2isvkaqvl.html


<!-- 参考信息 -->