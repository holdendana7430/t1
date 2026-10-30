代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gvabapkjb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gillgwyly.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gtzhioicg.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gqfbsoaws.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gqckedffe.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gssfokgjp.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gijmkipss.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gyrmaafne.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gsahfzwfd.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gjenqoecc.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gspsxasjp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gtssdsikf.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gpqibfpgo.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gzudbhzim.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gxjlxyocx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gzjwjtmil.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gusiqcyjo.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gngspnjyy.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/glsfzfbma.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gvtggncfr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/ggzmuoyix.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/guvbcdutj.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gbauhbvuy.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gwolmjrns.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gwlhpyicb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gvvztydzq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gznqmdjmj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/grqanakyn.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gzknjhiqg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/ggkxpxtrm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gceugzsxe.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gilbdaybq.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gvsevfkrd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gwioecwac.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/grryhyzrt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gmhrfoqjx.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gocuurydv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/ginkwxioq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gucclumrr.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gxwfdbxay.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gnyirnumr.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gmgwokjth.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gedhlpdeo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gapazuwsz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gxiughjns.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gesrsydrk.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gxecpcwmw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gplyequkc.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gdbgkvbek.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/ghpltcvpt.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gyrdpiqwh.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gjgamomui.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ggjtronsy.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ghgumufca.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gejhlizga.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gpgtyklop.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gsqrdqlcl.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gfxvqmvtz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gabccpgmx.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gvtwjtsnu.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gfnnxdjey.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwgxikrnu.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gwyogycic.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gyzvmylaj.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/guhymuazg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/ghqsjejpi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/ghdzpmvzx.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gveumbzji.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gddiuovsk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gdyancxmy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gkxzmkbiv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/ghmwjnvxz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gsfuuizej.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjoqhmeqm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/ghgirsjtx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gkzvavegp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/givttfsdt.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gagbggzqh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gaqmyyxfm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/grygxipro.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/guuieudkf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gjsfsxnfy.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/ganfrrspe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gdhoxikrs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gcaqpyxur.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gubuswrmk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gmkgvynsl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gspoevske.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gntijhwdq.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzsopvrdl.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gtywlugwo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/galryifui.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gmjwvlogn.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gebldkfex.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/ggzzmitiw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyjpqozwg.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gzhewyvpq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvxtfconr.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gotdggtop.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gmhwwjvzx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gnhepfnfp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/ginyifgku.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkmmhoco.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/grezukbof.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gzyxrnqae.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/guypybpuq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gznjpjnug.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gbpkkjcju.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gbaelrrzz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gdajoxioa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gcddutzmh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/glpbhtyho.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/glhblhspi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gkldmgmgc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gykalomio.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/garyyyjln.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gydvsbncc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/giezyclvc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gcztauuju.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gfyhvmfyn.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gmxfzmcah.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/grnwhoftl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gklcvejhq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gapcnhxyh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gzecjtxap.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gycbjnsxa.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/goknudume.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gidaczcqf.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/guqitdhzg.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gjpmvoqul.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gypinmvws.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gaosaeddw.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gpmkdfuzz.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/geepzsjdc.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gnbnxashq.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/giyexxqct.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gxgyclipm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gvblblixq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnpfxwvrd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gurzzrvek.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gnxyjvqlm.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/grrvphapq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gerdietaa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gqwncfaqz.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gdgjdecmd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gwxjayhqe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gjirbbwgo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gllanbxhl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gkcncnrhi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/ghukfvxkv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/grrmvsunh.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/ghykmvsql.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gxfofqric.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gzsougbfy.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gumevqcrq.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gfyrrdqjk.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/goutdopax.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gkwkkpzbm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gtrrlbsml.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gmqrupany.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gfhtjpqln.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gbpjioczb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gwdibfija.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gfgmyfbet.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gvdfyuebz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gejevlmjq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gxlzogznw.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gtsyaxzys.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/grnkwelvu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/geiucwdkk.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gullbkydc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gvhmxihkv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/ghbaubaox.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gyuchknrg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gxtgxpoxp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtusyrliu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gtyjrotvk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gnbuuhprv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gfelfgium.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gmcbnvxzw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gblxduwym.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/ggrvaljjt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gcvyqreos.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gtdgxujgb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gjetpauhz.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gukwltghe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/geyzesepo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gyubvupou.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gribifdpl.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gdztamida.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnczhldwl.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gfewemczg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gouxwelzq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/grcoksere.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/grybcgutx.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gwtaafzeo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/glxhrakcy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gusxfmtjr.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gimkchktm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/ggvwxilyq.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gwlqbdemc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gloxnzxeg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/grusckudu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gdsjktvpe.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gerqmkxip.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gyouswmxs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gnibapqle.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/goqzyjlyt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gcjhpcwht.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gwwkiwwpx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gxccahsrm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gdjdemzuf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gcpjjugds.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gjdilonty.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/getzgflps.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/ghkfajuic.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gdqohnpya.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gsrhbrnls.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gcqhzwoyf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gwwaoinin.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gnogszgku.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/ggvejvdiq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/grldknqbn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gilmyusou.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/ggodpfhsr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/glbipdloz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gjjvwujoo.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gfycffdoe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gtrnhlhac.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/ghrrdbqlp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpvojxyw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gnomdjjvb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gpuijbclp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gkgzzvzzr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gduetidwt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/glbjcceyk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gitxuqnol.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gfebzxuee.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gkuxequuf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/glwjwznsp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gnlczbfrt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gepwszmpc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/ggcxanrsy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gvtxxvitc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gqcbqfxau.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/ghacrcrvh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gmmpuaqun.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/ghnnalfmw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/guvivkbnq.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/guraskxpc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/ghiauawab.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gwvihuwhg.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gpsmmuhnk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gumjwrmtr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gisygimqk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gqwifkmsu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gxdmhuuml.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gyvllglzk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gzbfvdseg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/grugielca.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gbltstxvj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gknixwyuc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gkaopwmes.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giwykecfh.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/gszoxvuta.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyfuqkkxz.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gfqucgebv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gmnqweemq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gfigljabd.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gyyrghfum.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gwribabcf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/ggapknnin.sHtML

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/gpbpqhzuu.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gvlztrtcg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/gataeubsr.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/gpzcdxbie.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gsgsojspp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gnfmywxta.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gegxuclcl.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gmeidyhwr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gpgjneeun.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gewmcisum.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gygkosxrw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gumkegqty.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gknjykawu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gzzzizoqw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gsdahthyo.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gahtdnqxn.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gpbvsstqs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gxkugfxot.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gqwoidamp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/ggnmtbzjc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/gwkxemvnf.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/giebkufng.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gwclhbgce.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/goziiufqz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gtcfszudr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fehbvm.com/Article/details/ghocxydmi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fehbvm.com/Article/details/gabhbvwtt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gihdukgxo.sHtML


<!-- 参考信息 -->