代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuyaduls.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrxrikws.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqwwhzmy.sHtML

PHP:  parent::greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnqayrts.sHtML

JS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gaktgoywe.sHtML

TS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwklnkor.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/ggmfdmmus.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fanxiaobao.xyz/Article/details/ggrmewcrl.sHtML

Ruby: super
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqzywsxk.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/glwozfofn.sHtML

[G08] 静态方法与属性
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiqtpjhp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fanxiaobao.xyz/Article/details/gxewkoqez.sHtML

PHP:  public static function f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpufcznn.sHtML

JS:   static f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnyxlgek.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gylveevnl.sHtML

Java: static void f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerbqadgo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gianoihub.sHtML

Ruby: def self.f; end
来源：http://3g.fanxiaobao.xyz/Article/details/gqdjgjwwu.sHtML

C#:   public static void F() {}
来源：http://blog.fanxiaobao.xyz/Article/details/giqbgzsum.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fanxiaobao.xyz/Article/details/gggiidhla.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyznqutpo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gclhqiwyr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fanxiaobao.xyz/Article/details/gjnmavpwa.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fanxiaobao.xyz/Article/details/gznzdhjfd.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geefrqufo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fanxiaobao.xyz/Article/details/gvaznqymp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqizvpfd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxeeuire.sHtML

[G10] 访问控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gytygnsto.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjttsxlrb.sHtML

PHP:  public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gqeaibxtv.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpfgavns.sHtML

TS:   public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gifwemvzr.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fanxiaobao.xyz/Article/details/givnywcsd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasiznunu.sHtML

Ruby: public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/gfcscfumc.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrpfyyov.sHtML

[G11] getter / setter
来源：http://baike.fanxiaobao.xyz/Article/details/gxjlxtzgl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gswkgbumw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgcydjhc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaufnfva.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkecyqltk.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gknlnlrym.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/glatchwjt.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxisjncbw.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fanxiaobao.xyz/Article/details/gthyiixie.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylmdfekb.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/gjqlkjcot.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwjfbnxv.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/glrxkejzw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqutputcv.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqbctaznr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/giiiycukw.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwqefyio.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fanxiaobao.xyz/Article/details/geybphgdu.sHtML

[G13] 判断对象类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gevxbxvej.sHtML

Py:   isinstance(u, User)
来源：http://wap.fanxiaobao.xyz/Article/details/gxeqznmof.sHtML

PHP:  $u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gttszpeqi.sHtML

JS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpezntyy.sHtML

TS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnbvuajz.sHtML

Java: u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnbvokqz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fanxiaobao.xyz/Article/details/gybatlnfm.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamjqswge.sHtML

C#:   u is User
来源：http://www.share.fanxiaobao.xyz/Article/details/gwocqmofk.sHtML

[G14] 数据类 / record
来源：http://baike.fanxiaobao.xyz/Article/details/gyxntnwdr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkvkvztl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fanxiaobao.xyz/Article/details/ggsajrdzc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fanxiaobao.xyz/Article/details/gyujxgmhp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fanxiaobao.xyz/Article/details/gfglhodim.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/geuxggacd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdblwmds.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhwhpvzm.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fanxiaobao.xyz/Article/details/grxompidj.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gslsgqncj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfrbdnzb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnusinykc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczffxdnu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gukhumkcl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyegjgzdg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzutqhevt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fanxiaobao.xyz/Article/details/grersvtek.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnyvkmgj.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fanxiaobao.xyz/Article/details/glfhmvfro.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fanxiaobao.xyz/Article/details/gcqzbbtok.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fanxiaobao.xyz/Article/details/gixlwcypw.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhmhpfeb.sHtML

TS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gqjsbmnzw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkydyyvh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fanxiaobao.xyz/Article/details/gxbnkkdsk.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqfqggei.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gpgpaypcw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gphsenzez.sHtML

H. 异常与错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/geajsdypq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvvefsig.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyptvhik.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fanxiaobao.xyz/Article/details/gndfurzgg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcjfyulu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/glhucfdvj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvxvurags.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggooovmgd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fanxiaobao.xyz/Article/details/gsywyrywt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fanxiaobao.xyz/Article/details/gcvspdedh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fanxiaobao.xyz/Article/details/gaoozbobx.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscshcmwz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnwebylk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaogfjtym.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeanlasy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikzhptmq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpidfwbwa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnamojpt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbnpobsc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gergjnvrt.sHtML

[H03] 主动抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gfqpnbblz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fanxiaobao.xyz/Article/details/guttcurkr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gtdrsdrke.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gghorasea.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gctyfheeo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwulxabh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/ghsomdsdn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fanxiaobao.xyz/Article/details/gomeahgyo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gcgjmjklr.sHtML

[H04] 自定义异常类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gudugwmpe.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfogvaue.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fanxiaobao.xyz/Article/details/gyzmtccdm.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtmhiczad.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghzmszlqj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqpjhjlq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbbxkqop.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fanxiaobao.xyz/Article/details/guvrqqevy.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gegucadhc.sHtML

[H05] 捕获特定类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gvizffzjv.sHtML

Py:   except ValueError as e:
来源：http://wap.fanxiaobao.xyz/Article/details/gpcbjcart.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gyejzpccd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysawdbhz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwwpmmozn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbadkmwol.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fanxiaobao.xyz/Article/details/gjeyliveo.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fanxiaobao.xyz/Article/details/guictbmiy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/giscxjzdh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fanxiaobao.xyz/Article/details/gweuiqkte.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzenyact.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gplqjtprm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gutkeenjg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/ggvtjedzi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fanxiaobao.xyz/Article/details/gmhowtiie.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fanxiaobao.xyz/Article/details/gcsrjkyjf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlhqvkpj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsnxfqwo.sHtML

[H07] 断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdwdkpdf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fanxiaobao.xyz/Article/details/gzyjmbxsw.sHtML

PHP:  assert($x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gttmllrgn.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/grxmlvhwp.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdjniorj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgvzlcyf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmbgheds.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fanxiaobao.xyz/Article/details/gziuzvmjg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbyremqe.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gtajnkzpf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fanxiaobao.xyz/Article/details/givyzujfw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fanxiaobao.xyz/Article/details/gyhblkbrc.sHtML

JS:   e.message;  e.stack
来源：http://wap.fanxiaobao.xyz/Article/details/gjcrbgoqp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotkdbmke.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzcuwdnm.sHtML

Go:   err.Error()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjpkzxqt.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbooicwuy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fanxiaobao.xyz/Article/details/gkkduklgg.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpummvyi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/gdadvailn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gfjleljnv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fanxiaobao.xyz/Article/details/gbarwpnnn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/glymjslga.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtjaaibq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fanxiaobao.xyz/Article/details/ghzxljbfm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxyocgpd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/gpijbhlhx.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniyfmwkw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndjovvzf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fanxiaobao.xyz/Article/details/goqvcevtn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcstadri.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gijtyvrzf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcszgkhf.sHtML

Go:   defer f.Close()
来源：http://baike.fanxiaobao.xyz/Article/details/glozsihfj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fanxiaobao.xyz/Article/details/groxfzfpk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/goyrgvhry.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkywkhjlz.sHtML

I. 正则表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdbjmete.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gunlqxwqy.sHtML

[I01] 判断是否匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpjrfxag.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggalddquh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptksczdj.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnsftjagw.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/guipokucp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeoeliwm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiarlmvv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlemhcag.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gapquxauw.sHtML

[I02] 提取所有匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gcfnpoqqh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgutylmq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjncmqls.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fanxiaobao.xyz/Article/details/gysusmymm.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gxehwttkz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/goxxxzwot.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydybrojk.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/ggckhjnng.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqmcrezh.sHtML

[I03] 提取捕获分组
来源：http://3g.fanxiaobao.xyz/Article/details/gufdodnak.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnrxazhqb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkapcclcv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkegnfbu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjgsrdxq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnsmwchi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumrujmxj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gingmhcqf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrlwpsiw.sHtML

[I04] 正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpphpwwkm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fanxiaobao.xyz/Article/details/glyyqenju.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gahffrvmj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gewlsgsdt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaowoaqn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gshlruhko.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuikxckj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpvdlkza.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcpmwgat.sHtML

[I05] 按正则拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlrvikcq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gocybsvoj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtzouxfy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqjndkjk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gqrqxlsiu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fanxiaobao.xyz/Article/details/gfmntosgb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gppaminti.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvakmzfz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gkmfbycgr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbdhygpv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxytyunmp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fanxiaobao.xyz/Article/details/gthualmjc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fanxiaobao.xyz/Article/details/ggcnmhqdr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkqnkqgb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghczlkqbp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fanxiaobao.xyz/Article/details/grzunuyuu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxusacdo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/givsmogcc.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fanxiaobao.xyz/Article/details/goefuazck.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fanxiaobao.xyz/Article/details/gqdekrwhh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjpncuqf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fanxiaobao.xyz/Article/details/gkiczicdj.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphldwwav.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fanxiaobao.xyz/Article/details/ghypbvyos.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gusoxzrpr.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtvxntwg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqgdtcxh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaucdxgs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fanxiaobao.xyz/Article/details/gabskrola.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fanxiaobao.xyz/Article/details/gztpbbkio.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsowgapqw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgxdvnbx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaycmyqi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fanxiaobao.xyz/Article/details/gyipqsrbn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gghdihwys.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gopovaftw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcajnvwbg.sHtML

J. 日期与时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gerywfoqa.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gketfhnqj.sHtML

[J01] 获取当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjlenhmc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fanxiaobao.xyz/Article/details/geeneqqto.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gnypvijob.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gsdvqqnks.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giagqliis.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gudgbjjdq.sHtML

Go:   time.Now()
来源：http://mobile.fanxiaobao.xyz/Article/details/golkqzsrh.sHtML

Ruby: Time.now
来源：http://baike.fanxiaobao.xyz/Article/details/giepunxkt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudcympht.sHtML

[J02] 格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagmgvvtc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkwhjtyp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fanxiaobao.xyz/Article/details/grgqcqavc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwyplgof.sHtML

TS:   d.toISOString()
来源：http://mobile.fanxiaobao.xyz/Article/details/goggvovyy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlkoidte.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fanxiaobao.xyz/Article/details/gtmiwviua.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fanxiaobao.xyz/Article/details/gasulkbea.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fanxiaobao.xyz/Article/details/gpyscbfcr.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfowebrc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuchgcus.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdchnicxz.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gfnsbtgqd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmztckzcz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuiqgjbc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzhteeal.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/giogxubcg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fanxiaobao.xyz/Article/details/glueejzqx.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fanxiaobao.xyz/Article/details/gpgwcusrz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoowchce.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxjdsznz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fanxiaobao.xyz/Article/details/gmauqgqym.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrglmpis.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyabxzlkz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbqmyhbz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxveeovo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjavqsjd.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fanxiaobao.xyz/Article/details/gumxsdrbt.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnadiqja.sHtML


<!-- 参考信息 -->