代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hyyulvtx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2thnkfmai.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyalvawb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bhxmphmt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wihdhcfj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jeacyhuc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2krrvpwta.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdqdgsox.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2adrywepi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tucsmhsy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qqptgixx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggqvsxol.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtfwpost.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2blbnffpv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2noavclra.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2avowtgno.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tbiazymw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mnljtxsu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tkmbdvml.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wrjxuqpv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ldhjcxiq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hzsqljbf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pzwodfkr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cufzomqn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mhsksmay.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2himaucku.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2colodxps.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zoaxwevm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tvuomrco.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zuzjamsr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2evctmoim.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvvclwmm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yslglkzf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ntajdnme.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvfobe.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2aizzhmvh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2saycnrge.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouhxoniy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rdzgjvjb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ywcdkjrr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2batzbsax.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2epoygxus.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ryroznqn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfdkhndu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mdmadrcf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qhqjflmv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fdyjyshz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewgqoiqu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oawwdvma.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shplxsgz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2oxiqfibo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vitylxmu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xsaszpce.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bdoktnbj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jrxtvqgs.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xxrhsqig.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2irzmkwdu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ubisrgok.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zixppnun.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2krwqpujl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yphpzsls.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sbwhckay.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2olhmeswf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yupodlve.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vejytbcp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lglmujeh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zehmdnng.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mzfhrhwz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ylceztst.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jiavtjst.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bahyafwn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2szjbenpd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rqtbuned.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nwojhuph.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cocziwwq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ddmwemmx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylcwapcl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mxbdiwkn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qiwjpley.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fexghwrm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nlctmcng.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2odhluwzn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pygbdwuc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2sgvkrjbx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hxvqdhdv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ghhskcwv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ytjfaefh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2srvknkct.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2znosgjzq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xykuycci.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qogxjsxa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bicyzbwx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uhecyqdb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sisffflf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtqlglce.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uhilfujk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2qzfoyleq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqvixcje.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gojofmhc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zgtduyfg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gfmlpvdq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gsvwwlei.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kjuxpttr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xdamjclp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yiecyuzs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hutodajp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ulufzyzw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xaadtqga.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hvmefcsj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2epdmbbhi.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2emcuqwkg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2esuwfcnp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uemiyysb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lrnwhzbq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2iiqcvont.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ujxwdhwr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2samfddjc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zxfqxjzv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jcukdtog.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2mkbyfnig.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2syparlxo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkzyfsth.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zidzrxmu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2teyylntw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2iuzzdmqa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zttjmvof.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vmlqvqxj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fstgbvgt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2agrhuwys.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vlygsidv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2imfmltmr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pttzkmdn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2taxcrtab.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2songgwvz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lstehsjy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2iyrwxrqk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2pajskxho.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ffmjuktn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vxuylvhu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dsxuoued.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2fppsaqzm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zszilcka.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xptyabbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zutcpysr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rddewisn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lyjjhisy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jwnkvsft.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vkwcedjh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2dcmvebxi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jhpoowul.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jnhqjman.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2larvwblj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rawkweci.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2gejvqaqu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dtmchcwt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wxslobxr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ufucxcxh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmpmkfpo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljsxcjut.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfmdgdnf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2knqvagzt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ucgkjsnn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2dxghyfaz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ntidfgpj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ibmzegmp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wiqmivom.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rtziitko.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2khgxlxjq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lyljrwhe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nwjukvxt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2esjtuwbw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vklgkjgx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xjxeyvnx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2xuqasera.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fleqrtzk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsoqskis.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2edmyuudr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2layltvnm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykaktcht.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pchwiqfv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydndsvzt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bbrvrhay.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhroocph.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2djfihffy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2tzrrccnb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwucrzju.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iiogomif.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2qtapbxck.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2cwxagtes.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2feebnkfx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubctltit.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2rkgvcnuc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2mshsrztn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fwazgwse.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tryrrsec.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2digiiwky.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2sswbxfxu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kdeejkjk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2bsbinwmf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ejibmktu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ykyhclcu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fukukoed.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sqiymryg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jujfjxjk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iwaxecho.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gkxkahez.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lyboruxv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nhyvjidg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2amnplpbc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2boedhnuo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2nfduxyus.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2aabngupv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2grpngfkw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gvehuidf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dsamzmwz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ibahvrox.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2kvjccgze.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2wuczhlzi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2momieopp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kybglprm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qrdzfdgw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2yednstrj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2clsvqqef.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgwgehwv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dfkcibyj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2puplspkj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jxosdylc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2acdtzxct.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rvksyiqf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dbvpidtp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ezlvclgq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ydflqfan.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2nvndalka.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2scdcxwio.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bboprksp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gwxyojxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uadcfkzd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nmcadhvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmrvnsqg.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lzpryhvl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rolmxtyh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zccioiyv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vmxdjusm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eifyearv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2icambmiv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucrnlksj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2khlycnxc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2buyurjcl.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2dzsuujzw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gvtkggkt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2vndgmavw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2oikiqddi.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2qglonxnz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2qchahwgq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2apeawlqw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2kuwhhbrf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ksjqpgcy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2rgpvhyij.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2dkvvxrjr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2rnnjkdwe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2divgxafx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lyxexxtg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2siqjehno.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2jgoufiot.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2qesbiigr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jknhbxhy.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lmdoghws.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2uyzdycpg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2usrppajq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rjnztioy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ldrjzsot.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2erlfsadm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2nvebsljh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rlpuxqux.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fumldegs.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2cgpqxqfy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ouxcdxuv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ptloaizu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bpqftaza.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pmhflgan.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2arhvsdam.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2evpscrho.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vctyoycq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ydfaxhxh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2eelrxlmp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qgsrwhli.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2jjypcsdo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hvwchyta.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2blfslqaz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cnjxthrt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2volocfqz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2oheqepyo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pqdgbcwx.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2lfkbeibu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ppjmllhh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lidmmjzq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2axfxtact.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2jltykelz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2agocvtmb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2wqiqmfyo.html


<!-- 参考信息 -->