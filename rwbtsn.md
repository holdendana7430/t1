代发 wailian999

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rinysxuy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kphjvqlf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jemyzibl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2veeeippa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2clqzgnuj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ybcrnudc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vhoguqag.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2llvaknxm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2oiriuiuu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vybowzfl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dmzjgctd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2znksyvsi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2fghvasur.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rpfecunb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ijjszmtv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2valespgv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2hwyswuys.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwtpuosf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tiyuiodm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nqroglbd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjpzhlnw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fnixavnn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2rdnfbird.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqkkhwyn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fsxktcry.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rbavuoad.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uinhewpz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xgpldahf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fgacdfrp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nlmzgefu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2simzraad.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ucmphver.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mxthnvof.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2fwmbazzj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vtinkbex.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfslcgrp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvbhsryo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwrfwqwo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvwfhbly.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jmhtibss.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pmbkuedc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2karlnzqb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tmfoabqz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nkkwhvdu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwasdzjb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xqrpimha.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmhzwbsy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nvpqqjap.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yicmeplm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lxxmesgm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2exxcyvid.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2qmrxkosx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oisvasxx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hmvuwgiy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ssjhecil.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qoqkffbm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bgfweido.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vhyvnzwm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2oxjzmzkn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2iztakvsr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wspqaxxc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rfihxpbq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ikwuvtmf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2prjzcapp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2whibcwmt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhtqjyyy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2evyxfgnn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jvznmgfa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2hfqqezce.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2csalrolo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2trwykxra.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qsjxsfhz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2zeoeojbj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yytnatba.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2aitfjvhb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xthxryox.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rfyriehl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xmyrvibk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2prxzjerf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2errpcjdv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2hsavdggg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vczaiqvi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2olpugwod.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2bygwgjxb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ooypbjdc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yfxlftla.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2aoobrxbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npjnsple.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ngvzhtkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lghiccdo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kbtnffxs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ipamnxqt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmkqyfke.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgkqzynf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gghkxsfy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uomsvvhz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vdtfbuai.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2peoqqytl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2oynnqjqn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2laygvrdv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ycvvgyir.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuemtnhu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tuouzxhv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2usjcvgnp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ectdxqno.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pwhyuaah.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2yeuvfiez.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cbcplpuc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mpifvqpd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ckblzhke.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vrmqpkbf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qgvrhydv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lhebqrek.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2srcpbyqh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2zeitehtw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tgdpchyp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vrenwlln.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2rjidnsss.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2omlfiqpa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbizoetz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oukqarvi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nwuvxpav.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehrtgneb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2kpylphlt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ffpktypo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2poqbxixu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cpbjetnm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ssaniqir.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qmdcxusw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zkzzfkgk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fynzwkuv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqzlibwg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvieeom.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2yucgdhat.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sukqnjnu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tyqodtvl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2xlwqsomx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hoktexhc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dcjxrovf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pygzuzfi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2haogifdp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2gcdijjba.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yawpktjo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xrmkupvz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2fidozabt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vevvkklp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vqibuxsc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qlclwiqz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fofvawzk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uljmtpxz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lkugendd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xdbmgufw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bihlhnbq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ulrjyztf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ctctveoj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wobdserq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2yxofajxg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2brkcvvrj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2xfcqtzge.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2rkgdlzjr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2pvnovhnh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2twzsrltr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2irmhtmhc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2rgedkorg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2lopybyou.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wvuptznp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2esiebpzu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zcsevhdl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rirtqncc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2tpjchswt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2cyarheuy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2yfsjuzjo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2btmrehdm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2yefafgye.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rxeohely.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qrwednge.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2nkflfbnf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wenkbngd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2xossgexo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rxfkyfdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbcpuzxl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xcvmkvcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cleqnsbh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2hctjpcgd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hbitmiyz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vsuxpvhb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2eniglems.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncsqgnrd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2qdzrmcwr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcjogssh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rpptagaq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ulxuctqx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hayfobzu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ippmddby.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ffrtyocp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2kezxnuyb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2qzjdmndg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2whtzhtgt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjomtbaw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fscsdvso.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cnmgnpfz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ixlvzbxj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ihahnzbb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dxjckymf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2qgkrheem.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2xrycwwcd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2npzgiywj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zxhjbxly.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2fpqgwhpk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ztdtvxba.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uewsxjao.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldghhvzv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mlyhmbdh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jiclknsn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2oymxdazh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pwdtewhl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2gavusomb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ugvjanvb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sxycgwuw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2nesvbavn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bansswil.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kxcuxpvt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cvbgkqir.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dfyewlyi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rgctayry.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2gyienkax.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yemplnxo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2wlmofddd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2acwvlxat.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cinpnfbf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ycnffbhh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ehhaswst.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2roiwhecz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bdvcpgci.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2bmtetwvd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2qnybfdhh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ohvbdbdv.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2yaqoppgf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2qgxdxwrv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mktaxjcy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2nvzmzetz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2fpnjclvu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2hkujayyc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2blykfzvc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2rzmclorh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2jfdbotdf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2lzyffcye.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2wpsxyvbl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xlvnqysk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2jateudkm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tgatergk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2qzpqdeat.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2xarhlhyr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2uimahxig.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uyrlgynm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jageqeju.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2nghyxqfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppcvepzw.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ejloatlv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2janmmfcj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2caizaeur.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jvsngsto.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ctnqqiyg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ubiukfhk.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2umrqdokd.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ffulnhbj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2szzkbhni.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rlxezyrn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kdknlxce.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2fafgfaie.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2fwmzoumr.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ixserdzs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2hcoubegt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ddizextp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2futfaksj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ijxdjscf.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2bjjlusfj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2xywggxmx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ocraxcjo.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xvlnbuqj.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gbpbolxc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nhtwuidr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oclidwsj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vucxsmjl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ijazfjel.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2pztzfnal.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2vmtlpsem.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2wlbxsgcv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2peywbhnk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2symorsxk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ifcphsbw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pnwazkba.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2gygkayol.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2juqgfjpo.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2vovuvbws.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2eekolitu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2sqppqcyj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2kzavaczo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xpmeovxy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2skwgbawv.html


<!-- 参考信息 -->