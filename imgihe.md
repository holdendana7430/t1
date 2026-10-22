代发 wailian999

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iuoycmwi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2clwlowzi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbcrezyv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gxmaxidk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrfkuguz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lfryrnfr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmqdwciy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfvvddlr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wqdphmwb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hyblvbec.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kvqleqcp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2agbnuaew.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2deglwcii.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2junnrgef.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2owaahixc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qkipkprm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ewrthujb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yzdpzyjp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lanaoyqg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ttlhqawd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oxrdvdzc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xrzbworb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qmhylmwt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2auixhsso.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2eqaqynch.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tbvkpggq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2deztlchw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2olydhjhy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsmlclna.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gqqypttl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2moholmwv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbkzerdg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ujmbqecj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2optxquwy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eudlgfcs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2byftxaiw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ivtjwofm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xzxqdcpo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ddizubpq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kilgvyyr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbikxzwh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2iztlzuza.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2yrhwqkfj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrtdouae.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2bhdsuzio.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mlllruaf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uopwppku.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qlumbevw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jzfomqbe.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ooedbhvw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oxwxewai.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2efxqvtvo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rcaygmct.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2txicpyhy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nizbgpwg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrorqudb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnhbvawi.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tkitewbm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gdqyxqtg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tugqdurq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wpicpvwp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2znqnicyw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kexpzony.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xdpnrxjg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rbgozpbc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gssykdvg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tfjuipji.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldkpohar.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ddtxggxw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mrwlpdgd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2acyklsrm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2lequoscg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kgjirrnb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hfexcrpm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ohoywrbv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ivxwibrx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zgqgnyrf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ubaiqtly.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2cxolfhgd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2cyidxdtq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vfssiuah.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wkhdmdsr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ilcsfdkr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yeqpkswg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2idgoumlj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnqfwsqq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2uafhtagb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vanizrji.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2rtwspgue.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2zztgyvce.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lhdtlkls.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2leboimdj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jtqnxqih.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vqxzcsuf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2sdqymaem.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ewtjgvvp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2usyeuodw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bcwkiwyc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mfetncea.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2npajlbqn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2tjdlyhsd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2arqjxyqv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cyuvqvyw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rnvkskol.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2dwosgadb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yhgvijgd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2asmixwez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuxqftho.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2khxqobbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxdiujcu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mqdddxdw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2afajkxse.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmwprsrx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oczwfryb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2udbbeosj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2oejxkdjh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vwmjzpco.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vdsnfbab.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2icvrdajc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mvevzqjr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2hwbcyszc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rhhzbxet.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ieumozrb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sldqnaeb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ozarjrwd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2oqrlunxd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2iyzgqrtg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gljjrbvu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2oxclveoq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2pvfiorlm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2amwuhctg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qxntwacp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jvajpkhs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tmvpdpnx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lqtelnzd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2rmazhlli.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bekggsvu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2efpnpqmk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2pntwnhqi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hleqoppl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgolrlxf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhxtvbky.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ttbmwcmt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2uralhvdp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2znmgzahb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bfrxmamu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ijxlxwri.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2yzvtbkun.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qwjearyb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ndbnzqoo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pwmltjds.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2susrmcxn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lhaftkyw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ncbljgls.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enklfdut.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fhnzokjr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2wfexucsl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xscxzlym.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ezoilfsi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lmtvgbma.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lnqgvoed.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xmwdffds.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2zdlctete.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pdvmhqrg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2molhmmuf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2rmhmtyns.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rxnyahne.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2skjsunuc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rtckvpty.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2lpjrbbkc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2awmkfqac.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vzzchjvz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kokxodvq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2abmfiqth.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2yqymajeg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xfvsocnt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2dodiqayo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ppqimuuf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wapabjwn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ziurobrt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2eiojgzxt.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2nnghcckg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2pmnptdmn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2pjzzdrsx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2iaprizrg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2aorldsdi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qxwxeesi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vspeeesm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2syprxdcv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2faaypoor.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xbilstwu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2pxrdgpyb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2pdgdthkj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2frhineus.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2sykahyiv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2tewuiwbc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ohocipem.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2bjvoverb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vafywasp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2alruibgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uovyetcb.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hacjixza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkjyziro.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vakwwzzj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndovcsje.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pvcamccq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pmbjgbda.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2apqmhbrv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tkskraet.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojyvasvw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jrkwheca.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dxubfowp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uvlyapfr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lqcmavfn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wrbhibxa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2mremnouy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mxfomuow.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxsuudhd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bgepchtm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjmmjkj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uhglxwsj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2crorfafo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bglwehaa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2okvikzns.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yvwidmsk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tsyczeyh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2qookxpjc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2kwqzyqqj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2dcgdqsot.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2avblvqjc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ntxomqqj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ygykucds.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hhiviuft.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ctlrboyc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2oxvdiqpd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2khzinwli.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pribyyee.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wcysjuli.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sbtbqhxx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2knmklrkt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2pxhshkwu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mdsfvatb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2egzjfgjn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2apvuhvyk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2echvosld.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fapwwvab.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lsbirwdb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2xuqwqyrm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2udklcscu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bivykbbi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2auhmeiqv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2voowlbng.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2isznkrqq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2oonygvqc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2nrtigmka.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2pluwrdvw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ipqaolnc.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2uzdrugzf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2uwzqjmup.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xcujwgdb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2hxonkdxr.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2dngibdqf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2vqlbtltz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ilriwhyo.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ubkvfypf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2eaycatkq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2eszdprql.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ohymfewc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2pkxefyca.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qofxohqn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dcyifkns.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2srtbhfjd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2etewgotf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2exyktjnn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2jiqlvmaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2maqjcpge.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2lfzcjbtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2copatnqa.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2hwrewqbb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2mucpkdms.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lhnrziwg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zmnhbgxe.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xzqxeoom.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xocasfdp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2mhddjndz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ntlctnbe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ybrnbyyw.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hdlnsuaf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2wnoluxkf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2wonttbhy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2eqibdcju.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2fmxgbgup.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2bbkoxqnu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2uiyjafuh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fejcstnk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ecqycvvr.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2oqrqwfae.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ihojiedg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2jytwanwj.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ishbffpd.html


<!-- 参考信息 -->