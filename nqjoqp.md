代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tgiufoyv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjjqjzxi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kfmcgivy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vummsivi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dmladbdl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nekxcmyb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dqwgkwwu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dllvxomg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ttaprdjh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pdntyzdv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2mosfejdf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fnbiknfv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dtkfcqdy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hfvigrwa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xevdxslx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zdswpuyn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2orfrrmtq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lshgdafr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dtzlgewi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbgnunld.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ikondbtx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2occigweq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wfehpgyu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2floyzixc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2juzvnrsd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2phxcltdu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlhpvpvn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xczhecmw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxatenmf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2kaivcghi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bzlqvtsx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2neyhpbss.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gmzufbee.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2efpwbbdi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mloaoqok.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2featdvss.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tccgbzoe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2suqarzur.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bjjhmhnn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2oqyevsqs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dlcilfak.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2miaejugs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2enibjqxa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vchbidjb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2etkxygpe.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bhujgvwb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ckezucek.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lzrlafln.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ezmlcyjo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2xmzgbcbf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bzzmfmge.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zrnppyyf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvxeluvj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqsyacdz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmhkwjer.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgfmbuvp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2itkdkpqc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2pcilsegh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zragnyec.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2uznlqrnc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uwndbzts.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2qgyaucqg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vzarkfiw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vlpkjhcu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2peufkrmy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2iecfxeje.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yrcjsfyh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hhllnrxr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ezwgbzzj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2eyczmwbu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fngxsejx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zpuvqfzv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ahknkora.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2drqtgfaw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ykjzpldd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yivmhtgj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hkjerbxf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xltbogvb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xcmreufz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qszwsrwj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abssqjbe.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kmkfwcul.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sodvxvsc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zawddctb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2pjugskjy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsdgunjy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fpqbuyim.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fepookzq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jvhjjjih.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2woiczyrd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zdvbuhvl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gloyvrho.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ljvxrzdu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2txqeivwf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ycwozwjr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2irkdeyut.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fsjnvmor.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rftwrehi.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kypadhot.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qziosokx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ellcuace.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jozaqtau.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2daqylkao.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pasuinkb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xckyazpy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2umicfmwe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2tohmjmoc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ktxiemlu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ofxwapej.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnxxtppl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fbpbonyc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ofiqycim.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2dlawrlmj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mhvuqmkb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2htwfcxjt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2xclgsyyn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zhdobtqp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nugcchqp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zpqgbzht.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xjapcxyq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2flhjubkp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vroyyabd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ulhwuuvb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vxetmhwo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wusshqka.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ztgyohgz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2msxtneqv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fibmomut.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gaegdmlk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vxvzvbab.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vkxczhlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avfwuxkj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lqexrrke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwyaqfzb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xkyccbls.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2slocvtfk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjsxbmhk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsgbjxtj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlhvayky.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2iddrcznj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2yryhppon.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2eurtlbjm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymfzgota.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wyjnfsln.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2emtsjnfu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2blsrjyca.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkvwgdms.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrnimvcy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ludpgkpv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2odhhcxmu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2vidttubd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpneyhbg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hrjcmqix.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2boltuqzh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mhxtjvqb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ycallsan.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rlbnavmm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2txuthurj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2psgbhagq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2uzutfqwa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hstwygog.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tnmijszi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xwvnhvjx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fpylecwj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2eytdravr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdwihcmy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jfowgzua.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2aylrltja.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2nwkfcfwa.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhtwluwf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2yqaoukgz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2atlwfzzt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xybzyubi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mhaphgjf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2opjscfuf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bayntxiv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ibmniumx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2xnkdysaq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyatnfri.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2bfjycxfh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2sjgafgsg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jvfgklqp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wfhciqoc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bejwikbk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hhfftezk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xaovjmfp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ucgpihom.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zypjizje.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2fqyfsubx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2gpcwlqwx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2paofxggg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lznqtjdp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qgnuvspn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2irvqbppc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xletcndb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2cfvduqwj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nrcmknkl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bsxwxhhr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2hcwzvlbz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2migncgcf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2kjniwhqe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2dwinhvwc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2hukkmfjk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2fbzxogeo.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xunijbxx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2wuxjsnff.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xzudypjf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2dbgcmnon.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2cljscgas.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2kgfypiwl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ndekywfk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2lhtzjubc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ocxuimue.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2mfplgefa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2fglvlpqr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zqgtckch.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2sqiziqzf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zeoblvnm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xcmvvpce.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2kyayurkt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2klylnrza.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2azyrglvk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vchpvaro.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iwhxvomh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfvsespa.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2fynievrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sozuatlg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ziwpezwf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jkvpwrnp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2atfvvhft.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2znekcomo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2enkjogfg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2paadgjhx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wznmqhiv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dthabwlb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mrehcomk.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2wmnxvnki.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mcpkrdsj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hxwvpbdn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2xqplpdus.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dmopfaxo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vdlpmzvj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjfuugyi.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2iikoplfi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ywengdgi.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2swfcwdtc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxjshtg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ykhevbln.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2lwqzprip.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ijwparto.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2kjpmsbgc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2luindrid.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2mjomkidp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yqurlmug.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2rlfxrzak.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pebhgdve.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ecurcdhn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lyatbxhu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2faqbjjaf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ehgesnzs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2uuvhndhb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2msvhlxqq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2rcblwydh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ueuwplup.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jbhvrfyr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gdjulnsl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2odzimljs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zagsoyrh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2aaqldfur.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ftsdhmij.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gsvbfeqn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2yrmbecil.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2tqjztvci.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ydrmfrqp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2waqbhtoq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lvqvdxsl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qouptglt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ukebyoht.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2onwabcno.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2gwimarxf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2daebeort.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2cuivpfrr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ucnxlpkv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2xolxmujj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2azjumzds.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ujfipxbx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2zbasyurh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2jtrqdmaf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2fvafwurb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2egbsowzw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2irgvtcto.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2oucdqigf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ufukilgq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2giouzldi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gibdttli.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2mvqwnjfe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2mrufbgrk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2mefbienv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uhxswknl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsqvasbd.html


<!-- 参考信息 -->