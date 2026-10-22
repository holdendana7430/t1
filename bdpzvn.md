代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2cnynzhnm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bhkuatob.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2uqjdevmn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hewhbklz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uznairnb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wlpnyiel.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pxkuxlub.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xygzwrzc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vjozriqe.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rddvdknm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qbsfxffv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2sorvfreh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujqxmzwl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sucqfpls.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2agpevxma.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugaswvbe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2grghnguk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2tvigakon.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fxxnmbbk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qlzjqrwv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ffqdcdgx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxhyuuhz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yxrybunx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2oedltkgk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmuuigrx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ghtpkpje.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2prnjsopj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilbhfdph.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xmabqabi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ainxyceo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xefoduuy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2trdqvxde.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2idlbgkii.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tpysabph.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2emsloccl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mwgijdpm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tkuvgndg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2aqvpkbal.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2eiblznvq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okxmtcdr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmhewpwy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfixofws.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2smdfdbit.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mdgyelxq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wpysijnu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddhnsnrv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hoptymij.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pedzuach.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hcuqyivf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ersgusod.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yrovpsro.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xatvqyki.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jufybrrk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nyblrhps.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2btmpkhqi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zeonsrpi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yznvhrys.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2trjslxzk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jdesrbhq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bfoixaiv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ncskrpgq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cccduwkq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2poqjukzn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2datheqng.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2pnbzkovx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tgfcuhwt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2uradioac.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nnwieiog.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qjjnpijf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxfdpwmw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2inlqyimp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2slkkytoj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tkkdgled.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gmafkfno.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2dfxpfxha.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjhawidu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2urtzmnms.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jdkrxjpo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lebzpmlg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ooberxui.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wtyrasrv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2opfmjyee.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gsbyofjf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2svfoeujv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2thbavwmy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pzzuitqu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iwmmqwtj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fjmuvocb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2oobphrsi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2lausacfs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lecblgva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhlrwshj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qygtyqga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvkngmze.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mleyigez.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2livhthqd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rtaqnmju.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lxqqwomx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qaxqdhah.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhjyqdgv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2chwjnluy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fbaswyit.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2orzoqojj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2egcmehzm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2cfzghemo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsqbvrhk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfoyszsx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahrpmxnz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrzznbcv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ltdysvgw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2aapvywsi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bryabsvc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gotadwmn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2jakhhwum.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ewsuaqrn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2atxhqhwj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tuhmldfp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gelovxfd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2hsvwjmfc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bkxnbdwl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2isimguyq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ftnpzbto.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hcuucvlw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2elzuktud.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2krphueug.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzutakki.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijkckamx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vbbemfom.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2swegmwbp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2irncfakb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2lchoqhef.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xububnhh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2dyecmqaq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzweyzwi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftlebtrb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2anxsmhri.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ilxiiumn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zidsvjev.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2gmsssosq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tjduvlmx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dzsmctlq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ncgdrrsx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nbhjhrci.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xzzpkijm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rvzlufhs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2epzfvnoc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dszlvyif.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bitgzqyf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2orexmrbk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fzzphfvj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fijlcwss.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qleazkmw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hyguvpzu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vlajvnid.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2iznzquey.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2vcxfkczg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vuluygpy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2fvjnwbls.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wrhlyvnr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2pfqlrkxv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2mkyjcnbq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wsjiabfp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2rtsdhmwe.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vvwrrjix.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jadhjeuo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2mluavujt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2wwdoyqbn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2siuybsjy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vwsqnvrr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2laiylhac.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rpoiuydq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ohiwlzlw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2rnxjilnb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qrskicaf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2uliqsndp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2izdrgmdj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2lwhdooxn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2lhqmhrgm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hzqxmpmp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zmbdovti.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2rhvgmurf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2gwkcrvhp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2kboawfce.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eblfdktb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqiuxrcu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ginpntrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntqfphwa.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2yvzurnkn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nydkzxyk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cnukywfg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xndjehnm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bapdixez.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ryoticje.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tsjniowk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2niuhzeeh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2obajeyqv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qprluxpd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dchmpuxw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ktengpan.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2jqscyzzq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2jeykincb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aydwgyba.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcrendjd.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pzcyybar.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fayhxgpe.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2evjrhmal.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2kmtgtpcy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2exclzjef.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2smlwhzdo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2spoqogei.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ugarowrw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2kjwnbwyo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ujjizpbh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2doccsaaq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ipchoveg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofhatdpq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qffmekma.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fmuhyuqo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qghlbvwx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ugjkutle.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2cpykbpon.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2upzbheqf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wouedcud.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cksxfmrc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2moybzmfg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jwplnpmg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qvclkphj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cfetltzc.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2tapjaxan.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dehxwvzt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kltwvyxz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2osfspmsn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2pkjddxvf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gsnczfab.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2jegvqbmi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2hujhnrwg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2oxbmdotu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jnsapheg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2nzhpanxn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2xdaauuwp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jdhnfajm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2jxihkkpo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2redopkhl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2roahoxxg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2uvhofxnm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2kfgaukox.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2ayvmjczb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2tomupsre.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2csfsadpe.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2scyixgbd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2whlejzsm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2msrxnygy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2hkfycmzk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2volxvcqa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vxtcalfw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bihismxb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2jrkbsksp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2mosbruzh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ibzbkzdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxaddhti.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2bldvnvdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2najbtcwt.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ojebxojx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2obbgdmon.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qguvvtrh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2pkphgkqy.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2yamecccl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2yvlxehyl.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2cjjpdpik.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2xkakklzc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2apbwryhz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nfortnbm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xrmzljjr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vnmycysm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2yaalgpel.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2zgfuahra.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2kqvxppem.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2cfsptvli.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2tyvbnedv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2hrtqjczw.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2lzrgunik.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2heltptcp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2bfzdsqxa.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qzqmjsqy.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ueiacqhe.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nmsiohmp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wmkqdoon.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2anfikfnj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2cskapxzf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2djbmssjm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2unluwdqy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2pwhfgjnd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hfcolncw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jgpnfmvv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2okpucjjt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2zkejfisd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zognybmt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zzwttuve.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ebrnludv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2dtboumuy.html


<!-- 参考信息 -->