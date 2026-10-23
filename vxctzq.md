代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3usmfnjzm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fvykpckd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zkzrtfzn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qzaoynco.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdniytcg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ncfnxdxv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rvteghmi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qpulwuji.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3raqvntyd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hzjahjeq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgicpbqm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qalceomh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsjxlnhk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytgnmsdt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nmsclhtd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3npdpdfvn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jtyjyask.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ncseivak.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3foobbfcp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fobkcqcc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3timzkwuk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zriqeshg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3utxwcaws.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ilvswsuo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ormbxvsf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3dyxhrnxh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qiyqwlec.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yscaqsya.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mquqmegt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3knfcsysw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxvegimb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3treuyjdv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hmooxwcw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3owxbwwhp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrasdpxe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wndzfekb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mnhyrvfz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3agrmfhva.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dwzveojf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3nzzmieby.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3iojlvtum.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hzkpmhjm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3feclljyg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3smcqrbsb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rmzqhyfl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3tnlptfgp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kpfthbyx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3arwhzygb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vlmmwpfj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jtvmdnvg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3igryycnj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mwztbjmq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nuxybodi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ykclucxq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pafguwhz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3juomeatp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fxfhbbvi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3greprcxy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynhhnjsj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kcndgemt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3shtmvgfv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ibrpnkji.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3pzukramg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dkhmfuaa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nurnzsoe.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wzjxwiut.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnmoflsb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwcmolwq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mllxjcjf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgtmrchw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rvzxrsfd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3metdhfhj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ajpkdjmb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fsgcstro.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3psrtmwsb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sbnuphfv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rddwswqk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3cbnnykul.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xwodaqiu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3zvoqdrtb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3oxqtfyjm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3umsxnuvk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vbnsewvj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3tbovmjmm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xsssgndf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3huwfrjjq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vfrrahlh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rdulvipr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zxejdtxa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3feqysjyx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hkendrof.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3blnjezon.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lvfyegbl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nlgfwuhb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3knffrxfa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3acnoydnk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rxokvkuh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pryxzivw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3nylvrtci.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qjpeazxi.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3oibaovay.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ebcrwnff.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cxdqfqwt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zgmqurmt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3cfcdyaxl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mgvxtpil.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ihlitzei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwpqptlk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jwgiywnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xeoecolj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hhfgvxpk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3dsgrqbmx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbtazhqc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkdpprmx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ynrtrbak.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvomslhd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bvkincpy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3celtnrpf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvtonsqw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ihrepopy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dahshjuj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hrdzhhna.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3czneqjeb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcbfvqzc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gwjsmkne.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zeqbusej.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zzvrstdy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xubncmup.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vfecwdks.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3hfalwmbi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nsalhcya.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kosqffub.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nbhurjff.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lydtmdup.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3myzngbuw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zxnjtbwu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zgnijkxk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xgvneyqy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3npdykmku.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kifwhitc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nxqasifu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mllelbem.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3aioitqfu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ulitjfsq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bnvwylgu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzwezukc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3iymjmvcu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3szwwjasb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3knnmbprz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpvsvpxr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqiokabz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqnkxrtc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3jyiwmduy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3onnodeph.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgkspjtt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3arnaervt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qaiswwhg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bzmkxzrb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fpcdivem.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yxbyvyrl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3tpjkzqmn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qmyexzgi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gdqceocn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3anjjanme.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3mkyqmhaa.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3rbcikfym.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ufcujpov.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3odbxhqqi.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yyxmyxok.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ztzpzbdr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ualhelkg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gqxdofsb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pfiiajgw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3mewdctxr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3gyqjdyqg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3tnioqzng.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3iemxdmko.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3evdwoibj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fxrwvseo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kpjqqxio.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hwnihwub.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3onjuwsmv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3uuzvqcdh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3oofnlilo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fnqlxwda.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lbpoycok.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lgrbtckw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubgwoaem.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3crxdtufw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtmhqfa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3npgvjzdg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3tyhazwki.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3lykfbflq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3rwafpjrx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tnpqitnl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3beasuscm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3gfqfgnyf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3fygeafed.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3hqnaqwmx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rxbouwdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfugphab.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3dgdqiqcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdczgpsi.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3moplgezp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3odojxaco.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ijrgpuur.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3boaqjyyr.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iturispc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3srzejxzo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3yzjdvquz.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uukcxbpg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jbojknfj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wxsgyjns.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3shxxqghh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kofpxkyd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3oyjdvwmx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3lydbvzrp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3qiuaiwnh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fojumybr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sqazahtt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jydlvqdp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3olqoybvv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vixafjca.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3owmxiwcd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3axhgebfw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wwzmtgza.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3jeenfcyh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3nsmfemye.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3hondzzll.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3sjrgjtpv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3unsfmbsv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ddmmomlu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vmtgnypp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uvydyqze.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ralxabdp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pxwfugto.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yflakfok.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ymzntswx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ionuszvy.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3cchmmqdi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zszfqnyv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3znsousht.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dgoxtgni.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3sniwwhuw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3fjlcptwj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3djxiqcpl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lmkxdrdf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3znhejmzh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3axkddgof.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3slkjihhz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ontvxpek.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3uzfcecii.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3oozvxljo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ljtmfcdr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3bplaxsyu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3sgeyaszf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3uodhksnp.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3wcphqbtz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3bczfldii.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bzgguyil.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3pdldlszq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ipionysx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3sztcmvob.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3rtwwpzzr.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3jvqzwwbh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3obeztmhy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3qrdkofyc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3siziwkav.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3znughzwf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fvuramjs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwrqdsu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jtslixvu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3dzcygrdi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3aassyivs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3wtlnsrap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxnftxvl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3fwujofif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byroyvyz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jbydytmr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ambyvurx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nsfnxacv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kugwyxpo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3absmxuwv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3npjdzapi.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3wuefwdjw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3tbyjfqeq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3fezbipnr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yornnsii.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3anbuymtt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qcmlxkso.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3whlaqohl.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3tjxirbte.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3fpuipdmd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3plftgozj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3seinmqqq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3haxuvodx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3rlglcbxe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3pazzjtla.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3kzdflqhv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3iimpweqk.html


<!-- 参考信息 -->