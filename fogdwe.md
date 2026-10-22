代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2vvjugbal.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dlztpdzl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hrfmexsn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mjfejbiq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrefuleg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oacghaeo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mkeuqjbc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2afjygqsz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsqomims.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bxyclnhj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gabgnccl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2krjlmaci.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pwqigyfn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2clebjkwu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2psjrtvik.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ydoduolq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mbetcpka.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2sjmepsti.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tbpdnomf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rhpguxgb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ymierlov.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2srvwniay.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxxtyhoh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2esyiwblg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hfggloks.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2thmcmrim.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2coppkvhh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2nsasvhoi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xsnlpfrc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2whbvwvus.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljbykjlm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqtadllo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yacloozo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2sibbwfmt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2oklsdtba.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xsjpmcyi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2digxcrmb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xaueaqjs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bbrbpwtb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rdnstlbt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2utcuoenn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufpirjwi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rrhwvewi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dahotwfh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mpxylaxe.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kqpxdykp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ywgaylwp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2olnkprks.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xgpfndcr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jkellyco.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sqsynwqt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2eguxeitu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zbytenmb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2voyjgvvf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rmcavgka.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2tfwaveoc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezgwcxje.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogzmwkml.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdoiazkr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjjjdcku.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wbfpyxal.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2amlaawaj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rmdqkevz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mujnpyyd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2draiqnuz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zhsvhhcp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zvrqbatl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2guonykba.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2erejcqcb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2jvsjeluv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ubpzcgtk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwgfpnqy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wiowstea.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xksjjjac.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fwowwdcm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2svwpygwg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cllilezi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vxltsxqo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bkxgbeod.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dschjdki.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dlygjqxj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qaskthok.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mcidtsqh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrdwnyzu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wigjxubw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oigltdoo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2anzwevwi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cmwwxrek.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ttmrbmpo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fbmmgonz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mutkassa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vrivelve.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvunqscl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ampdnxrk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttjkrozg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cldabwpd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qcfnaowe.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bewtwris.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uwgmmkxy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2aecwdxjs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rvvfdbjc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zobwwcnq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fovwlemq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gwxxyojw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ltmsnovj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xrqsyzfm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2niyomvpv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2yhnzuxxo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2joheuccb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2igxfnbff.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xbrvrnpl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jifyphmw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wlcboyxu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ablohmez.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2iwbocyje.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2jvwxzmoy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2caidihsi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2aupkakya.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2bptaprrc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nrqvwmze.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2qerdtugr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cqadofiu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tnzybsjg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jyssgtvd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lksorbcu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2meyxrocm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ngzsonvw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2opujptvh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2snjcmikw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cwqdcqsr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkwwcsb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hscjknci.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2etfkldrt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2vovkosii.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rpjbbmne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2totfodgv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pvdtotmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acavovea.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ujfffszl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2nykwlpew.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlaqynrz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nyanqmer.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvxnuabe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ncpuwbjy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2sveaejfl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2fmjtidwo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ocmvwcmq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lstqiunk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2urystccv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2buhdckxh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqfqcdaq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxaljnuc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jtzyfpcu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ccvmdufo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2nuqibssd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzpwwfbc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kodlqmiu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lybmgzqw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ttiybvlq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2unwkmbpw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tgjztivi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2syswynfj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2wbyzhpqj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lqwxkkoq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xxpjtqnp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2njmdidbm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qaxdpvtt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2itqoxkin.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2waictigi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2swlixrhv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vfzwdmbi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rujjneac.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mdgdzrgf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2totqkqtt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2foyzuyho.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gtrjfnvi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2exiorgbo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnjomuui.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypdvdqqw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnrhlvec.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xdnlrrkn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2avmjcbwt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpzjkhgj.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bagxcczj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2laizkwbw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jgmetbfa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oywltroo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2edrfbsut.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2bjseotmd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pqworzvg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqyusnqq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2llezfyba.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2cgcbyswu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ddjwnipb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2exaduqvh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xfrfvvqd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lgjyzptv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hbdiubnz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2admdxeyp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vadmmehj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jpqpxppo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2hpifjkyu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wzjyrkxh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2glszrgtu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ccejauqu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jsqjuxbp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ftghaloj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vurtchqr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2nzquzjxq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xabhbwhu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2aqaekape.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2nynpmtom.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ehwgxguy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2omzugbkn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ifkqwtzi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2imnephxp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xrgbokkk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jspzdhlh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hiabzstx.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2lovrqcsf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2kpkgrxqc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2xrudkgqy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kmxdfmob.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2onrpoojt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2uqvezmfv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2aopofpdc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ezvswuyc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2upcwzwnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtxukabn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2djfbluhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxzmgucx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2nipmwoti.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nwgmflvu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssoqqcvy.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cmdrsabx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvvtgaq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2yldpcjgx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2odcxamxn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2szyrkneu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2moepemgv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qmkahcvw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vapfgjmr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fhppstyk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2bbwxuxgj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dhgcjiac.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qannykrx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xwuhwkak.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tzppasvr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zjzbvdfy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2pnfgkckd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wtshwpbw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ykegbfbg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2yuhkysft.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vhkvffcx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2imfqyyyw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2evlcfkjc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2myzdynyj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2iimlkxbd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2xsrawsnf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdqmvtb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfdtlsse.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2crfbwplb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2pohcquzr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fiehqmtt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2upodjbuk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ekcwgxxl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gbvasgnq.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2yjrtrpyw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yznfubnv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ugyehtcx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mnmytsto.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jewduvhe.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ogwghefx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2nfolndlt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2eseqjndl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2tthfslly.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ugtlqbmw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hqlmnuqv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2fqiyuzfg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2cbzhqzyu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2igxfbixq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ogtofabl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2nayhfxxd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ajnipwne.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nxrxttsp.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2cpxqiwur.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2gznmiqit.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ylmsqbzv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2sirckbha.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2lqbwsjui.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2sitqgupj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2wolrvufd.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2bvxubpgw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2cbasjwie.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ujnxnogc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2kmgldxrz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wcadrhcj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2riwfljro.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2eagsbays.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2dwtzothm.html


<!-- 参考信息 -->