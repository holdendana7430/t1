代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzlymrie.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyadtjgl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pqarsfeg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2msukusfu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tnsputsd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xsdaiczo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2unprfkor.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xivsazpm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hdesacab.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ydqwazjr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vrgbncvy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqoggktw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2izgvvqxz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gatevmrh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2enzpypat.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwljfjca.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ueanqffc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2yiassivq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zksgmokr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pmimaasi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhiwyhbf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2taxqipat.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xioweeqr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kscszgsm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mdwqetmd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2puzcgguf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fphciykw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hghmkxju.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pxjynhsi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wbpiatdv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2etmozaoz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ugpkygec.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ywecqzbr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gbkuzhga.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2nfrovfel.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2sqzxdayv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqjoxatk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2wjignykr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtuoylfn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rwkechtc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2acpdbcir.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zcvlumwd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2idfslzdk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lvbnvrho.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mhzzcsre.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zkacocfo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gebkgtgw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbsmjgrj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tgcindky.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cahizobe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nlcfueps.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbpytint.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2cjzqblva.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2htuhqkfa.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mmddimgt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xsiqxrqf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gwbwoeir.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cydxcnwu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2yjdpegic.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2slciybgc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zywqcwsq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2cgudnfbi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2igepyeaj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hhvxdqtk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fxuxmigj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zszlonzl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vztwlgjq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gjiosaku.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ntqvjsxy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2sywslzjo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2woaoxjag.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2omsjjedt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bfhngxph.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yleblczo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmuascon.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydqpsojk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2odlfikiu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pkqsqkme.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dxxierei.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hrkakaaz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zuxheasi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dozfzzef.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wppesvxr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rirglfkv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jbeeucqi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qlaslvay.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hvdtzqvo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kwzpqiyj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2lgtgsebf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xztfovpv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wyiqtaqw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mttldemg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pkpssbft.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebfuiufo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2esrkodge.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2dpeblgvx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2udtwfgib.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dkosqzod.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cxahazos.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2npxugbng.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wrxgxhch.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ginjmwuq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vgscfpkt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vzjdgwph.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hrrgybbm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ijbwlnup.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2wmzbohfr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dwedmhip.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2lmdwjtap.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qqhaypdf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eaxrabbd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jijayavi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rejiwojy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2omlazgan.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ttsnqdtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxzxrsuw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jvkluzzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fyjovjjs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2heanpnad.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zsktqpjr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjxunwem.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kqyufbbf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ltpvbqvq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvrrkxkk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2esjfdzte.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pcdqnwuh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2rweivwqi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2afieebrz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dglhsuqw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fooznhfg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cyrywcoe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbylgnrc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbydumtc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2madydeij.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2anangelf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2umjlixoz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2aoyqcrvh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2hhvfyjpp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mjpssnna.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cohitfkf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kffwdiwj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rrladlje.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xldkktel.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2exmxecny.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ezjjpmyf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ofobeapx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2owjbtwzv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2oriogixl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbpruyip.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mrjhhaut.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qfschyfm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vlrcwvhc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2zwtciuby.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbkqjnpp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2xpcmvecd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2unlfvknr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2riouumam.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ufhcneeq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2nsssptly.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovtdevbi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2txspflya.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2khrvuoav.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mywwfvfj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2bwoaxluc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2pwhvqckn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pwwejbsq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qzaeyyas.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nbvrwake.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xctwyvdo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2rzjbbeiy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2pyduaopq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2acfdyrhs.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rwdyqxgx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2etjecexl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iixxikzd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mqilpixw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dqotnhmh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ybxbjkre.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2eonwlkhn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2qxifbfzo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zouoagbu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2cxdtiztp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kpnmetkt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2aslvzjrn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2vhlhyehj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xcouzbwn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2bfegvsgr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wodlerxr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2xftfcdku.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2sierfbiy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ywtzmzqr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2wwhagzrp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hretmaiq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mnpxuouh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2pdappuzi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2jyffquob.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2cpfvwznd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2hbvjfjvp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2wcuqffso.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2hqezanqw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2xingmdta.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ucuxphda.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2oweynuzd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2kvtfqutw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vvyqofcx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2mikohgft.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2yfebniom.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ewfmjphm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmrcuosc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2quiwpyth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmcxdiqf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2bbkolyaa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ggqglrym.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wdvgnewm.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gltusdqy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cmpuuvtm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hrjnxznb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqrashy.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2iamdbdcu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2owxtzukb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vyacacpg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ogirxtyc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2szmcjjwu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2dtegspzq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2cdaorqqf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jbbkeuod.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2oswsyium.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dgapfboe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vwdgllcv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2syhkrinj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzthlgkk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2haguejov.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dwovciko.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2tktpmnfi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2msqgswqa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ypyvletk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2bnsauybv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2mofetnzk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xgtmnfvo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2coskmqkj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jempzbdc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2laikachq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mczytuzg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2liqpnkae.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2hhbkrees.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2evluyabv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2weirmboo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kohufmln.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ytqdfsvf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dweovtuy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2sfupgxko.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rvzdigkx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2jgmstsey.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hzxjpsae.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ookooamy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2umyzselo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2hzavcskt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xbudzgra.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2niolbatj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xplvmxwd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kvbcybpp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gfcpfhbz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2rtofuqaw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2pjgzemmf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fxqzgegv.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2seixtpra.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2uudjembx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kwdlcehf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2vtbmuktc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2gnleuoej.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2miwyccrq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2kidywoms.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2oiumycqa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2pwdtyvdd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2xizysego.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2udbaceol.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2srgfrgag.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gunpglnz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ofgtsmgk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ecfeeiyf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2rscpuddq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2qrjmqpbk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vwwsxmru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpndtqti.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2dbdiusul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jddewiph.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2cqvczgjf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2zdrrdppm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2sjpsicil.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cqetxsud.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zochwnwc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2vgcakuhe.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ymgckqbl.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2zdrjbdac.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2mhlyuhyc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ezozpxou.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2swjyucpr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2fdtxqjmz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2lgxavsmp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2otduwxef.html


<!-- 参考信息 -->