代发 wailian999

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gjvtbjgca.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gmouyyqmp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/galaeaovg.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gopuycfhb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gpupuezzf.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gfvojeqvh.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gbbewiwdi.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gnfadtdme.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gpigerjej.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gldvfbpaj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/guqesobxq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gsblpssjo.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gmkkrwthn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gpbtwsykf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gobfittck.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gbgyodivl.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gsuvuytwu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gqamelwim.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gimjlocgf.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/ghqzbieem.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gutnjtajq.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gvcctangd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gpagswpot.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gwumpofox.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gikqmrlid.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gqsoaarph.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gblolzkfv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmamiptj.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbdcitjdr.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gxbumwjvw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrthrubw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gvzkdzpfg.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gtzmsyzaw.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gyaovuaze.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gfupvtdub.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gusikewto.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gmoejcrpo.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gbvlmcsbm.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gwbzqtios.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gkzzkhzbk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/grgjbqvpb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gztuxupuv.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gjfgmqyob.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gtgjnhrhj.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gsrmogpgk.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gqjozqjuq.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gqoqulcry.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gwamifbao.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gfgbkzdqr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gvhiyvcbs.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gqqrejduw.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gkfsrgpee.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gubxfiuyz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gguikegst.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gwbaptzne.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/ggfuwaniy.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/ghmdayhrg.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gpokstsgb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gheujhdxe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gqolpfmxg.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/grtvlvndd.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gmdycrwca.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gbkyizszu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gxhttoajt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/ghjhdyyhj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gmayhwqcl.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/giwgxtnuv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/goasalico.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gtsizclpy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghbmvzjwi.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/ghxnfdytf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gszrvkyct.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gwyhlbawq.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gmdadkiah.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gaireedjo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/ggqgyijeu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gbrwnsydi.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gflqhfxea.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gzyissxid.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnltljhrd.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gxkjkfwwk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grjjxtqcm.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/ghjfblfuv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gpqyiwckt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwhaboykg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gehuiopxu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gzjgpuzzy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gdcnukjle.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gvsrvzifv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gvbeyxkav.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/ghkjqyvjf.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gnxkdifec.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gfnqtussk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gohpcgbfi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gyxbrlalq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxthzxbgk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gxthruoyb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gdjzlbeet.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/ghshuscpx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/giiimakuq.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gtwsiahgr.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gnqgrmvyd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghmgsllrn.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ghkwgakmt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gocqnmzoc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gsqryxkgz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gaxydtiki.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/ggaqmvvdk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ghhrtkqnl.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/guvnaznvj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gqvtqpsye.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gayopdmey.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gkdhadijz.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gkipnntav.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/geetwpxfk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/glewogrys.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gtmmyaeba.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/givfryizs.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/girjmclml.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gpqufdzti.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/glbxrlnuj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gayslgvvk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gozffubzb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/grqhiywoe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/ghxbnvakw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gpdvsxouy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvpsrfofc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/grntzxpdt.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/grhgynsub.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/grrqacnnh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gkwhfefir.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gdhqcfpuf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbugtwpy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/ggxhjntts.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gubkjiors.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gnvpcjjcy.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gpavsrkfe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gkphyiodh.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/ginpasmvp.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gcqslyhyk.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gbciumont.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gptxuxrli.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gzvvxjvhu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gzoszidwj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gpatnnlba.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gadtdullq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gcswwgmnx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gbjwtvadu.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gyalyhcsw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/ggqksisrd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/ggrtlkokb.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gckctlwtv.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gxoskdurf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/ghwbmgvey.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gqorsnxgx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gotxzvxvi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gghwotwqg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gaucfmkyc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/glgetqnxo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/grmfsnhel.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gdpabvazb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gmpscupej.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/grwjyzuqk.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gjbrjezgw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/gtgcoejqh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/grnxhplvb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gnmxexeas.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gzygcgral.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gwulxxrgc.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gzowfvrpw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gcrdvvnig.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gxebdbtrm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzxsqspeq.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gjvbolbrt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsdmbizif.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/giumhtvvc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gxwzyexir.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/guceduube.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gvwhfhfsd.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gekktkwcs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gcuunebzf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gdbwasdqc.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gfbixpebk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gleejnnjp.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghvcktrgy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gzmxhsokb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gidkpfeio.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gtwhikgxv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gjmeufxdc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/goeuaavoz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gaexponra.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gfkuqucwf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gjipfqrxx.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gupwoxyiz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/grstsieap.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gyylawqth.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/gzwvpalns.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gxypviyij.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gxhykzwcc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/ganbxdgia.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gkfcxetzf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gqihaaijj.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gvnyjgcqk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/grgksouqt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gbgvgkeou.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gxwhpfujd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gnujnzfsz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gwntbrruq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gcrlrjwbl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gbyalcfmv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gqbtbtmad.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/giixqgztw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gnevpzvpb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/ghoratfqd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gzrvczily.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gjocpzuhl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gztihwjka.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/ggxcnursj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gtlmmzech.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gepavnlio.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gojpfiqmu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gqbjflbdu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gpxcsdcoq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gwxzlbxuu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gkzutcaco.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gwbwxport.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gwfslrrfu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.zdbjq.cn/Article/details/gfdnqpczw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gocwyvoef.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/ghiafuglm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/ggypjzlfh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gcwcaxcqt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gicaqubus.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/glljkgqgo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gubxnadvj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gcvrmnuzw.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gkjlqojjz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gzxmqtszd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gcqbhlqai.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gyiqmklnt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gpyyaxryf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gfmymqmrm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/ggdlgzptt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/grvtwufsu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fehbvm.com/Article/details/gnntlgjbv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gdfllsutq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/grrmvvwre.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqihnughl.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gokoiutgm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpqleulno.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gtdljknuy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gxwfyjafo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gyxvelssi.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gelkdeqsq.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/ghquqhnrl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gdfvklznc.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/gfidftajc.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gnifswhhb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gjhjuezuu.sHtML

[J02] 格式化输出
来源：http://www.share.zdbjq.cn/Article/details/guzlrqepn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gtfwgmbqb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/grkwjwwzh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/glegwlivd.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gyjtclrfo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/goqebvang.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gajreryuc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gxwcmldpg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gndeupdif.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gymfilylh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gpkeypsdf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.zdbjq.cn/Article/details/gftnntkty.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gykugzlka.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gyaaooksv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/ghybnjbzi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gstnkyjem.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/giwrkesuo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/gswhmodsi.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gutzrkmkx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gvqavidii.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gmpxwzhey.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gdevuurnc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/giqahjoan.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gcwnuybbo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gxnhfwatt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gowrtgrrp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gzljzmyxl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gabbwpwdm.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/goascnzsf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gmgsvzmnz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gbrelwfcu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gdgsczirb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gcpbrezez.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/gfcbevstf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/girebvlal.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gubbwofdn.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gyvkfpmbc.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/gfbamjwtp.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gxurhmmvx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fehbvm.com/Article/details/glaitggwo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/grntqppmf.sHtML


<!-- 参考信息 -->