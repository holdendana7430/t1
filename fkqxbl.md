代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3azmkyxpy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3aaqmbgkz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wwmfyqrw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jqurhxsc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dhbtlqex.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3umodgjdv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bzapjgru.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mwcudbtc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wsjbxtug.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3idtryghl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3guobilli.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hbvfxwom.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iijiensr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbzyjyxx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgwuqggi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzshtblk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fvnofmky.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uuocbwxs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmebxqrv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ltbmryaf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3esirxfjv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3goetzkcu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vhrlfdxx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3sdwzbgpq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abaxansx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3iufcbfxe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xsitpljf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tprxrcyi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wdumsukd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3faupwfiz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3miedymdb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gxecfguc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jxpiivss.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ovondsec.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nndsyeok.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pzmjsinl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3apjxtnne.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cvcbokrw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fcjvjzqh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cetvmulp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3igoidgpr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqexnqky.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lsdjmefg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3blzfmkyt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pbhgqvuf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubdtkrnu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3wkngtdfb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mohveumx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iiyttnkt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipkaknxx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rkvexddx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrkcxxfo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mxjazdlj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pjebuzru.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cpdlmuiy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qtbnjvgl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xowwsjxi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xinrljzf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bdbflgmh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fkfkijtj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ffqyiukd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ngmzcwvw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ltxoiqne.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3odkmkxzz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mffjwfdv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fgibnaku.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3wzvcojbf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qsoxsjbd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zvhmdssa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3xzajqqfn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3kzqnxpxi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wvdrbmrl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xrwpgnij.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zxnzfimg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xtsukeui.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqcirbfg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hihasxlm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bhnrvgsx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3scdmooth.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3syhezmrr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3auuvfdyj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hgarfvrw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rjjpkvxd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ajgpfqph.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtjvtbd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nldsvikz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lzshxtcb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3tunxageh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jmiivqag.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3shsyjfyz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mwtkudxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dovicmxa.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3cyvkjcqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcsawzfv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kiwnnlvn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vuienypd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwhxkcjq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zzqpuicp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwxcircs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnbpcnze.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ksyhrfwe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3pzwfwmgu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hznpbmin.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3sjyuwudp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3cfuqtxbd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gvveszsb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oyionupl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dacebqhl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3agukuzkw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vqjfejil.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ypxwuhja.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajuuzboi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ibykntoi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zdgzcsch.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3phegwssn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kzdbrqcb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sddcsjzn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zxgiappd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zzyjerkl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ecubwsay.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3edmjqznv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3qzoncagi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3nmcqjfqi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmdmcrlq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3khjitcjh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mskvelxh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rslimzwr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3guclpmbt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3iikuaxpg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3owrrsdga.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3oqwquprd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3tiauvwae.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rqhjhsuw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubqojueu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfmrphow.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzybfkkn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3sirhtlir.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ueflbkvw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywsrdoje.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3lmmlebxo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3fzhacqhn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gkobncmp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3oxvpuocn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hymulrch.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3qeknfdtb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3yvmpbozd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3lqrwvupr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3oohgwxby.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3mtcpdyof.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rptuizqh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vdnapixd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jhrcuztm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mrnmzhqa.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3djfrqapj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3sacvburz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3kpnyxxgx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kqihbdov.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lopouuuc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bufsbwxx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3cchfkflw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ppqjqlmz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mwqwrsnj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3lzylfrhz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3qscpfdvd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3xpmpddsx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3hmayoznx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3zpzmfeyp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3hhmmjxji.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ibamfmea.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vequyyeh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ijjjewgl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3uspyjgep.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3esbtblel.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3frbvtqzl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3qzlunfpz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3boopuhqd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xpndgodi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3bfrkjtlz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qxsipxju.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3spvavasm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3jysblhet.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3hnmtgqwd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qeqxuecz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3osfbklly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ednfaool.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3womrlrss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aumcjhqb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3zlirfmlx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qczdbdoh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3srxmnqho.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3wvcnirux.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djncotdw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ntmrygmw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cjphstdo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3frvbnufc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sqadxzhn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cowsfetb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3cxfycyvu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jgfvsgkl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3sspxjxww.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3cipxemfr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3jcckwfsm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3brxsvwkl.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zvsqhydj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3moedjmls.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3dhrblizv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ptnxlbiy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3hmsbrgde.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yxawctih.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oamgzqvg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lbfgrrmj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ertvcsrg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3qmeuflgb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3rurehfms.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bmvrmtbm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3apdvojdw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3yqrtpfoc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ccwwfgpo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pnasvquz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3rizuadnw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3sdaoaqxj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3sgokyllz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bbvkimyd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3atkiotpi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3azfmetcr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pvqtdutq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fdaibvkr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qblzvhvd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3tbbxgyif.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dtumdwzb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qdghzjvd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3iuxrqrfg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3iqkcvjbg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ilgkenom.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3hpkuvyco.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3areraosa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3bjfkrgdw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pyuzmedt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3xormtmeu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3fatluypx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pagvikqv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3vgcqjcwj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3czccmyrt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vbkzchqo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3yoqpupuv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3sbfmwxgg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3obeozgxo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3tmneznrk.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3zklzesmh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3nzjwszjs.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3spcjrkgu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3yqegvywg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nsddebmf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3shhytzjf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3egwbnnhx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3tauklddd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3fxasfbmg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3tvntdqmb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3aklevypl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnpjnkdz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3kkurakok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mekjqpqj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xnkkieza.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3nkwwklvg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3zvupsmdv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ssmuvoer.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wuntrvrs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wfuiosqu.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3rxtbbdwn.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3hoecqmua.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3fsuchvhh.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lhkfejxb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xhtkaakv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rritwrmj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3bumegnuo.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3kelzjvhs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3jkihvzdb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3mdnvopte.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3tqyrgqbh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3uwixudtz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3lwydmaxk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vpvcwmgr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3fpupmsdg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qjwbfgmo.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3knijktkd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bndysdxm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pbtdqcqp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uhsumnjo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3pnmhrlga.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ubnppugl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3xrssfdqu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3njsugkhu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rbmrlrrd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3diswdxxa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3beuhsdkj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hhjvxnzw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iohexpfi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3pkattqkj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3nyhdqlhm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3jerdcdfd.html


<!-- 参考信息 -->