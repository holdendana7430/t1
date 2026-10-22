代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2slufqhbg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kekqdqdm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kyukfury.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzafxclv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgxdwyiq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2wyudsbfb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bjsbwvtu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2drhqyljk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zgvhhdwh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qckjdidp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wljdfvht.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qeacqbmo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ocuszabq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lxjthtgn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kxvnloot.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jjzwpxud.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjjjwboh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkqahwrq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vgqsikcf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gmkuwyph.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2owltlcfx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2smdfysiw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vwtqkadh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hbfgiofc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mkyxdhib.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jofguzqs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kitvbhyp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsmxegfk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lztukltb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2sjgcvmhj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lsiruuxa.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkfvtfuz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sjlquuep.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2owscckod.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ggwlblge.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ycyayzbi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eexazqns.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvcsxikv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wcslocqq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kxiimbvn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ivcejzuj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zjfxjdly.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2uqnqyran.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2snddihmg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2weosqtkp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lzgorymp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ujhqqsbv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hqpvewuw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bhiiuxez.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fuuhihsw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zwzdingq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2osgkbjfb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ivmvilnw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfqyepcp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2vodxlvsf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zipehjpn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2iiiswrti.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ygomnzjo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2semoogzj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qjnjnixw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mhwwrisw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucmyullh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zujtsysc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2femidwgx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjbffmaq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bpwodhoo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2takynkmd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkvymwkl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2dcqpvsuj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zxbsceee.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oqawbvsb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vfryqpbl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2afeluxwq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ufbvxtvf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wbwlefux.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ypybddbm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lbgnkwgl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lsebqdqa.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qoidxslz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqvvsunu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntfekolr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sjbqlmhd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2waehrdgj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bbzbgunb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2dnuvagjl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bidbgqng.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kiyqykjz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pluqmber.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ygsafgwr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ejqytasx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2syocfogy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egyypfsa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ixwjqffz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uzjqizbj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vcarmnyi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2eamsnrdz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bftohrat.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kjagtxol.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bcxnnvlh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dimavxhz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2erofexqf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vrwwgjfj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2eezijfda.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2iqotgubw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cpmsnorp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ndddlmsa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2enbszcid.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lmlbtwsl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2iflvxprj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ihycukll.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2pzwwfcso.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qykyzlzl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kmtbfros.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eutwiczc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ihwxerzo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ymhinlem.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mlsokruw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vivwipkj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ibxkvzew.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2kolvwlpf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2dxdcrpyg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vbjcatef.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xqzvuedc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2xfayxnvt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kjdwlhhq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2iftnxplx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vkixjtvc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mxxhezmo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xzohicem.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xpehuzuf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dmxccjmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uamwyikj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2bwinemgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jusatnfc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kyogbuac.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mkkkfmfl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2autdpbqj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypznabvg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqrdaaxz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmxttcuw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fwqtjcmp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fhnbmvan.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ezzhemod.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xxhnkryh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2dbmueaat.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2btrkjfpf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2entpdsgu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mkhiuplw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlpvcmzt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zptmeavz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2idurtonq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnwiuhgc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fwnvdmxx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2eowlnddm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zqoicwvd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jnilniuy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zltdnjam.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cviwoqpc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ylefszbp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hsakxntn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lscdaqwv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jezbscgn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pcxbobmp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yycyyzhv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dpceajpp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ngujqxhr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqlgdcgr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2gsidwvys.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vtzphhuj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wawrtrbq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2povnthha.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2pwliwxzu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xjrhmoen.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcamuims.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbfvsrax.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vkfhrpnn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2isrysakv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vjedwhgt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cyrowvgn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cechugxz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2eurwqmye.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ualmuayv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oajtfovp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ipytwaxl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2zryrsdap.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2gvurwqce.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dlylrjlx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ocoocgan.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2vpcnusls.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2riwbrwtr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xcwyvvin.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vngzquec.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2luuujqzf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bexwckpk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xymgkvas.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2itdeaqdb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pcyarduu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2wvwelpxa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2tyhtgfqz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2yoomrxjb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2zptueoui.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2erebewqm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jzmhqjor.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2mqvmmqat.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2kcwqpqku.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2grssvhwo.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wlvocybn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2wjhcakum.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vkrclupu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2eshuowuz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2bphjavdg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2evjktssu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2frcmhmgz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2pugokmzp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2cacggnba.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rbmmkkog.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2xsuhvujs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2pkmqyzcp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vciascde.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ytxhpqyz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2bjurmbwo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2xcbudkpo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2mscxymio.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2krrfqnzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adunwqrn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ncmxydnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giyyxenw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2sbeuzlsd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlrepdnu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tbzfoabg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lodorsou.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2weljllpm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2gsbrkwwq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wppggvdf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rgeoszoo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gnmoqidx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cdmstjin.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2markbqiz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2selzzpom.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ljukyqaf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fwjawbwl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2dxaojmte.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ukrjslzn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2yorabeox.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qerdpumn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2mnhpeswt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2msvvjjet.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2wbastobz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yktddxcy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dpsvrnan.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2idntvgxl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2cbfdizvq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2mrwlzrcs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2amwiqewk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2pfllmzfx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ibrttxyj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vsfvxgkv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2skbdqijd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2twmwvbtk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hhgvkzfg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sfyfwezs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2itcrlfhb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2axxnosqi.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2omjvuzsn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rzsoicim.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2osajrjen.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2risesvox.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ptcmpdok.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2qfpwbnhn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ncepmijm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yeytijlx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qcltowmg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ycchjiun.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ytstmxtw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2dgksernr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2tbyksttc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2xxtvknwk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2eufnlnws.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2jowkstpu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2bylcpmvz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2innehrrj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mfntachg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2iqgwxykf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2sekwabhl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ayyzlpdf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2jbwaaplx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2eualbktw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2bvzojgwn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2hojnnvna.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2huoxzcnd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2owdoasoh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ulkawdkk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2muhwwyzd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gvwxjrqw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2sxdpishv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2aptsfavi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2sqmealfa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2hitrpsgg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2jwhzrrhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecqiyffp.html


<!-- 参考信息 -->