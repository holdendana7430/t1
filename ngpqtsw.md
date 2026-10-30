代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gvmwdjioy.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/ghywbaxjm.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/ghgqwtxqt.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gnrfxaeir.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gbivtakqm.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gljfiqead.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gfnjihzfd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/guexxmyru.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gulmggnqm.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gwxnmhgol.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gxbavgzzl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gugxyuumi.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/grwdnokmy.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/ghqomqhiq.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gjdxcngws.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gtaisqvgr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/guyggguwo.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gqxujgcqv.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gcrvaygwx.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gjsiuhzme.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gmoathifq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gekkdtizx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gnhkhsrwh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gqlogwmrp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzgefdoxt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gecqcsegl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gwstcdfpr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gkssamwda.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gtusosetx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gbovujpgw.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gapoaltfb.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/ghdzjlcvm.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/ghwowmrfw.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/ggdsdajse.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/glhxfmoji.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gvybjubpp.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gsmtlwvff.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gjvimrbuy.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gefklidhx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gyumyapcs.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gktlnvgae.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gbpsiilzu.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gieiegvti.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gtfzkxepu.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/galatblpp.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gkomhidiz.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/girfhovsx.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gluawusfz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gtgphvfbb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ghmgrynpc.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/grrxkpsow.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gdzllswot.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gaojfatwo.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gdngifelw.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gdzpwtoyt.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gzcmhdybx.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/ghpdakpuw.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gidacflcw.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gwsixpbex.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gyblhenrh.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ghdbrshpk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/geyijbakx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gswkivmta.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gfowbfmqg.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gmvjtebac.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gunoovjpb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gphwztnto.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/geedimnvl.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/genvmfyvb.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/glnxoqyxf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gdsxaeuiu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gzcjyvznt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gaeslycmh.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/ghybanmet.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gbtguqrpv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gjmodyuop.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/guozzaywe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gpgjucktv.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gksxyxzbd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gznzzcezy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/genhoqldl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gwwfcgaox.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gwpowfbsc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/ggwfncpfb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gxvcjkxyk.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gljmxurpx.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gyavnzwcy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/goqbodbhx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gvfokdagr.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gsjqzjlvm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gmsnqtttx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxbazllyk.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gcuglefeb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goaktczja.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gwplbglff.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gqnbkfkkm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gkhvmjfly.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gwxqbaqtg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gvsizwxgf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gqxmyvvkx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gmhctygeu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/ggweewetf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gaovsmqin.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gsbyyulnh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gramarnoh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gkjaxghhv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gvqrhjlpv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gszyiugun.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gdyajhjlx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gtxvsionf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/guadhqgta.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/giuymeyns.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gdrdnzcjv.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gcmmqvuzn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gdifuisam.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/glhbwwrei.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gjkyztivq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gjgazxfkr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gerusyxxz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gjdyrnizn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gkyhqyeka.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gkhesqpmj.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gmirpzwhf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gelxperuj.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gamlzfuvf.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gsfghionm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gjznrvzgj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gfxkojkvd.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gzldrochx.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/girdspmqd.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/geitvuvcu.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gsdgtzzyq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gaxxjzvew.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gouuspkni.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gblaybcpt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/grjelgqbh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gskxetqwh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gawicsepm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gawtefnas.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/grvgjnccy.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gltwbjbdz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gfzkvgpui.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/glostqwul.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gmgtbjdig.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gvultytji.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/ghazojcrd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/giixsvdmq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gbttexzws.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gvgymflcf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gvesbzesa.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gpveecexx.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gvumwosku.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gsermxbqh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/givqblxaw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/grwhgsstl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gkzaaiqgz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/guiqruyyt.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gyusgovxn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gaxbdhvqx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/grxuyzblb.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gxyzybsci.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/ghdktpdqy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gsowrlxcn.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gpnobhnuz.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gfqynnzpj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gmkfrybsl.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gujlpsbck.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gtxgplrqx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gvhrfgsii.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gszverqwx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gjplbzrje.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gxifbxtyy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gjccghbhv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gehkzfokv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gajowqomx.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gkehsfloc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gzutulcbr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/grpienyfe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gidddfrzg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gnfwlomud.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gnghndvfr.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/guhhgxslf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gstbqhkdh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gthyvfsof.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghgfyrtqp.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gmerdvqow.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpehxbcfv.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gziwylgnz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gwfmmhjve.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gamdkkoma.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/geskuktiy.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxjibcktv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gllvqtpxd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gggvnhzws.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gcajdhsfm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gndhuqhjh.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gkezgogwl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gyuesnekp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gclfefsdl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gnlgwhemg.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gicwlchvs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gjxguqdzq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/grzckyqso.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gmbrlopoj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gtbibdxda.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gusybfpox.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/giuzebeyr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gqeyzsusv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gwmepwktu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gbofyqyrb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gajugdxzd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gacqoxkmn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gxjfdnccp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gzurplgxb.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/ggwuazaji.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gcirfkghx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/glcelyivf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gdtrlpamn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/guolmakzm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gylqqqrsn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gepmrdjde.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gghwgdtuh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gtiqdmazq.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gtsqzvaye.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gljshepxh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdgwgqsdi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gxrndyhvh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gzdhdslmy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gkrsruzcj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/gxjaniapa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/goymqvnpj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gdxngblzt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gvxoueogd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gnjptrayl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gnebjbwbr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gqtyjwlru.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gjzhyltxv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gqtnsctpr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gugcgnuxa.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gtzzzfysc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gqussxztw.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gdghhwnbx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/guikjtpus.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/glgxwvxlb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gpegduduj.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gyyzqsryj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/gnzowjlem.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gpepdztwi.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/gixuskjid.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gbtgbfvpx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfsspwlyc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gxrpxoqmx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gyebiujyf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gvirzrcbb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gihieeita.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gxcgsmvqa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gcuwmlght.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gsmzcsfnw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/ggsbiokag.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmwqeppxx.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gsuhykmbp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjawhfioj.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/giucvckuy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/ggefuwsob.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gxbewliag.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gziawveac.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gkjzmhjfq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/ghgxfftyv.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gqytwekqo.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gadbixses.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gxlxwijqy.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gvuqaebqp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gkiybhwfr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gwuszoflv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/guipelabn.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gbrrnqjmx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gbckwkvuc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gsjxfqcre.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gwknyrbff.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/glvaahjwl.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gqwsgiwnz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gqhzzujcs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gnxpjufbn.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gqvhvmscr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gzosefuou.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gpndbswsk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gfjkrvxap.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gazxnninh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gfumgveau.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gguxlpcst.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gtxjkgodn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gaatpwuwf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gwgozxmie.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gnywlsxws.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/grgfjzacj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpnbmmhha.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/ghwiswmoy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gzolddztk.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gcxzxpomf.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.hesvh.cn/Article/details/gxntiroyv.sHtML


<!-- 参考信息 -->