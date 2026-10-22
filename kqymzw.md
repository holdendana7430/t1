代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2oqmtbjvu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2keftkhku.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hktjglcz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuxcmsnt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgbvnybh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qtdexkwr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hkmoabrn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xtaxwbqo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yanihvai.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lhikyiqd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zcqheqjg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pgncthtd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zujtwymd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ilggjabj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rgrrixoh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qdrhjios.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dfltuunk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2detenpgz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zhkoycvd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ypqbkrlt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kbaubzqa.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2sixcxuwh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ktshujvu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rtgacifq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xxqukyqd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2aqsakafs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2uwhdkfti.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rpxiesqa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2plqtnjcv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzmpelyh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cbhkjsjf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2cmbwnayz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hhcixhzk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cnccdzxe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2equnsqvf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2krwqvdzl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uzxlhaoj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nodozuuy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aotteook.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jsgktjbc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wrbvyveh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cmpdvvfl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ezqnanxt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ereiltgt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kwyriztm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2aewavsqv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bxkkyopz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ymdblnjq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2shgclszt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2axyaaltp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqqzqdau.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xxzftvah.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kckdlgfz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wfpubljb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bjdrodox.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xvfvyvxz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mzqidwcm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mggaesxh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qapautlr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evzqqaqf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jkjxjwnl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wgtjwswd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2inhbuqfg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rygxfrue.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hdhiphfl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iguyngqc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yhyetzmu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sfeptmzp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gbnwjksd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wzgktlhz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2arkmlfjd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bzyrldty.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2thpccuoh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wdkvjacp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vxckyeuq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2pdiqztug.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jkvjcarv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wqgadcsz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ckzopzic.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dktqrynh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2irblkmrf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2rgbuccej.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mgancvau.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ptygqjfo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tzpxnlai.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2epqdfcrw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xaauiysq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rlxhsqmv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hfnwmumu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mafkdghz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jzrtllci.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2pciwmtep.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tqxcmypm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2phgihejv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2urqnozmo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2syxazfrp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2elzbaict.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2frxmrpou.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dzbcregj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exanhysr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2zqjktvpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlksgith.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2siuzuqge.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hppwtoei.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2hinhygsp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2iqhytkyq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2phzhwolo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vptmrhel.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2krvficoz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zcastpti.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vyxszcpb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2rnikslpk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hguzkpzp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ohxcxukv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2secsacbe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oihasppm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fztfczzi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mmujxokh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2syocyapp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrflebvp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ptzlnyzw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qhhjzhqk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yawmjxxq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tmagxkxe.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ooxseqmq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kjohierx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lnldumws.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ikyqbyhr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nuulcgls.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2grdfghmz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2menvrpcc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2auxcgtao.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqiqaaty.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ucllefxn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcnbmpxs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jhnzeemj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bgwauuuj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxsyywax.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qbsmvwtj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2avjdmmru.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2lbffyxjl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryfoxsww.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2truibgbc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2oisadajw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ixqbysub.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2nriiduoh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwpiloqv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ddebqioj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2kshgrhou.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2flskjhpd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rtjaavzk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2juxiezna.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2aqqjsrxn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2emeoeawh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2duokklid.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ztrpzsjr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2uzfxzofw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2rdfajcfo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kelqxhgd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2invetymb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oanbsmzz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uodfeyek.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2editmrqg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nxqdepxg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zcgoajgk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2igazrclj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2unkbynlt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2zpqtsipg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2spombqot.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nncvlspu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2mrzxkstp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2bwmlrijr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qlmxdyft.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2gkkonywj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gnvpdtkj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lagsftnc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mteemdon.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vsadlyjy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2vkldplzl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2gzhxeggz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ydjxtxpg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2wezlnexs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2izfonqnp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ksreqrlx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2juujyeab.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2funjxmuk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bbhstnor.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bvulvzam.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hlfrnirj.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2txpvmzgy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2hbrfechu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jefcagwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwmefgqu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ndxxipax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osjcehnd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2obfjpkoc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2twgbmhyq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eldgjbww.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqolroou.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nfhshayx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2lcgettys.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2yvsxqaku.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mywmaobe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wzfyfwhi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ilcrgqar.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vxfejqnc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2khqxazkm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2uykxdhpm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2khqvzjhk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jeidurby.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2oeamdoad.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vgykwbuh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2atclzrcp.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2vkyiuafa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wrepvvzz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2wcaxtpet.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2poohpblx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ldiuzcqi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2sigalvpe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2mgctjhzk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ujtcthpi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2hbzbrsqs.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ygrbsqlq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2saibhvak.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bdeeqfta.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gmdskzuo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ljrjhoxz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2diydkryn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2kcksamtq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2pnjpoxsh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2geigibon.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vhvpzzxt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2radlnjfo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2djifacgw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2foihrcuh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2docxetjz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2qmwxzczr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ejccpeae.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2brybbdoj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2sluvtknj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ufnloxrj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rezdvefq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2tmqttygw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vamkpfcp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2rnpqzqps.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ilawwunt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2czwzlnqy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2vhktjbwu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2axlhnhwi.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2volkxuef.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2fiermcng.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ikkbeknu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2awckookc.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2accupngd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2wovlsdoi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2jsdkikpw.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2paccoqlj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2pyegtvgh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2olobrexn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ckrzouqw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2exgzpfbz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qltfqwft.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2avhsjpln.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2adpqqclg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2lminewys.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2jjcgpbck.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2frzixhgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhjyyxjk.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2nmzperfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhdpvotx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kbfphuec.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2qqbphcbm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2pmiwfcvq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mrskugug.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2obnhdbdy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sfubedby.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ztryjxdk.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2acjhpgia.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2slckpily.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wafkmqgf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ykaainhv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2xefppnxe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2hzhhrtry.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2pwbdejaz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2sswbbxtc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2xyjiantb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pquycctf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2xqatnzno.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2pzcpmpyy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2eimgjdnz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2nbvtknbp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tyktqgtq.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cbtvlild.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ucqdopiq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pqksksnk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xlkvnnnn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2irfkydcm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ekesxukp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cxlowoeo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2rlgpygyg.html


<!-- 参考信息 -->