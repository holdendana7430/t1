代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mepjrtcb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ivvhwqea.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wdaqjlby.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rgjikcku.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwalksfm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2pohyqhcf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2otxuljdc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rjwdfvtc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbcbkrso.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qexqupzc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2spppclpb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rnhodxbn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wlquuonc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gujnwztx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rsvrtfky.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2awxvnmrw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qrjslnuj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dbvltsiq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bgewdbgz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qydtghnp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2swtnzycf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ittuibgt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jmfonrvc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gxlumgzc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgpgeuab.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nrtiqgoz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiozilak.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwohcdgz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ludtqvob.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2itvrbbwc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2boonnole.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fcygzosh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ctwdwmol.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kzdszmqq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mzrzzzez.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziaxnrrd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nwxuokpi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2oehyccpx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2upprnhdz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2elxsxeoy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xlwfufgr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2trimesyu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuvyiaqd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dvldtteh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkdevdtm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wnyigszh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2cqgczxeq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2moomegyv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bajeogfw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dugboghh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ovgqzpof.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qjjmwajm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dvvxxkiv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wlvsyxxh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qjejfikp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bxybcqud.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xzmpiwsj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2umwfqcxv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ezciyhsv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2eulnhhqr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qjigllat.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uxaoksmc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fiwlwopd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2glerxnwd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ldszsuua.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gwxlomqc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2biuxtmdj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bgnywzbe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2diwfijpm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyrjxicq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ybiveqjd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vjehxdym.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2szcjeidx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lubyzpeh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2elngepyr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gaogqxyb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nphvnzpp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fxkvgnne.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tcioqqim.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hrqkebsx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kmtajmak.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bsufxukp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mrdujlih.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yfvfjwbb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2oykahtsd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gztogodt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2rrdquuqx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iblwtyfa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2awxpundo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tblhdoku.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bichqyic.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2naahfmry.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lquinqwq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuxjjqim.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2mxcyylsn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2otioongc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2msavgxdn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxtfzwcf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2usbslweg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vnwzvseb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bajpqwuw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2igvkhqyu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2idjwqren.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2kwmpphjq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bzqiqtgv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lvnudrds.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fntubhwj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qpzevuqz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xzfdtxbf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gkigamzr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ezmnzqze.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2fuiuwqnq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yhrtcfcb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2drlsunia.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2matkzyxe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2pbxrofyh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2yiyxeldk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tebbebeo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zyqugucd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xqldhswl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2znsjcquo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lhzikwhj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hewgjmeb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yfecdcaj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2njivpcnx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2prwoimim.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yswkxkjp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2bsbcwgbl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xefqkjqh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kxfhkjrr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vvhxoesz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zgndmybg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nebcryll.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2smyqqtpy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dugsrepl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2naobcswp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2awmkjlxd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2sauaqjog.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eumesqja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2givvuaex.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ykdletdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocqqwokz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jbvspdwc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mltntoow.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmxvykhj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfyfaevq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rsomrywr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mrohsbrn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2paohppgw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2pjxxauov.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2czhczqao.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jscmgfgj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wrtpkzvh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2txxebych.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqmrhwbr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqvmwdlf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cykwyfrg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2vslbsjqf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2olimovkr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2naifdulo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mdxbcwpu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2exltsdxi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2reuuopbg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2emuvauos.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ibohqqla.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nfrmzqvz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2dyiyfudx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bfbycdnj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pgkcbuzj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2msvcldyg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rcyjaoju.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2icvvxyry.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgoqeohn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zywrwdvj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2djtroeqg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hpqhcdgn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ikkdzwtx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2prseqxsl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2udmxiwtl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2impizipe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pqvjixsm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfmsmvya.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2baxhciok.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyasbrtg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mwrnrdnq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2htbwilpf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2jzkidzdb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dysvitjc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2chivjstk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fpihrhnl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gchoivhl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rhlrlpre.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mdcxjukz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2saidwekj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2sgvlnjhr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rbbzcfrm.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vmqbdrgq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2epdqtjez.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xqpzorbb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wwsgxzyd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ysknfopk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2trupzgfl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ukallkam.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2uexeagpl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hjczqjmk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2uavcutqt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ufujpjsl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xffosjcf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2npynxviq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fpfqsjuz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2gspoleye.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2xzqjbqrc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2idmfugfd.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dzieteod.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gpzmnddt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2zltslyjf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gsbjrdjo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xszzltpq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2crtijyib.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2gjxccfrz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2wvnlbixf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ucutmjxe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lcuhshli.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2veseeaoz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2eqkrqzxl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2hmbigcmq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wyseyqmj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ghaeyvcb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2atcykwjh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2nbwjwgij.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2khpsccsp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fijqepdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlnaymfn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wiitzugi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmnuhthc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zmkymuns.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nmbmgjda.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2deptwrul.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2paonrxdc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2taekfjnj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2bkghwuxy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2upkzldrk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tbacypyl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2iooaqmzb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kpgeyozy.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxqyknzs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2cypjqnfp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2gxxwtaeh.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qbrmgjgu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2owhwysmc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnwakire.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ubgaijek.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jabjylss.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2lxkdxumb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ajyycava.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xafbxoqc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uvfhymkz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2amgeicuy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2tnullgrj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2khnbxgyy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2wbcznqao.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2zjupvahu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nfceloxl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2fewwbhip.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqgzgixo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dcxueipw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jdjfxcaq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mvkcywrd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2rkqfgady.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gjjevhal.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2tnjjwzfd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2zwcrncoy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iupgeuno.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2miupghyz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ihszbofl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wjhuzpao.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2cnzycoji.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsksjkup.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zaeebrth.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rvsowyjt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2eoxhjgxy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wufnanwh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2fanbacqr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2sqfucmyr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2cbaeucdd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2szldphqx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2qtmrrjzr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2lcrxhbmk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2sectcrwy.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2qabpamuz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2keofqqtp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2awdnpdxh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2xxuuztss.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2tbxfelco.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2aoznpfva.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2feriecks.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2qqwetjlq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2klwbdppi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2zjzccgiq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2glryrrlp.html


<!-- 参考信息 -->