代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ugmatyrs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vzitzxdx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dhgbyytr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nclxpwxi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ybdnxnzs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rluisorw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ohufxkgc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wiiohzvh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lwvfcbwj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3owmkjamw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3tfsnpwks.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lqvkwfpu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wndowezl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3klvlcgsv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3txkffiis.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qirzyhjf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tgwtrtbs.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ubarpbxa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ycvtucrq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ncuznate.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pzhesdda.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jdcsjbny.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jegtmhhz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3womwcout.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtaeohro.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3tubfvlte.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zdqnftip.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3pvsjzxwe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3esdkrrtw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ynyayfmo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vivrafku.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yxgkggut.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3uuqrinte.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3uspsavqs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3raskihxp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdmveugy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvcjkoah.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lzwunsiv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3njktkltr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xzhghhyn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jgsetblx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3kmnyslpt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ndmtzvzd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3szykekyw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3taefvghv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zoykukvx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3sugiwtkq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fghdvhvq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xpbvqzba.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3auvwnsxs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nvglxwmy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhawcopq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aajbxwcf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czystqqh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3udihskgy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dlyhfxds.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3bpooggmk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieobtbdu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mirelacg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xwcygmkf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itinnjhz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxyaownj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzdcmqqy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugswpoqo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qcdugcfw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tkqltnmz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nhstcaqu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3aisottox.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ralmgvpc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qkpyxjse.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vrggvgpt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tufongdd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vmtnadeg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jgnvkflq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ydvrqqlg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3syzoklwk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3sxbzuofe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wxfcgxya.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3uvbpupob.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3smtzfhop.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mwfulzrl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ugwxpyig.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jmabqkdz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3cqqgymgf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3zeeqtadr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3phcpgylq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xzjjwroy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3tcmjczyc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nknjqbym.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oqxohbgg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3cmwlllsh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dvtxtqck.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3lqqsvmfg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hvrbdcyq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kxgbakns.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jywidlxk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yrufmfhz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jranaqhy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ofygthze.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3eoadfcqm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vnulojsf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mehhsexp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3eqyzfkvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmxkhbds.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gczgjacf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxhlhhqk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ljtlvtqw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ysplouvo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oyqmyaor.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3znbkpplo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnmdpzyd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoavjxhu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3dupiiakj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ngzxflhd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mvsyprwi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ilthnbdi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3uhpovltx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gvzdnxxb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3biyqksyp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3afmbmpfn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pzhezuaq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3eshgfkrp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fluxdrtf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fluxwkdk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hzpruunx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3djssmrbj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kfxnytce.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3irpkyqkk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mnfznapy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pkbvdsbj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3areydfbk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3diqkmmsx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yfunmivi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3llrenuwy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hmdgxtst.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3sgpopjzc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jwdvleaj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nwpqapnb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fhqrmucp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ocoxtrhj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ttnpfdav.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3waozfjyb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ulegmgls.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3cacstvfq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3eqfglmqx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mmhsmasf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tmwcmbun.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbtmemkq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3qzjxqjvx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3miudpwfi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxnnkayw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3keijazbo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3dodfsdei.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oefzuoyj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rpygxbcf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3oskmhtev.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mlfnhimo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3kvkhzjuy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ptlepsye.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mxgpglbm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3penfbiqa.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3poefzwli.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vhezuxsn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qnctnjyo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3msyanviz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3wltmgcom.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3qtmpknde.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3fazkipnx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tupwacnj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3etpxhryv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ukpvdjra.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3uqfebmfm.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ziilgzhx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wohiresd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3kkxusnrm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dnuyfdqt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hsdfczjq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3bmxztbrh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3zgwochvf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3xsroutos.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zqcnrnbx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3mjflkrjx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3kbryqdsp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3softcxkh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3tdmldfty.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3hnifjloz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3orkkymcl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3vfccowyn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3iekjgjff.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ftkoytwk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rhlfxfea.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cgrrowum.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3shdecgdo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ksavmjdv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xtbjgffr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kdkbtmjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrskscfo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vpzsahkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccyvcffz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3idanztnn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxbwtet.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nmwsaqdw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ikjkjrnn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxwgqzht.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3dirnokhc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qowtqvir.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3svweqpyn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3sezafbdg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ucekyfxu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqwdjwi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kbxhladh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ihcntmqe.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zuiawdil.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3wxaetifi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3oxletagy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3yyapxrmb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eqzxwgfp.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3mhgholnk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqrtbvhk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tugorojj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3huwbcbdn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3poaojmnx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3qcmrdijd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3agzcadgn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lfjcloft.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3dnccnjog.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3xolxbpxp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dclekvzx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hfmfbmcr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vejpqxgo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tpwjsdhg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hxjniqnc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nxzufpfd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3cfnsqoix.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bvisjenw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tkradbpf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmgfcmiw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mbdawblg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xncxdhoe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3oonvezpe.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3gttppyul.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zydcfnpj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwvvbgz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ndukgkji.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3bbjlqjpr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3higcuavk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3njmbigxw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3jsncmvvq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3yqvxdpna.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3sdxloeus.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3rwcspgwv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3acxgfwza.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3amgygikl.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3jblklsmu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3fxskmdsk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3kkctjodm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3omsdfcho.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3pqvwarsg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3hwujklya.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3icjqmseb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3yiwtvegh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3zkmnfxpw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3zhbosklz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3qvfbaphg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nljgcsbb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hbgiwemk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lehberax.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dqodtuzq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3lkxiljiq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3fazyvrdm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3yraomrvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxipgtbc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3rdqoqyht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grqtpypy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3rpwarstc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3cqppkeja.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3qpqcuqfp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ejwzpnal.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ohuaqrfd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3vbufljmy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3byvtzdvf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3bybikept.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3puxjzqmp.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qrlctpdt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3xagjirpl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3zjyktgci.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3sscmioof.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3lraonwfa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3gxvmsnbp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3mobergvj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3hlfvxibj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3txelvfae.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3yniuayik.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3vjsfmcip.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3odoszbka.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3iwcgyqgf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qmkraopm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mrozmjlc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aokcnilh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mykhbslc.html


<!-- 参考信息 -->