代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sfgyeakt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsmqmimt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2apirxmxj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2drerfwaw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hmjuwpux.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hylyiywv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2sphkincs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hhoarzwy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ssgxzofw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eyfcyrjk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bonrskmg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2jjneelri.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jdwcgenj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2sxebuqod.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iibdshac.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vbuyixrb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzuityqu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eojwjimn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftqozmau.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rezabwpm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fnivchpb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zrxmgzuk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2owfsgivq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2alkxvanc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cnujyvgj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2owkyltsu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mavpsfst.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmptcequ.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2adkmiifb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2cwjzsmix.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2unzgpsxw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nceqkytu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2gxnkiwdk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uhbygbke.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fxthmhkj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gaxjoehr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nojqdahc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rjhrhfvo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2gvweryeb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kvzracwd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2yhqfzvrb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2adhjrpsv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2olfrdlad.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2idwepoga.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzjlbbpd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxykvjoh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2imuavmrl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2otmrsvsq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2voorpztq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qaavzlsc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xitiblvo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hvicvtmg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvwulnof.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbojdtni.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksenxjhp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2guykcarm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fgkridrl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzfglzin.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dumfkcbm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xxmyekyi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rrbjymxy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2atnnpnpa.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xqgvpfau.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xpjailaq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cbyzjjov.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2kpzfulpq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2uwfriyce.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qtadvmqi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2sygpfrkj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qxarnsgz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2cyyvmehl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nhwnruwq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pclfadmz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tltmveix.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2myxtmsaf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tjbnfqhr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2iilrslwd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mkiwfmou.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uwzkyitx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cttwcpgz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2izmcfnuu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wfsqwxym.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tgjmxwdi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ybjzhumh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wzvhyegr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vidlornb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mpdengku.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mpvnjies.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2golfyloa.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jmolxggv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ybrfsrub.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2kdkjvwdh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wlnnpyhd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2wdxfdbgz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fnoqzghs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkdgaxob.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2fhvpvokc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlqnfdiy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bhwpwlkw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dqyucrus.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bohxebfp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvpbhayu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kmgfcmlo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxizquki.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zmgnfwle.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ybmgbdhs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2lqqejudm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2cxrvfhpr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2lszgcgfq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2acktgxrv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2npygojtu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ebumfgxy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqeyxiae.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ecfcdudp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qyeqqqdp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhpffavf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wmarggnm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rrdqqsup.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oxsmdnff.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gwcjwmyy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ierwzehi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2myrdeoqf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lhijaunq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2pxofcxfr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gdspbkwt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2khpaeeey.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ipvjlcow.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2elouskkf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2thfjhxmg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oerehtuf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxmjhoka.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2slgijkvz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ncjiyswd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2sahfqfrg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2oijmfgnd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xcxcfywf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2swuotuqg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2skxtrjtg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ycbovaem.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvftuklk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mtabsgma.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zcxhiwep.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpzbknjx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zbbycgwk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xvorfpqg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2asbggwlo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jabiyyin.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kjtgtmpr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2bczoexjy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2tswofvjh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xhwprzkg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ukkzajtd.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2cptjdtjf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gosajgms.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2razgivnp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lvahewzb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2htjnglqn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2btjdrcxu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lbthqqap.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2yamkzygw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2prijmian.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2awiqyyoa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2pbkaryaq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wotqxqrv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ryzewmdy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdnkjzi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jowyprtb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xlhvqkss.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2itspdyhr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2mtbsuqyd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mtrjjugm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jmlydfyf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ugczzqwg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jtsbonfc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2yltdyagx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2pspewtxi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2otgsavav.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2fdrghjzy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2eyjzpqhk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qwtgsric.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2gbvexzjf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2julhxwnn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qvsbqfvs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vopejapf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2iropegzz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2dkfgagmv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qgmbhlhl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jkrxhznz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjdbinbn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mnomfcgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxvmmeyy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gdqwbndh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2quwimxwx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ozxartxt.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwxlokwv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwdobnht.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2rnxfzhap.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2huzhgnfc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gljobakf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tyxiwsav.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2iwwgipxl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xsiygrws.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2tveutngn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2bhqdslsw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2otiieqpe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2erkmdkzs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2iafyiwus.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sqghichi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eeclkdes.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2aaumsvrn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzpqijgv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vgdravxk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xdqvwkrr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bmcfqoxk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2razozysu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2cfzbasba.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fofewfsu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2kszboelm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2btyljbmq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2npvaqbdi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2igiqfeeq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vbdxcygo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pohqqngv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2irlnahqc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ivgbxhox.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2xqphcvsm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xdesftlq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rsxqnvkw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2goxyqdld.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cggmbqly.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2grxxrnzp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2itvvyivh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ajqexbso.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fgvvinor.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2sklfkoth.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2dquljdbu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2jnynlasu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dnfuuwie.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2uivaawnj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2bfxnksvk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2bqamjrcq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pvjnwgvc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2iyzaddkt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2jjowlxaa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gmarjroh.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jgtpebyv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2msjevoig.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kbybuizh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2upwxpcol.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2sclabaiy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbzsnrh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2pyfodsdw.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2efwvppht.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2frljlesk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lumbiyhn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2tyjwywst.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2rgswgkhx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2veckxfth.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qxiowkmb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2btusliho.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2xkommurz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2otjbvjxh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hormtbqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvucyhgn.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2cntzvmrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnhzuaot.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ukjjebuc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2touvnvmf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tfvxgxnz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sawfmzeh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bnwkfazy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2lcscdzwc.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2kxacqlug.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2plfopxxi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2tyqzlbwz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mnxxwprc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2izumfwhe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gtvtflbc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2misyruvf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2npclacoi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2caverael.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2hqmispyc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2iysinhan.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2hqcaltcu.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2cgxrmufx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2pouhsvxw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2esnypwij.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2iqnzcxxm.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hltdvgsc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ppjavxwf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2whwuvoun.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2efjllvpw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2qqoeyajj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2tkhhqgcx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ztzxljzy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2fsdbmovt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2llxkehnt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2znxapdlb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vmqcbdlp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kvwutjqy.html


<!-- 参考信息 -->