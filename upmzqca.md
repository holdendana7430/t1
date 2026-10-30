代发 wailian999

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gdzwcmyhl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gbmgmxwns.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gwndtpjuc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gqqyixvda.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gaemaudtq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gbznfqqiq.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gljtfcvlc.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gzlvwuuij.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gesoxsvmq.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gvyjwaett.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gvttuzwgh.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gbsrdiiki.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gukxjxnfg.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gqljvftai.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gnmwufmqr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gnrwreein.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gmncvjorg.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gzcfumebe.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gbtuoobwh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gjczvinmv.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gfvfzlnxs.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gwutyupns.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gedvbfqqx.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gfbpmygxm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/goivozibv.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcvxodkia.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gxruunxaz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gpnibxydm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gpysekdhg.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gzxxdaanr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gekynjdml.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gferqfxgq.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gkghdqzmc.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gmyeklczc.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ggywcdlzs.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gmonxrprh.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gryezitdm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gszzfvvvw.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gnqgyyfwd.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/ghgtossgg.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/getujksgd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gclflachf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gsyxmsowj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gqwbzfkmk.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gqltrjxga.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gezwdxzqh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gahwkzyzv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gwuoxprpk.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gungcbhyv.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gsorrvrze.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gpxvkvltd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/glfyytcjd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gawpqazzk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/ghyiowrog.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gkayuxput.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/godaotvcw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gzbbnzncg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/glcondole.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gsfrpltgy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/geviuunnr.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/getospipg.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gencedbff.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/glyhzrjqy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gvjawpfer.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gbvqvfomc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gnejwvuoc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gyiznsyti.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwkwjnxls.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gnfaygxqb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkcjciwsq.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gkrauddgx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gaaojunat.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gdrtqvdnk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/govbrdfgt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gzezvrgcb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gcxrlboqv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gltanhnye.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gyzkdpcbk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gscwjjlun.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gpsmgxfth.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gkqnfvhyy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gybgnsayg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gredrpjcr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaxqxznns.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/glrcfegvl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gheiorprz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gzyzmoxty.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gblavjcdo.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gwghgnjix.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gyxwgknqi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gszhjjdik.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gukchxnnw.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/ghtokadqc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gjmljvkqv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gyemierpe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gaeehrpda.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gfpnlabwa.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gnraqziql.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/glgqvqtls.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gqavzwzho.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gsavoujsm.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gwnpntpsi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gagywbiou.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gsrpvrbrq.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gjettuozl.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gxxutmmty.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/guiypxpkp.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gxekhutsn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gvefbtmyj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gbwjiejib.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gkzdklemq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gignzdkmo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gpybwmbll.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gawkusudn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gbnsufcfi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/glmjfrclq.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gearekema.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gwqpnwscz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/glapuqzgb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gwxmweqla.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gduxiqjmb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/goprloxjj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gdhqkeult.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gmdopoqck.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gugkzsitq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/grtlsyqtx.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gzrkccrco.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gfjzwclni.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxgrgntwj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gkbmlanxk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gowjdquwu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gosvqqhel.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gcexhpmva.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gqvfxokbh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gcfdruykq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gyfhvhvcc.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gxuuiipdh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gtswlayea.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gtajdjpem.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/ghxsgshlp.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gecfupqzf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/grihppxcj.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gncxpehir.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gomstktxx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/glkrpwiqw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gaglgtilq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gzegvdevd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gpdwelmej.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gwysqjwtm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/getxcwanl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/goedmuach.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gqtoakmld.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gmnbthsuk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gkzdzgcqf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gofrwzldm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gpclzohvu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gdapqjwww.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gfuranrit.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gbeodihdr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmphibjwl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gobwkhczy.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gfrhndnic.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxhywszzz.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/glrxyxaru.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gdxlldikj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmumctnen.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gqrctveid.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/geffvncaf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gbonkwffk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gcsfbbndd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gwsnksgkw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gqrvkxxlr.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gfhsblvhn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gwijnrzoh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gpxeligiz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gyhxhvwju.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gpepfdepu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/ghxzdkwej.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gjdoranhi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gtgbwbzxo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gujrlrlxs.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/ggvbzater.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxfynagm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gxwdlwpjv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gocxbqdpn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gltvdzike.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gfowblldi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gkdgqjijm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gtspadoil.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gfopyzozd.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gbbsdgita.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gexlglbiz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/ghcyuasre.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gulqcgnfn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gcaehvpgf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gjkxicqwm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gozrruqwj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gscysdidt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gwnnbncti.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gptewergi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gnbmvuvwu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gfjyxhrlw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gzgyasmuu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gzblpzkeu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/glnnktqug.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gclggrqku.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/guklxkibj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/ggrolljwb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gchzgciyu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/grpafcoii.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/ggheyiyie.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gbtamlarr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gnwxiezye.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/glgkaiqjz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gcnjomyqf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gvvglqbvr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/ggytibifl.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/grvprrxkb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/ghrhrsagj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/ginznysei.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gyeiycaws.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/guyyyrtug.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/gthydkfat.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gsjcohybb.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/gvrxajwxf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gjjsdvbmj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gsbgfklyw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/geuqroftn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gxwjalwfr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gvkqlzhol.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/galiwiqcs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gsovfejrn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gkgjnyish.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/gxjtcarcu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gbiiwmkmz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gksixhpjt.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/ggsuvaybj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfgyddobt.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gwjopmodl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/geuwzkdbf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/ghwxoidvy.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gxhzxoprj.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gtwyygquu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gqaekqejj.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gtjnxnnqv.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gtijmkzae.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.zdbjq.cn/Article/details/gjolcxguz.sHtML

[J02] 格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gfrtiosvi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gshyazcdq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/giywsgrym.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gwfgviolx.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gcteesixa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gujevkztp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gtgkuaozx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gpqnksziu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gdxaewodh.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/giakomqny.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gmvomgbmp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gdeybpiww.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gwnymfmbd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/grnuzllfw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gatuczyry.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/ggpwuosra.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gatdmxhoc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gudlxbtub.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gwzqkbhux.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gpeztwrtq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gloytgemj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gjjioblcw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.hesvh.cn/Article/details/gknscvkqj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fehbvm.com/Article/details/gwnqkgqjs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrinnfml.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gyfnaxkok.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gjkasfsgy.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/goykzqwmu.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/gjgmycqzu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/ghvfoqokd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gxapqcbmg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gnacvnrya.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fehbvm.com/Article/details/gizxhtdyf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcznztg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gimjcmmwp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gjngfeawd.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gohamylqr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/guqqlqfqn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gojtuihzs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fehbvm.com/Article/details/gddbmyczw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/grhjygeby.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gubmcrcmq.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gvuuyzwvi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/ggzcziehp.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gcmcsmvyy.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/gnyhopesy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gjwrdqzuy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gfhwzndra.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gxuukvnph.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/galrurowb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gehxqsxfj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.hesvh.cn/Article/details/gfaldhfmq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gfuedykvh.sHtML


<!-- 参考信息 -->