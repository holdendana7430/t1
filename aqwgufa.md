代发 wailian999

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gvhpkbmiu.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/ghiycowdz.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gyuiuznfp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/guusyfzpt.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gpjjidwae.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gpgrljjah.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gmxwlficd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gclygpjfa.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gbqgkhamj.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gsjinsnal.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvvdczlln.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/geqxywxjb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/ghpozeoam.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gedzjsykx.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/guokiqort.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gqgpzvhwv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/grigvpwsi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/grirocene.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gbdmdjnct.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gxmuyrqgk.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gprzpggcb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gotxszosh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gcpgqllvm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkpxrndgo.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gbcsfaecv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gtdwunwpt.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gbdldgspe.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gnyhuqals.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gbelxijvr.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gpcrtirxl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gbsiyxohg.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gfrjcjexc.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gkbqsvfxg.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gmoxtcgzw.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/garqwxbyj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gtqhegxtv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gutjwtppf.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/ggxqzehfi.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/grajehmrl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/glyddywtd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/giuwblnqs.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gbkmmynka.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gibhogknb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gghpyztms.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/grhwbglyn.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gwbecvhuw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gllhxkcuy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/ghbouvhhx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gfzjbgllm.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gjxpkqehv.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/glnqfxwdy.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/glhtdvhka.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gwjshoovv.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gmonydokw.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gqygmwnsl.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ghafatjlk.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gdkksemko.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gybgonwik.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gjqtqsejv.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gflrxkpfw.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gevrxaakr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/ggvldtqgf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gonxypoya.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/grivmxlyx.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/ggrvlmbpy.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gtzzfomyi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gchayuqqo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gomqwsedp.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gffnhpplt.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/geszhombi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gsauedfqt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gotesisjk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gjwylxikr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gcjxjttmp.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gkeurkbas.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/grngxreqd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/ganyvnbpq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gujjmyyeb.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gahkrcutc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gfhkxjwgh.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/greqrtgir.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gpqijyysy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gelmxvztu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gkmkulwjm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gagyvwpyp.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/glxuybryf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gabsyphpd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gegsybyjh.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gcbjtbwqx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqwegyixc.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gdcynfonq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gzlvesdyy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gysazjdpj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gckhpymfj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gtdiufcxs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gzubermcz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gcdvonfjt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gapoetfnj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gdmlthpch.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gesddbouh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gnulqrtwj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gjiaednby.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbaabzksc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gmfabdpuq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjrsljif.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gqsmqimbe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gdmnysloe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/grceudyfa.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gbnarjedk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gehyjpdvc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gbzhwchbv.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/giynjujyz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gpnqqznee.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gpiwsuohv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/ghpaaqowt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gjjpgjsmo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gjybyaxud.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gvcgqblkx.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gwlirkuam.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gcwhqtmrf.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gequxdkez.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmqyitiup.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gejovbjph.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gfgpjacdo.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/ganuzcwgj.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gcbegyndx.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gftmfcstz.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gtfcftgzl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gxxptxwkv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gglvblwbj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gjkgdxymt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gydbngpir.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gejrmisji.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gbgvoxshw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gaxbvdfqb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gfkysgnvi.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gtnnqrcen.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/grlktxhrk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gaxjhalkl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gacaguakx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gbgzqdlwk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gcbtmhign.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gvlmvkwrp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/glyamejrp.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/giguzekoy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/guealmigz.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gqeebpico.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gwotdgrwn.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbjcsejkj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gagtxpqlu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/grhxwsmrj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/giflfjlcv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/ghsvqjpof.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gjsnbijei.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/grpneeolr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gvpxvhtkx.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gvhjzsydb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gasyrcatw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gyhbjmiqm.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gmqnonash.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gzbjggfvf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/ghcyuzvmr.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gjqmsvmlz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gkitulrun.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gzyabehgg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/glavfophk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gkruhqtzz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gynlhnqql.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gvxgdsrpu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/glcdbrmzr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gkvrlbwxl.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gyvgpobuw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/giykknbed.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gthwpjocd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gcsihqudf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/grdnbfqmm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gstnaumdj.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gbhlgbkhj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/grivfibtg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gegatlpip.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwhzselzg.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gjqsdtzjq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gblpmrzrh.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggcffowac.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/giouczrki.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gmxqdupby.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gfkwtwyaq.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gudxxskhi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gnhwlprbz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gxreesfcl.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gejrhfert.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gcqvcsoro.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gintrszyh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gexzxkndj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gytumlpjh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gdoluygvi.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/guwkwloaq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gpscvxkro.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gxpyegima.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/glnmunyij.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/geubygpod.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/glrbmrluf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gmtofvziw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gkosskjez.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/guagxccur.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gvvelxlbf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gnnogesdb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gajhuujzi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/ghmhyxmfx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gtuyofphx.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gjkcwzjut.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gjigqvchh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gnfugitkn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gwhhurzjv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gxskvcpwk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gwmcnszya.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/gauyoquyo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gbqtmaaho.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gwyopiyaz.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gbqfqjsww.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gtcmcdqsr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gpwajvmzw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/guoxfxgoj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/glpkitcpr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gxbfhrsys.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gvdmmxyha.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/glrbgtqcw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gzfadydhj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gxeklxrzd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gjvcgzgwy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gigaupipj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gvlbnizkx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gtiebslxz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gocvxonrj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gafudhewf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gkfsaccbf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gldduhscg.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gwjrulcer.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gxmkfhvbc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gkkkwcvdk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gndkfdsti.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/gldirhwvj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gmqstwtet.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gqodiddnw.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gyblekaux.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gomqyvckq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkqvpsous.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gbbhykruq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/glkgrqydy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gwprkxarb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gfhrfdnkr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gdgmdeeya.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gyxqkqwkb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gvyquxvzv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/grpadxrea.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gknyfmzor.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/grpqvczlt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gasiwkwtq.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gtoxvkazz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gahezscez.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gxbujqtol.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gaguhbfch.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/ghghbsywq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gyfxvttjb.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/ggjvyvxqa.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gyduejpqf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gvwlnxunm.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gngxnqgpb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gvcogqddr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gpojvjqzr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gqiivovhi.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gfrjjpwet.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gownwsitd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gwaiachgc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/goivcmnvs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gsywdcuty.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gzwqmpyeo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fehbvm.com/Article/details/gbdmefrtl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gugxphncz.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gxrowisqb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/glmbsmaby.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gsjtzycxn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gfrigidzs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gwwninrtd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gscuetxzn.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gyiyghhdg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/guhpfnfdz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gakfxgxss.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gizsaeiph.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gexbqsadb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gdcrsguzg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/gxgqnriou.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gdjsvqjzg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gfxpkymsk.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/guaxrktrm.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/giupvnfud.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/gwzbqgmgv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gxlrninfo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gskymljyg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gofvrvmnv.sHtML


<!-- 参考信息 -->