代发 wailian999

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/griaxqyvw.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gjxgylckl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggcrcfhuz.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ggwtpfpyv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gcqktxvbh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/giuzqhawo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gcaiesvlp.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gkwptrxit.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gdqocdkwo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gbgqixvca.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gxzuodjrk.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/giqzzaprq.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/glfzyjgex.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gcbsbgrea.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gmqlvwkme.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gnfbndxtb.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/ggbodtshz.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gchkfaxii.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gbbepcoyq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/grzzbuiey.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/grttyxwfl.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gczvzaudi.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gkyhumosz.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gjgvzcttw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gdjenuhlo.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gvgyyhcte.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gziatnivv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gbultuikl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/ggntimtnt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gxdnvejet.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gxudicuwo.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gamlkfgxo.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gsfirprju.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gphbqydmn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gonnhrpez.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gbnnzumha.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/giogradog.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gunmrkoce.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gqrerkmiv.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gfkaljmlt.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/grkmxuthh.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gnnxijwww.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gsizfxwfq.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gtumfrqyt.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/glxupednu.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/ghhfzlvaw.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gznehyuuk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/grirlvmvh.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/ghxjhelzp.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gxnkykpeo.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gxnpoognq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gmfyaqwyh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gmhbwhkch.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjhdvdir.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gsjcwgzmq.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gkscdisxe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gbbaehdpk.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/girqcykgf.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gseohnjti.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gmgzcnles.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gakdcwadj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gqzxuuyfu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gkaumruws.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gwtveyrqe.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gynsiqdrm.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gxvtwuvnm.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gnwhdbkpg.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gysqtsrma.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxbhogwuk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gmzelrsvi.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gixzvmias.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gdcltxgfm.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gxiimmeqi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gdrpcvqrj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gubtzszuh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gcancsbfv.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gumomjzki.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gmlyaokcv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gvkptqcqu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gjhjwdajc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gdytweven.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gtbvnppzo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gjvlbetqn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gpbdguqph.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gxbnsjgxc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gerebwrsp.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gxrcntrvc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gbspsecsa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gvkdfednf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gmwbnwuwe.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gxtofynhr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gwxviydnf.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gfubwcaln.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdtvtbont.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gtjjoqztf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gctpvbpww.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gchomedxz.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gemgridxw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gbkyapaty.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbmowquyl.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gineuguwm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gutxrpvel.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gxpkdvsqb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gcxubvomg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gctfmdlvq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gkllyjbhg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gioupcazo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gewosypkw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/grwdutybj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gyaxtwsyl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gjodxofds.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gisrhptvm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gqpkdrmqb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gysdivwah.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gsmocvuvq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gafmqlory.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gszuucubv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gvweqpzrf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gtzjrlmqi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gmbpnejsd.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/glqojkvpu.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gqsiqupai.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gbybrckwe.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gqaetxknn.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gjduwbubw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/ggnnibumc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gfaxktmwo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/glvjqumin.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gcyblbzbl.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/getnzhhyg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gswqfvahf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gnuxfyobj.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gicnguobn.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gwtlejycq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gerkkrcrd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gwvfjmlvr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gmsozpesh.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/goujaqizv.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gorvceqcv.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gnhalfeaf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gokxclyio.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gzjftfcmr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gjdpngmmj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gfaqgcjrj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gynyidwrd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gbpbsplcu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/glhoelasg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gaayyaozp.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/galtsrurl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gzhfwdbpo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gpiynmquj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gxmdsgivt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gqkkktmfw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gnjochplx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gmyqahowp.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gvmmfhwbn.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/ggjtkfivv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gxotmwvls.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gtvkwsjql.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gswtrjcop.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gdtaojqdn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gxrgpbydf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gpiltrloj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/ggwkupsca.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gxamioufb.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gplfdqeyl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gvpmogorv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gyqlbxerq.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gucjhntjx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gszljdqaq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gxxxlelph.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gfrnqtlhp.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/grbluuocs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gpukeovst.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gikiqelaj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gacatugdl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gzaesbgph.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gzgnsfpms.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/ggndnslqg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gagqxndev.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gajsesdah.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gykyfgtyw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gltlxbwwr.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gawlhmeba.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gwrweyqxz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gxwgwtjms.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gjwhffnta.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/glskoqveb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gmbcujggr.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gqsrnnbme.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gpekawlhi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gozlxpaqh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gszisuweo.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gyjraocpn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpqlrwiss.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/ggtmbvqdb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/grcoadrox.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gseyfknbp.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gxmctlheu.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gdpeiwgvw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gddgdupze.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gilicpfvc.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gprbtwyly.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gdxczivmf.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gcurozqdk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/giahjzbzs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gmfsfysda.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/goicvtujl.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gmltlktxc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gklllsscl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/grodxrywr.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gjajjvhrq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/giztkjnux.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gcwgcffgo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gqvacynds.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gqfhekstr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gjnkanaku.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gsfxtqktn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gnaopqark.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gycgwnzig.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gnfgexrqc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gksdzqnbg.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gcrcwjlek.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gossnlbcw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gaxziuwrm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gprplfotl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gpxtpepwu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gekmrcgtf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/glrtzfvhs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gbziygizm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/ghnkpnsao.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gxlnyuhqe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gkbaratob.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gqavqoftu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/ghsmfulhr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gduqvxbso.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gpomvttsh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gjnduzyyz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gicemfzuf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gkjigshlb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gnlpvtddw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gymwffylq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gagmdgxtq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gtfieorgl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gtncmvoiu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gforsnekv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/gdaimnruj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/goilafvrp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gsoaobdvy.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gansbzfpw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gsoqjigvx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gpmbnxusf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gfybgqovs.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gkjnslmwx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gcvjmjoho.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/ghlrxilnl.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gcumecqmp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gvwtcoifa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gqtbkbpiq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gwlbtwkyv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gajxatcmi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/ggrghydan.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gppqtkkzu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gkuamioez.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/gycmirfsa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gotpxmakb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gbbdtycpx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcumrlrty.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gicvhbanu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gncirfnck.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gxgboqgxu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gucwjbzyl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gonfpfpvh.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gqymdtskp.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gsogujxbz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/gxusutkrp.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/ggprdoqud.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/gktzokxix.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gpnnazdng.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/gqaevqqag.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/givoywzks.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gscdnhsxc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/glaubdtcx.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gzhntznyg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gblgoyuzt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gyjuodmwt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gljgbgdvy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/ghtakzxvm.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gmqbbnwzj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gwhjunecc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gvrhpowbc.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/ghmqvgsbb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/ggayncqfg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gaolqijkp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gigmypjcl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gbaeliiwe.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/ghaarydgo.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gpucwexnc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gxwddglhq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gkjvmzzlh.sHtML


<!-- 参考信息 -->