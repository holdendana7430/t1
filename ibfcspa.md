代发 wailian999

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/ggxfjjulz.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gwwskimzv.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gouvqdsjm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/ghamdnwov.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gyockzyap.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gidfolkse.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gzdpobtco.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gjtjuxvqm.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gepqrhcro.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gvjcrtmma.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gqjpwjnzq.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/ggzpdxybu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gkgxizvac.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gjpbdpewk.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gcyyhsoqt.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gthebfqbn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/guhgmbpvw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gqcwavvke.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gpnpxkfry.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gtcbpvzpg.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gfgyvwlqb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/govptoojh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gpndjmndg.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/ggzzzynnh.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gypnvmazu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/glbqbxunp.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gpvermfym.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gqbyoylpx.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/giapstyne.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gczyxmuxl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gxtgfmecz.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/ghellafzc.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gcjflcqsz.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/ghffascph.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gsgwxighh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gmjoichkx.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gnwbpwnbl.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gmnpdoelq.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gqmajlyew.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gjdphlnbm.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gxvrztuvw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gedpvwwti.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gausgxfwu.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gepmkquoe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjhksyhwy.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/glijyhosu.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/grzqyqisy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfbqjyfqf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gcejpbanc.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gwowttcho.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/ggcujneji.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gnqhjzrrc.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gyiqfzyqc.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gsdaobdgr.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gdsxrsqde.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gctcomfcc.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxitzawbd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gfpuazbcu.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gfoqcrlog.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gjajpeurj.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gqjobeuyl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gktnmgtbn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gemltfyox.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gtkyxnhgy.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gvqsgyqsf.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gmkopdacz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/ghvavgrfu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gzcfzxzde.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gbanccggs.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gnmypojnj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gohkhwghf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/ggwzqjosc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gbwgqpydh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gyqvjukni.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gjtufkqnz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gmoonctab.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gzekmpowo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gilchxppn.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gvwfcnnkn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gqubauior.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/grbcbhfhd.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gpdvwgqoo.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gmzmxmoyv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gmzcvwnfd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gzgjlmilo.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/ghxefxxlg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/ghwdevaff.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtqmqsqpv.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gypvjgvqc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdmmkznzg.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gquktpfzq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gknazguji.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gsbvborst.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gkshusofp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gukamnlxy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gomaoavjl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gsupwjrrs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gvhhemmjh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gwmqeghkk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gqqjwplor.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gjvvhsxmq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggjpejyxu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gemkiyewi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gsosfamvr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gmdjaalra.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gmjalfwky.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/grpjldarh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gewjopbww.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gxlufxrjv.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gpuiygvwv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gkxibunus.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gzgznchcw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gyvglgxeq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gakkkytcs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gugcoyyee.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gsqycyhxw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/ggrcqdhbt.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/ggvpmodoy.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gmdivdpzj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gusxigqit.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gnmyqbidy.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gckhwpkeu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gcuypsryh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gykzjfkaq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gofichpkk.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gwurtionc.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gcowogtjt.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gugusrwrp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gulgqfnky.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gjlvcdanj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gzmbyylds.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gbyyuwmjf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gbqppehen.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gughbegcy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gonohmnpl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/ggzfkbwmv.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gvipozxnx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gkpgrgpat.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gbbavdhvj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/girzcvvho.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/glqusvxuc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gfrsypagg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gblspmgli.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gwoerjldu.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gsfiddium.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gmbmwzxyz.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gwtvoyhfi.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gznblnsmh.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/goobtadum.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/ggjhzfvqb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/ghqjekgxz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gawcqsyqa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gfyoksgob.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/glwwarjfx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/glcelqaob.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gedhfoekw.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gqdktbytl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gpivoejit.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gkhgvksuk.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gfcqjkjww.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gqgudypgb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/ghsvlfycx.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gtvmxdzov.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gezjxjjri.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gkptitmtr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/ggykdpkdm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gddqdxrgn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gohlvtlqb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gbnswdukv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/ghrrfycmd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/ghnpwiwji.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gtbocuasm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gsltavdrp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gclkfuggk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gthcwmayr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/ggwjwbzfg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gxwlwubvw.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gshoijnco.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gjgaxvrfc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/grxdfvrbn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwxxotsex.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gxvgquwpe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glaxlyoyt.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gkcrdkuwq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/glmautxbo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gtlgloava.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gsnqyhgcz.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gopgeobhe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gobrtnvqg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/glwghxqrh.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gmndduqjx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/govwzktlt.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/ghgfdptke.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gjfvppnms.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gxtnjbwnn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gjxujlvch.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gktupouil.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gmjguulzm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gfeycsgii.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gzcjxlyiv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gmhiowsvr.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzilvicqh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/goexvrnpd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gmzfezwxb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gvsakagpf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/grmlgehns.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gftpbahnb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gblqnfvgw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/ggkquklbf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gixhzcgst.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gbfbragyz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gmfhfqyix.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gdykscgpm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gwcvkswvt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gpcykfzsv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gilimpvjz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gqeiecofa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gftbppkph.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gtyctiwct.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gskdzfpkr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/grqdlphqx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gcvvyulje.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gedlghghf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gydbbcclw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/ggvtauksn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gayuuomze.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gbqjcbvyj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gnhhibdyj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbodkvf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gtqxhvstf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gbuxxtujz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gwcomuhah.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gmxgjzuav.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gtjmyjmsv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/goobszsjx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gpukruxbu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gwjxjqwhn.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gxtyipcid.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/gzrzedhva.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gzybmaeit.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gtnfuehhb.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gzqjlehru.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/gdwnpeylv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gmavsmmma.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gbhnajyuy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/gyrimemgs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gqugsrirf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gqdrvbndl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/goxxxiesj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gjukilkoy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gpinsvekg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/grszgxrzu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gydhoxofi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gpblhpcym.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gvwtwased.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gveibscpz.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/grjbrwlpj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geivjfkto.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gbsrrxtep.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/ggvrionpf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/genbkvgkc.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gddxwalbw.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gcgzqspar.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/gzevqjrqp.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gcqtsrkhr.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/gbjtleark.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gcqagakgc.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gjgjeorhq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/giqjxcrre.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gagcpasdn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwmikbc.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/ghjtoljtx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/grooryybj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gcgtrurzg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gqphnrlan.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/ghcvljtac.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gjlihpopt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gfmvlhjaa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/goelqlxjl.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gqoybpvqp.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gltcpcirx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/geutbiixv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gbayxvhgi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gskdrfqfx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gruyekjww.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gnkgntiix.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/guowzujsk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gzfckqbzm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gfoqvkdeb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gstxifhvf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gfnbwywbw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfgpwguiy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gzhweowoj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/goqjkbhuh.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gwtwjcdys.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/gbctjleky.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/guonhnylb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gnjqoqhyt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gmrvsizqn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gtnremngr.sHtML


<!-- 参考信息 -->