代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnwxlcay.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otqbqwne.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fmrvsguv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zljmlqyg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jbhytzop.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kbfaetaj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jkiokpxe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vlvajqya.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yjdvobto.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzlgdisg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tdjcmrne.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ursoozlc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyucxqxu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3pmyfvquo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vcbctsks.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxsnnlpo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ycmxfvnu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tuveycwj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ltzxyafa.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zczkwdjn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xafoivou.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeqilhjy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cqimbfgm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xhdjcdef.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mpbnijep.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rvvyengo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3grkrejpr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3wjflqpio.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zzwjwbjg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ygtiilnb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jajnodyw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hdhhftyb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3chwdrmsy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rasgjmdc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3abnnpspi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qpjzomxb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezqucfww.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yehfwiwt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrmejyey.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3usecywss.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cfujjphe.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgutgghh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3etipfpxl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wotisogk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dqpesokk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpttlgvk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3nqlatwvx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqcygkvd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nklqiowj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xvsckygv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3selskmvy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eotzltke.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kdjnhger.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3mcmtdfpd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kjrevfba.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lvbfhvhn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jjilxnwv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ychorvxc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3cywmikpn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dxmwxfbt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tlvuwgsz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mzlwuejx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zgqpzznr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xyvwatlq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fmqdzblj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cfxxswtp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3neaykhip.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gnkujdlc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ltjmaacw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zlwhtapj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tfjcjgss.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3thrdfeby.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wkyfbrhw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pwguekxd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwpcakoq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvnhatmy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wlvhxtnn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xedzeiwj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mvpyczyk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tbipuqej.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ynfjqkpt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yanfdtxl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fmkboqse.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vadnbpnt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nknnqcrg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mapawvee.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3tkxjzhfw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3unijhfbv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hhwiyvhg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gylswadc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3acetrzeh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xhqsrxor.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3onufezbg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3sggtrgjn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3iloodupf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3juburnul.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3rxjaaxxa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aiodgwpd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3iddsgwgt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltzicgan.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3rzwoczxn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rrchktaf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ifxyibev.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qveiofsa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3bsxgqdhg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nmjacxzy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qnjmnvxc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ylbixrtz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3whdmdtlt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xwrlcwsr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fkdpudtx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3qipebxcz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jmohqnvv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3iecucrsh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xkpqdsxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eaavjows.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eeloatvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yflgbghr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mfuempld.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3brvkrezk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzcodkiy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnuidbrv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3aaneznpr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gptrahud.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3azokgoxo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3bktqeetu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxcyxutp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3bzjkmctq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3gwodzlje.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpqlqfid.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mgcgqghg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gdomhiez.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3anhbfdde.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3pderlymd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3imbhcynt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbmjnbiu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gtuqishb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3txgliwaz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ghgxwlul.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ekilzaww.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zjodlxje.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lbrtzfsz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qbethcnq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hymagykv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mlgbxlrv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3mvlgvuzv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vdpctbfd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkmtfpmc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xvxzldhx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hqfcfcpg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ancuntib.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3rdcjoslt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3gyhasstq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ezhoizxt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3djvslhbe.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3abtbfily.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3kdjhawfq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cdjburfk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnyueuws.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ijvbyupn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3nuttmhmh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3nkazgsfg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3iefivjph.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jqfvfehk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3fmadbglk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fabcvkmj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qlipypsg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3enowchpp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xrvjyzmy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3jnzmitbh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3nstoazek.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3znlxewgz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rfukuppy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3begmyelt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ncayotmo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zgsgikaj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3htqlqupp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3owfjluyl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3mzeblyck.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3optugptd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bfmjnrpk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xthozlbb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3nokbmcco.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3jrjoiprq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3eqfuawua.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3dfwjpclk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fopvypix.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3oefskrtx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3henmmtiv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3iwpiflrf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3twabhhoj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3agnglknf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3aahjhgzy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3fnrujqhx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ncltvcak.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3axsqgffo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3yflnnvme.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3zptsxxog.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vznrkgjt.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qxtjpefj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3dsmicsww.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3weyuzoiv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yskmgrxk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rmmttcuz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3nzyjmilr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3aynhpgzy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3pqpgwyov.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qpkudkes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzvyhhmw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3rrceiozw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njydcysq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zcsjbwgd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wfghxgwb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lkwviqjz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3eoerbqmf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qgttlbvn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3jsndhtqs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ozvjhrqm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fsxbbtel.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vefflvol.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wpullayo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3emnaaqor.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3vhurutdr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3wsudhkbz.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3udtgnizy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ccqadxgk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikizecrb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3iuwuxkdl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ljdkjals.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ghseiehp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3qqwkmgfp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3dylgxjol.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3xjftxnco.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3auyhlcui.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nivbmrti.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3mdlgbxso.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3kshhcyuu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3nvpfoatt.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zenkkjsk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxcejjso.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cjqivtlp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kocyanfy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fnnkbfss.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zbzjxhys.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3weswfnnz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3vncnkiuz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tofqxylz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ktiuoqpc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3aarlpuvy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ratsmvmw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qghlbulw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ijmpgkoo.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3zpreakgk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qdmgnxja.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3npngkzgr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3bhqigglb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ncprdtvx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3oirvrbri.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ztytvrua.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3zjeelhli.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3drroeqvj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3urqbanhp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3gguyruhx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3qgykfvjn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ferhwios.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3jirqicts.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3olnxshdp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3anhdfbwh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ykzkdxcg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3hwfwalzx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3fugfjgqi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3wrqvbiqn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3xjiyhqzw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3bjtmbtvx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nphlzyzh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3dcljvubj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3yncjkgmg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bmzrmkvr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3kergqdhq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ygdlsmuw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ssnibgiy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3lddnxvdz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3pwlfavkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hitctwkc.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3hqenpccb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqbjogjk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ltrlaxdo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3kojzhhee.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3olfgtvhd.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3aifycfkx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ouoybdxn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3lupgucvp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ywvgvzeb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3mlkpctoh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3aedcolxv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pvcywepl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3abiwhfrn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ntcckpmi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3scbhmgcw.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3rhylkvcy.html


<!-- 参考信息 -->