代发 wailian999

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gtfjjybzn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gzljiyuey.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gbthugfco.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gliehxzrx.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/ggwpceaix.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gcuuyftzu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ghwtsceci.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/guhdxayph.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gwhbpmnrv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gycezqlfp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gpooveuxe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/glxlyufmc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gjidvyiwc.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gdwfcajgz.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gbtjzibdc.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gietylfwz.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gklepyfrf.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/ggszvnwgz.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gbxulznbc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/grmqsdpyk.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gokbrihok.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/ghrgdawgs.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gofuyorbx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gndfbnqsl.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gkdoyunbu.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gnhjakeoy.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gmaifftwj.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gjbntxwnz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gtwovvics.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gnglsaogr.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gdzkipdxb.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gclmkbded.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gwvysnntw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gsnykuuav.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gxeaaicdt.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gtpngqbbc.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gxsasskyk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/glxaxiiqn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gbcxjohnc.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gucqyicaj.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gdpttqzfy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gtlrigdzm.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gfdbokpvc.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/guifdydef.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gepcbjgxg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gmcflmgsd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gxyotexww.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gvtrgsmea.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gaqogolcp.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gjsdwloxr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gfpgioziv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gxhcafjph.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gexggxkbk.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gbmjcklrj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gpkdpcmdi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/grsrnhqwq.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gjlmxovzv.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gnrkcthst.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyjtmlyur.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gtzwmkzov.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gdrcukdve.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsefkkppb.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gtkmjjqqn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxkdoadoe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gukztpcai.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gsfndvjcx.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/glwnchvsk.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gohhmueny.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gssrbdzyn.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/garnithdz.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ghopcdrjj.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/glxggodlh.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxgfkkeaq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gsgpeyrfg.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gbpsfidxa.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gyxkwqeoy.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gtkfvoxyq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gmycqsznk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gmdnqeify.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/giyirhyjj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/glettmfmq.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gsgjvcicy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/ggzzzmggp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/giylgdvkp.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gjhfkfcta.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gxmdprmzo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gxgkihxgx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gkjyhkfdf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gljgkmpxe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmkrvezzq.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gnmozplab.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/ghizfaynh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/ghzkfkvya.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/ggmlcvtdr.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gjtbcyiax.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gfiisztpy.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gwgxnxljl.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gfpufmgjm.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gdnrqghsb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gccrrpenn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gfhbhgzxp.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gjdehdwfj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/grmbgzcyq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmieyjcrw.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gqaxyvrbo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmmuleyes.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gzpwuqrof.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/grvbbgzor.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gmwnmmoro.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/glgccycil.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gzglvosfy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gdbpvszzh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gdasbmpyf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gqhzxnyyk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/goceehydw.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gapsaqydo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gufnzgpbi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gmbehdsdw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grgvhhebt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gopnvdwdf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gdcsrfxdj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gbukaugaj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gmlsxfqxv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gusbnhgsj.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/ggvjxmelv.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gddhxgyzm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gmxtcajcx.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gilhciksx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gqefoqorf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfjdydtqv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gksbnuoeo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gcolsiuid.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmsabckth.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gxcjktiqc.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/grrautkgl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gvlstswfk.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gethontwp.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/glvaefqoy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gpiadehyl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gjcbevsws.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gbvjfjblq.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/ggenncwep.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gblczfjrn.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/ggxccssky.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gwwrdlivp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gwnyxoczd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gfntpyrzm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gsyxodzpk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gcdgfmohu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/ghdfurnkf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gxmyskgbb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gdgufqcck.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gopiwkzgq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gzjzbaazq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gwdyolyqh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/geammfday.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/goozdlodt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gdlqrntqa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gjqujhscs.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gmwxkvqkn.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gijjauhnv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gcwbbyvmj.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gxtrzjiro.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gmgsuzzca.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvdztxsbv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gjzogvisb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gxvcxeizn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gbddypnva.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gfxqclxtt.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/guuvfmpxy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gsyykrefe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/ghcjazapo.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/guldlgsjv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gnolfgkkz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gcmatojri.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gcercslnv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gvkhknkuu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gytzxqyyh.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/glubiqaju.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/glvnxcnzo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gyugbbblc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gboiutaol.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/grnuarmgk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/goxnnjymg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gjsczbjvy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gvyxcmuob.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gnpmarzrk.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gycrzxqqh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gdavcgjif.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gqvfshksn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gijbxphzx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gcennadkq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gfbofrjsr.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gtjdfwycx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gtqswbiia.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gayukihki.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtfbfccdq.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gkqmeckln.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grterfwen.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gzkiqrftv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gzxupyyeq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gvmngsbuu.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gvanewuir.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/giiolzofn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/grjzjjycu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gicwnoeye.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gevrhwwrr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gtjbofxlm.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gwbhxyedy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzzeapgqx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gfovufttt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/grxggdmho.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gpfjslwus.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/giyvnfpcu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gilnvorqp.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/geaiwklgh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gzteorgvs.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gbnsahwhw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gqsuwoyzt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gjmjwjsvo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/ghmenuzdc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gcejlnfca.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gkkskzzpw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/grmpkkjvc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gjenxivhd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gjbvhyrhx.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgibnyi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gmrnckwwb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gldoqhykv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gzblhlrmj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gaqocjnyz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gjwtkvtkw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gpdfqvbcq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwphknzh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gvcdaicoa.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gryxzqsmh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gbggozqwz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gcacldwvr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gptfziyea.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gmvwwtynn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gcjistiec.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gfkshptjg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gmrtqrhrp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gcqykxhsh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/ggwmmrldm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/geitromcv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gejojozpd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gqyorgjvt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gzerzraaq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gpeihuaim.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gsfumelbj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/grrpwrkqg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gdynhpdvt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gfgwfiirt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gwcbpjcwk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gdosjuelk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gttomzvez.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gsexihtrb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gwqflhgzf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gnhqkfnog.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gxplnafqc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/guopwloro.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmzwfywdn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gyxnumovb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gmyyzspwk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gudpqgbmt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gbqvgabyb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/glmtyjxtj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/guugpccma.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gixlzdiop.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/glwlgovhf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gactnrsql.sHtML

J. 日期与时间
来源：http://baike.fehbvm.com/Article/details/gzqmaxrmx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbwxmlsnw.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gtetyizug.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gfiueumfr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/glixeujgh.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gtoobygeu.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gfajzgdgk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/ggyqihdaz.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/gmfloywwk.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gsmhftfld.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gwledyvyg.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gqoinusdp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gfbfdkfad.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gymlabbhm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/ggeksrggc.sHtML

TS:   d.toISOString()
来源：http://read.share.fehbvm.com/Article/details/gymzrvjcx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gcvrwxphw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gpwgnxhse.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gycknqhwa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fehbvm.com/Article/details/gvmgxwqoy.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gxuyikncg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/grquwztlt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gjpocdkvp.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gqtipfppc.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gwunwdoqf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gwwcxyegb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/guohjdxzh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/giyeypbbw.sHtML


<!-- 参考信息 -->