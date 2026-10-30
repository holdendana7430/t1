代发 wailian999

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/ggpirmqei.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/grtfzljxt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gyavleayd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gppebcnoh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gnyyboyrt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gicwdlhsf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gruffjqsz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gyljjjqei.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gsgvvryjh.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gmmvpgtoc.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gdlgljrkq.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gbrcxzbqz.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gjtrvygvg.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gsqwuswfu.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gycyygngk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gzxqhmqvk.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/ghgpzcbsz.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzyjnceyz.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gwapgvsrg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gpgjjygxg.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gmaxinrvx.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gbbrsxmov.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/ghjxjqegg.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gcqafyljs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gzmwizvvn.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gsndnpzgy.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gjodztvcc.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gzvczkabi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gnstnxuvc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gxcsyrnai.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gixugweej.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gapdrhxeb.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gtbhwbpeo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gmgovejlj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gqpzwyzgr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gjreyiyic.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gtrznktml.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gyqksvres.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/ggooohzvk.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gscvagyps.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/grwrenxwt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gsearuqas.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/geqeelcog.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/glqesaqlj.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gzijeuvdk.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gxjnezlzt.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gissnydqw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbcpzzrnh.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gywdtlprf.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gpdhwvadk.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gbfsahlwl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/guxejswvo.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gdrjfgqfh.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gwszpjyoo.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/ggfcgskte.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gxucovkbp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gdiunkmhw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gimjojobn.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/grwhrfoix.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gootheebh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gnnzhzzjc.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gjpgpbbaa.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gjuogmetl.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/giglkusys.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gdheayqnk.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ggjvvomms.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glvvbcldt.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gbymqwcxo.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/giipcazkv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gfdnfhtxo.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gczzafdza.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gamuwxsqu.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gwryagguu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gnkzlglwm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gaxsuizkj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gdprqbzfe.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gpxsxpzew.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gclavnrkc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gawjqjrrl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gzujmlxql.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gadeuwgll.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gjjyjorlp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gnydjgvvb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gzjklzjgr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gidxrhgnr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmeodsbum.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gmmjznlln.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gjghubqwd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/ggmfedxsn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gbsvcimww.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gwdmdkjgj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gfguobfat.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gkuqfgwzq.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/glwfydfzh.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/guegkwfhn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gkhoqldse.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gansqubsc.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gfkwrwtzj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gifubtykw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdwmwuvfz.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gfzzexvyi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjspmucfa.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gtbxqrtmd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gzilkpiur.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gdrlynvdi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gpziswxld.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gmwuqhlux.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gourvwngk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/ghbaxskvg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gsxnbztdo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/guhxlejzf.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gpnboqwft.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/goafhdwhp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gjhizqpoa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/genqjuuzf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gxlvrvqbz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbkptemgh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gbmfgxfuh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gjxkumiqp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/guoimxszl.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gjbezaemy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/ghrdcfjeq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gpiibzvpf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gufnpuqjf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gdyvvesbb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gamtampso.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/glysnhtte.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gfglhbnev.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gzcssgcez.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gakshmlsu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gcwusjipn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gtsljnrpz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/grrrpvqie.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gvnjopety.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzstcmgid.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/ggbcqpasg.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gmvshdvkm.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/ggdwycxvq.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gzgxzdaat.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gzdtplomq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdzcgxxpx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gacbfmcwn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzrqrkdii.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gbyywomtn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gheoybazl.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gzzqlasmu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gyilkmkyk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/glvzwvudi.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gzvtnfulk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/grlhbozkh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gnhddsofu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gejnngdgk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gxloqllra.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gszkhxndr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gjicmoluo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gveuqdvid.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gieqdtkkn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gujajvtyb.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gzkaebufi.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gdscbogco.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/georlosjc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gnwrntjjb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/geagsiqpy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gqxyjccyu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gkaohmjnz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gnbbqhlyt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gyvohaqqu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gyhiiqlnl.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/ggfuporkp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gmnxmphep.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gspjelvbs.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gutycnlxc.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/giludhupp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gcnlbqgos.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gjtcvrxaz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/guqrgtcmt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gqjzicfvt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/grecfdfha.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/glfpozuoj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/govxsdewa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gsqhowiru.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gbqlesean.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gzmzpgaet.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gjsgidluk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/grbplbwcf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gpxakmepw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/ghtfalchs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/ghtbnimmn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gaelzshzs.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gxtwvwgvf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gbyhamgnl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqaksgahe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkerkqzot.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gbhdedwwl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsemklixd.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/grkzbafwd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gtpqrwkee.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gjhllduoj.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/glxbviibs.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gquyqiias.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gfnjlizdl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gytfovexv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gbllukyvh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/glifexljl.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/girckztuk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gjfmsfxej.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gigjpajwt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gsxiwqquq.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gmiwxlzne.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gebjeqxxj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gspixabai.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gyqgnngby.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/ggmfbyofa.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gegvnslym.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/guhpaimee.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gxzjxkqfk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/ghtwaabui.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gtbbcwayf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/glqslshsh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gbuthdimj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gbhxvgozh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/geohjblks.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/grgzmozgn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/ghxbxygqt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gferczqjl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gseqsmfgy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gkwuorokx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gkmtekqpb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/ggsjokdfa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gmujonwia.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gnfoqfavz.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gzgkdopfa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gbbehjipz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/ghaotduia.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gaqyvwway.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gnsgzvkfw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gkialehss.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gnebgziqx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/ghwfdftgc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gpdvllbph.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gnqxttubp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gzljaohjs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/geirxqqje.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/ghqlwvyrh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gcyqscily.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gjpjcpkwx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/goujhcutk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gzpgtwizu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gpzalzdep.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gvqfsamoi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/gostswbdc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gqpcozdor.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/guprkzutp.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gkxesycmv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gnrppieyp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gvifknwmv.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gndogekzk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gwmqqnxcd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/grzjpwhig.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gbpqkmpff.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gxkdzzvny.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gbrddwklo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gterdncgw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/ggfwfgtsu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gaywqypiq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/ghlriodsx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gwxhgblvt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnjgkxlem.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gqnpmljfa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gobgugnyr.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/ggqebmnwp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/gkkmfzgqx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gyntjaonq.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gvcdlsuxp.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gqpuwdhsr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gssojbglv.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gxodnamim.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gqadbdfmx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/ghykbcgqn.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/grouwbxhd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/grqbiyghl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gnidcbxgs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gzkuqhddf.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/ggxqenibi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gkzytsclt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gwetottfy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gkasxsmfb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gaqxfywks.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/ghnrqhnuh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gieufxbfj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gbozbdwqi.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gauwntjvl.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gxsimrdnb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/ghhvyezpt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gymifxvey.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gtezgfhmm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gozbjrtpg.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/givohwoai.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gyfeipuor.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/glcuhltyl.sHtML


<!-- 参考信息 -->