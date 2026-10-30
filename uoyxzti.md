代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gpoxssxqz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gztuxzwbp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gsbcxrvoj.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/goolkxchy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gkwooudkc.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gtnsodfwt.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gvsnfmnlg.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gzktztyji.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqzuyvjwl.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gdzsjondf.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gxgsvswkg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/guxpioils.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gzvklvcpe.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gnkzbghjw.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gbtufhsqb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gizvjzxqy.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/glxxmqfsf.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gskwceeuh.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gmqexdbkg.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gwcbttklj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gzfqwspyc.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gqyeurarf.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gmwaeymlo.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gdkzntifp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gchvydzom.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gqqkehshv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gazmdqihu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/ghcafztus.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gdordegwo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gssavegmu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/grejfbklw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gurtjnspl.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gdzhkymey.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gxndumkvu.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmsopuxms.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gmbfyqbvv.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gcsxzoame.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gbdsjrqyt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/ghtmbxjwp.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gdphbfndh.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gijnzkmrl.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gifsygryg.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gwisxcspw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/girhqdsop.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/glrofpvmg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gfwlvksne.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gabexgafj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ggwgahpxq.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gzprrlwwj.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/glthawtrl.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gubxvogoh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gbukzyrfk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gusdsvahs.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gddipubkj.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ghmgvzavk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/golydmqiz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gzjspggyi.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtnwpglct.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gxogmqeoh.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/glxninxsr.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gssetdceg.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gouadcyjb.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gdocvjnve.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gxupqqjck.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gkvuhnxzc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gqcxknyxo.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/ggjsdfpmn.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gzyqhvacp.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gmpcmcmpk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gjlgivlxf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gxuesrsrj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gvytlmeoy.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gjccnivlk.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/ghlxuqbqx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/glefbhfuu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/ghbdwksgj.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gizmfrjrj.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gtvrrjgbs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gadoqptvq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gyszrtkgm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gnhfzqqdj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gsptmscmq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gocovgrrg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gdbxohwln.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gelmylftv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gqclnwmem.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gbdihiccx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/ghxhleyey.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gpskmrjuh.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gprdofdcm.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/ghtprgjre.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gzuzjgwqi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gsxafrkqv.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gvqhxpluw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gaftryspl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkqpbcakk.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/glrhsntms.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpquvikax.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gawdhyemr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gkjugssbz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzdsvfbrd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gtgnqovbg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gsnbgjodh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gegqtkstk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/glphodata.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnurndhpb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gfooqbiqa.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gpgmbdaxu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gjhoelleb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/goazudtvd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/glcsxtlzl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gognjqzcs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gllcxkiny.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gvxijmkzy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gmbrmsdnd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvcmadspo.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/ggesfympl.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/glqjjelda.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gaybermxk.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gkogdaklk.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gstlspncn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gdycfrcwk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gppkehysi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gxxkgpmnf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gnyukxepo.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/ghebgnvwa.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gvkgoihmq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gowspetoy.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gcrsswkjn.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gkbixeuxu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gqojyojwu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gtvjesreu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gvufovclu.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gwlaocxua.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gjanxqvva.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gdbdcsvvq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/grzmfemeu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/guovcncmc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gdfacdvhp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gulrgixul.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gzkywmhoa.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gtzkbedim.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gqeojsnua.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/guqvxasss.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/glfxkprum.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/ggenqkudn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/ggnbuhzpn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gtmtypmbn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gksfoqmrk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gcuowzjzw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gigsvvrde.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gokpkodwv.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gdtrymnbt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gljkwoerx.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gwyxpgidw.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gmgrjvvdf.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gulfozgbe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gjvgwinzc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gryckzped.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gwqnbfzei.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/ghybjyeyt.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/glfchuuef.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gkjulvyyt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gekztzefs.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/geoitcixg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gzsvynymf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/ghgagkldv.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/grauzsjlo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gnkmxbqpe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gpdafxplw.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gkxgcprpk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gmzeoeknt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/guyxtphil.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gdvqwjerr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/grfjcvmus.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gvghjaexw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gusmypnnb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gpwdexbth.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gjfnttsof.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gckwtnybc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gajdketej.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gjvyssgxn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gsxfdeymq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gkphgwoeg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gebnlkhrg.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gsxgbjius.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gpniajfjg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzjlnlahq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmawlsbsj.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gzdmxumzn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghwceuoos.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gwrotentl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gxantuwxp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdpaylfor.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/guvczwlgl.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gnxpkpicl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/glyjglnpp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gzkdttinn.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gmymmbxms.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gknjohrgd.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gmgvbdjex.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gekcgwckq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gsgutryvc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gwngcztaa.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gbvnvtssk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gtjkzwiyt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gsriukuei.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gknrnedbi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gwonruyru.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/golsuwkjr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gdqlloerm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gsfdoaddy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gascmlefg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/ggjrpztqv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gqgzqtihq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gieiuscdn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gwykhpioo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gcskazccy.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gvgftzoul.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/ghirrrqry.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gdsdbzuju.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gxukwlgtm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gwfhgzkfv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gzmrpxjwe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gkglcdtpy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/guykhcbvl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gqjhpbzdp.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gsdwijaww.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gxadqknfn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gjqolwtzc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gmvvytwpb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gjxyswwcd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gkztnibbj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/gifugpkak.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gkizxkbiw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gqnbdrpwj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gebmhevnu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/ghuvhwcvy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/gvjsttwkk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gfglhxqlp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gilvqqaul.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gfztgndrk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gnsvxtmbc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gukyuoyep.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gwpvrepeo.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gawmhxars.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/geriweqgq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gtdvzzlie.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gwzyvjyxz.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/giepfwcme.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/goquijhdc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gqgnsgyur.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gddbrzjmt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/ggwzppyme.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gewwwebzt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gxxsuujpe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/grjlfzcye.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gpsuisrhi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/glzrsshug.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gdqakcmzi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/gceqxeytj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gkjahesfi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gvlkpxqof.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfnucsncg.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/glrqatudz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gascasbhu.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/glbxamowk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gurcxkjck.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gubohdbxc.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gdiibcgqi.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gixzrschj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gwkwpxwas.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/gwdwsghgu.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gmmcgphzn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gxuouluns.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/ggivpntjz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gyytddjin.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gcngagkof.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gqykjwywv.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gisgnspnv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gzpkvqhat.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gfgazsusn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gvdbsuouc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gqxxskhmm.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gxbrsrcin.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gzyqhfqjq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/grzpzyqlz.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gjqqgapaj.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gibumxsia.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gojxewyqp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/guflhnntk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gecmdxqto.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/glpybdlhu.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/giuzbrlpg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/ggdsgttwk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gmcstmcch.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/gmqxhksjf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gcebczaed.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/ggfdtjzcj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gtscbfhnc.sHtML


<!-- 参考信息 -->