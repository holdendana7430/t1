代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pylepppd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tbrsoxvj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xjnwkhsz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nkniibwj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dvfkfvqr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2sasrjzle.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnopgthg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rknqxnwj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vjaxdaiu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2azubfzet.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2urwdacat.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fvthanew.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjuydisy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hrrxpedr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fvlexged.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ycsrzofl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vwsehkrs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hqyocwrr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2amrtsyvf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2monwamih.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zztzdult.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tsfoobyj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2etvmkwtw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zjghlnvt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tezlnwzg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jetbfvap.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycpqbhqw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iopxtjca.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hzanwwde.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vxqbawda.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xtlvsfch.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2meoinmrp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xzknosyk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhcwabub.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hofthevq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tydqqvfn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2grxauwsu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2agzegvtl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xvlprzpi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2unmupkra.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rnsdypuc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zyoqwppx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lueuljhm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrtyffdh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wzpnixuh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2igvwmrpe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2itbvdytz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dhpmhbgy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2blzkxgaa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wekrsuhk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kbvmwlws.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lgdyxzyt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sceuxhto.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2izwpzeuu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sdlgtxxl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dtfluejg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jqrxmjtr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jrgzcnvf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pdwcjyxz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kazdephb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzuanoqe.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2edobuyim.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnxkwnfk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsasjobb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wcwwbzhy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jbnpvsmf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qeevwrda.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ohjmeopc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2rdvagpal.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekzuhztw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vqstowvl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtyahtfx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvoelcmr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2niqyafud.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nkxqwlll.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2odwyqxlh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vlzdvbbo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2paiwutfv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pcbsnouj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hpsrtioz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2neavgzrk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qvaztwgs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pcpnwrqv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zpkjgwho.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mqrucvtd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ckwsobfo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2utexncnw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mcvlrdsl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2owwnwcxd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2azhuvlzu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdbniemi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ebowliyc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ftielquz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rarzzrku.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zdyybrwp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2udwtjoqd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lpdnpvxu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jftuftzv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubjebxtn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pywnvqdb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yahjtmws.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dqeqnhjg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lhaxlykf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rmiiicpy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xogpndmd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qpusiklx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nmudlxxw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eepnghrw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wjpekrkk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2iwslzrmk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2jnbyxfsa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2sozcuzoz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ldvvfrmg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2lhekawci.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dibaxixv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2mwrsvlhb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gnznxdnr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2aoptyddw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zzifewua.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ntlpzexg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ynaqeipm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2suysiqcl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pkrusiqo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jzhsmjeb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2whrsocme.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yecjppuf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xrqfhupk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2liadpphw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dcbbydgc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zhrgfdfh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2aenbufbz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2xygqlmst.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bwdwuhld.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ftcrhjdo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lpzspcnk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qgwgodmq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2rzoexbux.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2adofavya.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2invrprnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjzslcsj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2bzounetl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iyhcjsft.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dtfsfrar.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2epucramb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2sukapsmq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kjspofbs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ghiwypkl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2egivzyjn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2booontyf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wyfdripm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnjhriaj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tvnaiddu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2utlgtkkw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zuskozqn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyizbxnn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujuympfz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bnzhjrec.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ybtxgwtv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pqqatlky.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjuttxqz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mmkdnefe.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2enmyoxri.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lpkrtvhg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wlwbsvuy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ylsveagt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ffumcqdo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2fjqfslvk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2pukeifel.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lklkvxxh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ervbolir.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lingpwil.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2btoditxt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ksieuqqy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vwihjfze.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjflhpny.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2afjhwkep.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gavkzzzx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2yrvseypu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ygeadith.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bpbfjxqr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qbtaxuji.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ylpjvxxb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ebgexjlx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tevtkmgm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ncfseduu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ocrdfzub.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mdiqtoic.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ntvgnlkx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jreaixsl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fcapkrml.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fcvmjigp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ffhnanms.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2aqzakbep.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lrtnajjy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wphqmcrz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lctdntvh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2nwfaxugc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tbslufhs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xibnmvyp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qkioiyle.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yuoyaplf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fmspeqkr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dvirmsat.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2pvgghckb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jjikjzuu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2azhfrivl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ybpjyxpe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2iuswmbhy.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2alhyukzc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zwofmffy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2muxkgybx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2olaomxlt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jjqlssgt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2narafwun.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2aakooekx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tsxxwkfj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wbpccjgi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2nwgupacy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2mcezyzay.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajaaydjh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2diqvqxur.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2unyouxve.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qjpmrkdf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2awtjuepe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2jftzweow.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2bxgnocup.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ejnwsogn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2odcbpvlk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2tnbrroyi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2nnduqita.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qfhaylum.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ctvfrwsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsvuohjc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ruanagpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grnqjpyy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ztnoymhz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbbhlmlq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bsbrwwkf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qnaxtgah.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dielghsg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2pvdzqjdd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2yprpsfig.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cwtjmewx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zyivwzvc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2dmrfeckk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vxfhnysj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2nvzznarf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2djclszdl.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dybfenrg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2qsbzjrxp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qezzzzjm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2koxsgyvo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2npqbpcjj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2awkoydki.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xvcinqlf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2znqoajcz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2indlqygh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fpjfhxqv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2qcetdwig.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2hnrgwlul.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2fhixmxxg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2dmpjcgoa.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jommcyfn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2gzeyxtyl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2irbzfntr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2uocecbsv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rxkmsqwl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nijsxeez.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nyijcwrs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2taoirjok.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2myzvtqmu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2byaynmyj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2hcgkwesw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2flnafuta.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mbzrkuuk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xnluvksb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rbdjdhyh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2acrolybr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rhrihuxm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2putanenk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2mkgkohku.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2adawaucv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2xxiudqdx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dqkqcvlz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lcusdtts.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qwmqnked.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2rkuflvnl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ekwfuerk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2lslamrdn.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mnwdccgg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2hqtayzik.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mhssyevd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2joypsoic.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2lytfsetx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2ezfhahbd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2rlgstjtt.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2qoyxkqic.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ghtgowtv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2iihvhewe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2xmzyavje.html


<!-- 参考信息 -->