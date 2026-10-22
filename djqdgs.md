代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kpfninrg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ynjyklda.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ygvksary.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emhwgpiq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nltrqsjo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzqvscaa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pkwysnxf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oytityym.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xnyldvtl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dwaotngn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ngnzbfeo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2detzulzm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2sotcjeay.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jkvjuadt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2apryrjkk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mwyojhtr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2niznduqv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yrzmmofq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nzbftjea.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lpgtofme.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlibsnzi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzziodyd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhdynlqb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iifmhwad.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2blwoivdf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2twrsieqb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yjkqygbf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cuknehig.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bhdigxip.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbidzuje.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2akqfbttk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tvvbjdbq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwsrlrkw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wrldyirp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nednzile.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ladenkvw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mcgpgrqk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nzewwwub.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2viqmizmz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlkitxss.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2laidadvw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ltyyytvl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rqmngvxs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2cvenepkc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hdpfdpyz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yeyhkkfd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2kjlloyec.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2zogjkrfl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mffdqwsi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mrerrwcz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ayxetpco.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2uhfigduo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2msmtaetl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2kkdhuijc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2mdpihlpk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2azrqnwpa.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jffmtuhb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ffidvgof.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jyeklbdm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqusgkwq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lrlllynh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xyunkhxb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fwdgusdc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2tcklhlbv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xkblisza.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mtwjiffy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vtohicuf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zwbphevi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsyecfzy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2oinctlzq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2txqezkmz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2euwmqjwk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qeccmzil.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dnogjjjm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2entgsnhb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2prndascd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zbrlwqnk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nbalritq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ptsfbplr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ebslkrgc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2kowrtfwq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vnzkrils.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kxvbkjbi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wnifagym.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hikceeny.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmmqmrxm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zmpveqwq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wpgusajh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wouryrrm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ircylbbd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jjjstxqq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uvtedqaw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ushtctpy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phfvssys.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2srhexgnw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcikshhr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eskmfmkv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hpydjecg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2shvdxkkd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tutfoecv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lsmkcssa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2umldcrku.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ykphavak.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jaqlnpem.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hauavekq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zlenxdhq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zcbdyfrd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ipalcqkf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kuikquvj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ceaelwiw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ojyiibwg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ssdjhbsw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dwzfqecs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpfctyvv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mhgjtfhe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vdxknlef.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wyyoxasg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wnvklxhy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kkyfkauv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lpyhyxgu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rgxjurun.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ejqrrlhf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2djadcxxj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gzkqwgcp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2chpuboaz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ypdiuaak.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jjqvdntr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mxcoccpu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2iwtlkkig.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xptomqtj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aszhxohj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zlmtopwe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ghxufdav.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2gldgknqj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nsfahsjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxjnjrwd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wgpeyerm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ackzhibo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vcmejcdk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2fqhgcdup.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbktlkea.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvlkzkei.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cntxbgxk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vjybytyb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xcraucgo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2exzyrfaj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qyzjzmue.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tyhyrwqv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kxggopin.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qajscmwk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2erjleloc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dtfddjfn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oyvryyxz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2dccqbkkr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pvhujvwq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hqfgswpf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wnamfblo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2oupwohtt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ljoiifxo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fknzxfpv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aelqmmve.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eqekiccj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2isazunpa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qqtkjyis.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ijgbghlk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kxnbnjnh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2wctftbif.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mearpjxr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ydbeoanu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2unvgtspb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgebtewt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2flqlxruu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ezsbvhcx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndtjltqk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mbzfdaqc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2catqtydi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wwwskyin.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zbrbhzvh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iokrwbjs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2isgordax.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fdzdxdrt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2uhfexcsd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nexnglej.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zslswiox.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wlxgsgpl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uaggteoj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mgmaclva.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zujvybno.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zwqxxpan.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2quezsski.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2pidbleon.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vvfyrkui.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2rgkhovkj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2octyvlea.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2izrugbck.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zlruurnb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lseugzjr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2fqejxdne.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2amiaobyg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2pthtvfki.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pultsddl.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2lkgcrmxi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hrzkmxco.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2vaxolbhr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xmrvzshk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2eefveypa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2xutolzgf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2faxvudqh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ualjktnm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2mqrbynch.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2mnzxjecl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2hhfmmgxf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xktghpmj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2yjxeuxpi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ucfvothk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2sfgcdnyu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2kniyxaxu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2gnesdddc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2bjgaciml.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2sdmqfnau.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2wueujzhq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2rlzzegca.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2armqbpnq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fjvxniem.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2xfgdinqb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2tucsdykp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ruimvehx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zwfurpeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdcqwjxl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2gbbaeomv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlrwknbb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2qzrujisi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yqwgxkfi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xaoisjtn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxvbfyyd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rlqqusrr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2vudsjiin.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujsayarf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fuoksijm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gfckasgm.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2joqpiymw.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fneykecf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2alfvztyd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2pdmsawwm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ykrnmcms.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2rqzoxnfx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjpawoo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fwidtxfy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iahrhbfs.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2aswxtzke.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2okburgls.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wvbewkjx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cqrlcbxi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2afbphxkx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2nfsfapsb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2buayjleh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2remqegdz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2rjxiawsv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ssnexxuo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2zhrecknf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bmgizagp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jeeprvkn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dunxjxzx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fbgaauhy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lpybxamm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2tbxljcar.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jxygftlp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2qnykzmih.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2zifcpzpn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aspnjhac.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zzspcpwf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jxunkqeo.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2mdixalpu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2tzdvhwxn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2byxjnfua.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2sinvfpms.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2xhmuczlt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2suyiptuv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2edyadswc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2bvriwkyq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gutjedvu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2isifgzyx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2feqovsuf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2hfasxnpb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sxngcjoi.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2nbejbcni.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2yyxhcyei.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vpcmmxye.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2kqcbetws.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2pbyydwpy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2vpwjldzz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvpfltm.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2qafcinue.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2zlrdakwa.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vnyiwglf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ncithvbx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2iosqvkqo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqzvvdk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gwaivavy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2djoarjhb.html


<!-- 参考信息 -->