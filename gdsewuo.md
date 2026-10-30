代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjagupkbo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/glzbukqti.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fanxiaobao.xyz/Article/details/gnaskwsva.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdkityxz.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fanxiaobao.xyz/Article/details/gbdtcaxqk.sHtML

[G07] 调用父类方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgzfzbev.sHtML

Py:   super().greet()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhdiocdo.sHtML

PHP:  parent::greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjrguwcv.sHtML

JS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/geuziffew.sHtML

TS:   super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/guozdjril.sHtML

Java: super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbljguiy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fanxiaobao.xyz/Article/details/gmavuqxlz.sHtML

Ruby: super
来源：http://m.share.fanxiaobao.xyz/Article/details/gulyeuusq.sHtML

C#:   base.Greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gzfhtdrfc.sHtML

[G08] 静态方法与属性
来源：http://baike.fanxiaobao.xyz/Article/details/geljzxymn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fanxiaobao.xyz/Article/details/giwizhmyj.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/goedpnrmj.sHtML

JS:   static f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjkrfvte.sHtML

TS:   static f(): void {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtemzszwd.sHtML

Java: static void f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbgsdmza.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fanxiaobao.xyz/Article/details/gxambercw.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gsedijlip.sHtML

C#:   public static void F() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpbvwxhx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fanxiaobao.xyz/Article/details/gjdtcbngd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijvizgmt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giiykpdrf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fanxiaobao.xyz/Article/details/gkofcvbka.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqakkern.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/goouhhury.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwsxpmcu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fanxiaobao.xyz/Article/details/guxlbkehk.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjefxbxsq.sHtML

[G10] 访问控制
来源：http://wap.fanxiaobao.xyz/Article/details/gsnlutvek.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvtydqxn.sHtML

PHP:  public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gsinrhywe.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fanxiaobao.xyz/Article/details/guyrwhbjb.sHtML

TS:   public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlzxouxr.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fanxiaobao.xyz/Article/details/gecusbzjy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fanxiaobao.xyz/Article/details/gysbalozh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvheqkwjb.sHtML

C#:   public / protected / private / internal
来源：http://baike.fanxiaobao.xyz/Article/details/gudnqkbsl.sHtML

[G11] getter / setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafvxjwxw.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fanxiaobao.xyz/Article/details/gkfqgqbnx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkjiaqxge.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggsdqkbsa.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaolxgud.sHtML

Java: public String getName() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gejzwklzo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcagjvgip.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyuksger.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goulfqqui.sHtML

[G12] 对象转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzhhrwuz.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gexisuqzv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxybbhhhl.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghmhqsepo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzadzbqgm.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrgsntvr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaahdmfx.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxzkfcwd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxmvvmme.sHtML

[G13] 判断对象类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gjryrapfd.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fanxiaobao.xyz/Article/details/grhzkshgo.sHtML

PHP:  $u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gtshoodrw.sHtML

JS:   u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgorezeg.sHtML

TS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltmtslou.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gppvfmngc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixphmyws.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gprjpesom.sHtML

C#:   u is User
来源：http://wap.fanxiaobao.xyz/Article/details/gpesuella.sHtML

[G14] 数据类 / record
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsotujwq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fanxiaobao.xyz/Article/details/geyrsgvhs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fanxiaobao.xyz/Article/details/grygequkw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxquozore.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fanxiaobao.xyz/Article/details/gasyfusdo.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtrgdtquf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gadvrgksl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fanxiaobao.xyz/Article/details/gjgeqpbbx.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fanxiaobao.xyz/Article/details/gvkoikasy.sHtML

[G15] 枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gqotzfghd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gfntrdnsc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glufmdmxl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtqnvckz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gvdorypdr.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fanxiaobao.xyz/Article/details/gszpebvgx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyzqyfwf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyitpzlk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaijlmzx.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpolxycr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyvhoogu.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyjtjroh.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gczmhfwmn.sHtML

TS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gxqchbofq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fanxiaobao.xyz/Article/details/grwilcqvx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwzfbufv.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fanxiaobao.xyz/Article/details/gczsbhyin.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/ghxscsrrd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtxwfswz.sHtML

H. 异常与错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gahqbvrkp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhrohtbg.sHtML

[H01] try / catch 基础
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpxewcpx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gnoigkzui.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqryishg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gynopxtck.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzoiuawf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gajkikogd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtceabem.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fanxiaobao.xyz/Article/details/gvffvxoha.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvikuooo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxwjvxia.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fanxiaobao.xyz/Article/details/goqfacocc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gozdwwdcs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gazepaljr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjuarxlls.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygjsuktd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fanxiaobao.xyz/Article/details/gjdiiltek.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fanxiaobao.xyz/Article/details/gsmkrkovs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gggdmloww.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvfpjrmg.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fanxiaobao.xyz/Article/details/grcktazvv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbkrsnff.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gysjbrhed.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/giaxcvigx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gyzvjzkwf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccnluqot.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeubylra.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgwzcjgp.sHtML

[H04] 自定义异常类型
来源：http://baike.fanxiaobao.xyz/Article/details/giemzskpl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gepwghycb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glbcphddf.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gaadljgzb.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouzsgnvt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbymqyvzm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fanxiaobao.xyz/Article/details/garsmzxsn.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fanxiaobao.xyz/Article/details/gqkhffrmk.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fanxiaobao.xyz/Article/details/guxuendwu.sHtML

[H05] 捕获特定类型
来源：http://baike.fanxiaobao.xyz/Article/details/gynyqjrms.sHtML

Py:   except ValueError as e:
来源：http://m.share.fanxiaobao.xyz/Article/details/guyxtowun.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gpmixzoof.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghofucxen.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkcbskhrw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkbgkjku.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fanxiaobao.xyz/Article/details/gkipapgdc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghejeoqyz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzsignhg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fanxiaobao.xyz/Article/details/ghucbpujr.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpsiudsq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gwyjkaigh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzybriqtp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyvqpglw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnbuwlia.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fanxiaobao.xyz/Article/details/gbuqqktnp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fanxiaobao.xyz/Article/details/giyttdztv.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gypbsnzvw.sHtML

[H07] 断言
来源：http://3g.fanxiaobao.xyz/Article/details/gzbmbxofv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gayyzjjym.sHtML

PHP:  assert($x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/glsoviomn.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/grtkmmojz.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gobqtxgxp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fanxiaobao.xyz/Article/details/gqsydtnlp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fanxiaobao.xyz/Article/details/gmholvbpb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fanxiaobao.xyz/Article/details/gmenifmek.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdldondp.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fanxiaobao.xyz/Article/details/gdjtztgut.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/goknokxpt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fanxiaobao.xyz/Article/details/gbglfvxut.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdiqkgqo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gbsbwmvki.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fanxiaobao.xyz/Article/details/gippfjhux.sHtML

Go:   err.Error()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthunxdbr.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fanxiaobao.xyz/Article/details/ghxmwqxsq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoteuiyu.sHtML

[H09] 带错误码的异常
来源：http://blog.fanxiaobao.xyz/Article/details/gwuknxqqq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndeypals.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkgnsrnk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrbgfjqa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fanxiaobao.xyz/Article/details/gpuefgnis.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/goayqbntx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuyogdrr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fanxiaobao.xyz/Article/details/gzpwybsdq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/gapfwmqhb.sHtML

[H10] 资源自动释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gppailkpc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrovjmjz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fanxiaobao.xyz/Article/details/gzztrkozi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/ggxmhjdij.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxruvhqk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fanxiaobao.xyz/Article/details/guqvtqykd.sHtML

Go:   defer f.Close()
来源：http://read.share.fanxiaobao.xyz/Article/details/gunzslksj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fanxiaobao.xyz/Article/details/giznxnjtk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gdwsfsrum.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gszttiabe.sHtML

I. 正则表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gssxlvyoi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbycwddkr.sHtML

[I01] 判断是否匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghresjp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdalhcygt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gmtbkpssd.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghawgbcse.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gndbxwpky.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fanxiaobao.xyz/Article/details/gakkxbkgg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubiygpts.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjodrryvp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdunqtjlp.sHtML

[I02] 提取所有匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrxrppjc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbedbqlij.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fanxiaobao.xyz/Article/details/gperrseey.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fanxiaobao.xyz/Article/details/glgfzdhek.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gnpsxzmin.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/grbvidrxz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggvbpheyv.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcztyzhbz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfsqgygo.sHtML

[I03] 提取捕获分组
来源：http://3g.fanxiaobao.xyz/Article/details/gxaovqcyb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/goopevzah.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/glsyonfag.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnvvtzov.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giomhxknq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fanxiaobao.xyz/Article/details/gbzxddwsw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fanxiaobao.xyz/Article/details/gogfmjdwp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glybkpbgm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqdxasjn.sHtML

[I04] 正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grcyjgurz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxdgansb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxdzxwxe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqxdxgow.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaoaxewg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gedprvpmq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqihujvkc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbquecpw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnsravok.sHtML

[I05] 按正则拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gnaapxdff.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpnoakmw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gwoqwzapm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgvkkjqx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyqcokec.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvsxnsue.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/govfkwhax.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtagwdfp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gzwiskzig.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fanxiaobao.xyz/Article/details/gqkgiqwwy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gmmnpwkli.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngthekpc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvuffvjn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gloxogqnl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/guoxgltxr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhdylfwl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fanxiaobao.xyz/Article/details/gxuachgge.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gsgwdpmyr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthipiyqk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fanxiaobao.xyz/Article/details/gkeirfzqf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gymylkuxc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhiavmgu.sHtML

TS:   /error/gim
来源：http://www.share.fanxiaobao.xyz/Article/details/glcluechg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fanxiaobao.xyz/Article/details/goixzmgja.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyrudozd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzejhabc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fanxiaobao.xyz/Article/details/gfrpdmvcw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrmmcnjk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fanxiaobao.xyz/Article/details/glfshocds.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/gnflunbfg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gopbbvaih.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gflnqriuw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/glpexibxe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfrywogn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fanxiaobao.xyz/Article/details/ghczihhfy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grerxjwyb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvsawbtx.sHtML

J. 日期与时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gektmjank.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmshwrzkp.sHtML

[J01] 获取当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gshlrkcxt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fanxiaobao.xyz/Article/details/gltzvrwqf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fanxiaobao.xyz/Article/details/gillxtmzv.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjqxjpvs.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gtarmleeg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fanxiaobao.xyz/Article/details/guwmlubkz.sHtML

Go:   time.Now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvwtxign.sHtML

Ruby: Time.now
来源：http://baike.fanxiaobao.xyz/Article/details/gaifqekdm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fanxiaobao.xyz/Article/details/gjoshgyzl.sHtML

[J02] 格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gsogkjxce.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbcjstaa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqsxczve.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fanxiaobao.xyz/Article/details/geeqnlsxf.sHtML

TS:   d.toISOString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gquijxnqj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/gwsljicqy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmptehizx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezpnkbbi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fanxiaobao.xyz/Article/details/goysposnh.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fanxiaobao.xyz/Article/details/girhbdvvq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fanxiaobao.xyz/Article/details/gaqcyvylf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiftihsz.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gflpklrcq.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcqvhmcz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyeqfbmw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwloxvdc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpiyvemb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fanxiaobao.xyz/Article/details/gbpxfcapb.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guihltzzq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhcolmfk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpldnuzz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqwrajfr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/geloqpuzj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcgyqiyl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gjlvhvrgu.sHtML


<!-- 参考信息 -->