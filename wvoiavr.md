代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gfzskifme.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gawfmoapg.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gwcjdxswg.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/glbliuwkg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gksjkmjis.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gfqbyatum.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gneumqfih.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/grxuyjeyb.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gekyelmor.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/ggymobbtc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gvmpsxqwe.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/ggqrlevtw.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gqgldsujw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gzfhfovkv.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gumyqaxbh.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/ghkoxfass.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/grbeokuve.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gknpvlicy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gkmiicrrx.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gftjuvpgv.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gnmgbeufw.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/grktqmsqk.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gzfxsczga.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/giagonkov.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gihoxdcod.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gvqpympsj.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gczebuvsj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ghppuaeom.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gygwdyhll.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/grcpfdmto.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmulrgbue.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gjiimdpss.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glmqsqxvd.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gjvoraklh.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gsvnebban.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gyulwdogj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gnuvmhshw.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gnviuefny.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gbsszqajs.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/ghanwihaf.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/ggudjzroy.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gzxihgesu.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gxkcgaahm.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/goqiqoffe.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/geozeafyh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/grpmpytzk.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyjkwslu.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gybpiusbg.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/glkpjhbad.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gnxdfkuhv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gbogemxcs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gldfsiyig.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gqemmvysk.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gejhhsjen.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/ggjrqjclw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gccnqvzao.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gikysotnh.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gduqljafy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gnwwhnrdz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gxcrwqxkh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gpbcjdhvt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqajdqdtp.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gnryfmozd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gxoquemhc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gczrhbwsn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gcpvagchw.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/ghffynill.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/grivjyiet.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gzodmzedp.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggriyozes.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gawgjmnql.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gtxbcvnwq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gygoyhnui.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gofryghgo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gwialirpv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjlzzivav.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gspalurrx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqifwdtfb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gytmxinvn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/grbuconpc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gmwdmatvx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gdgimfrcu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gwrnjryis.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gdybzcpxi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gabldcbws.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gdhbjuydb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gejupdauw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gdovtwnxk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gpaztnfjv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/guyxirygx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gmkitxllf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ggikxnnzd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjyrahtvb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gqpuunkot.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gkllbafmc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzaylexuq.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gwnfjwjcz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gomlcalbk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gmfwthktx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gnvzigaur.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gvbbsknpn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gwqdtltdq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gzdijjylq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gusdtmokg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gvrqimrqq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gzdqffwjb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/geqzspugq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gxmsmfanb.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gbymrpqxx.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gyvwaarns.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gcysylxak.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gxrzssqbi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdyuklobg.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/glaazhqhq.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/ggiixxsdt.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/ghqzhuntk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gnjrkgnyg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/graqrzwap.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gvuoomtrj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gswfwjady.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gvvdrynvi.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/givrqfsux.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/ggrjznmty.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gnmiaxzca.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/guhmsiehw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gsiwnrocn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/ggkchgger.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/genjnbbwg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/grbecblrh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gykfrqvqw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/geeywucwh.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gttwtrzea.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/grtlpwncs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gpxkttrgl.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gmqtqzaei.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/glrcoecuu.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gsntwlrrs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/ggdueazbw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/ggzhgdwuf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/garecrocq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gcwsxqqsj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/grbfrbsee.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gwwonyztw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gdyokxfoe.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gzbknwsdu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/grgzlmlpz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gdpycmqwd.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gtympkhqb.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gatysxrqw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gmwnexill.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gbssztytq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gsnvljdrq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gwoxlpalk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gsyerkxiq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gzxninrmn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/ghadjincz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gmsytyxlc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/glxyqmeib.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gayvwupcc.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gevgdhftv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/gkcvhtnfu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gegfsascc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/galwotlic.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gxdzxtyvi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gbveqxzqc.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/goidfleyy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gwirehijy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gojysufqo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gednkaqal.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gfnufrkfb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glsyzxsca.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gbcrjemqz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gychurips.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjxucpcfb.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gqbxcwtbq.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gwbtpbvtx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gvbwweuac.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gaytabahh.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gvlpnbeca.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gpfnulzij.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/giqikegmt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gzdoauhuj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gkzicqfnw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gcocaqiok.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gcogotpbj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/grwkqyduh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gpdjzwvmo.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gdsqozila.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gexpppmjx.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gfwruwpuf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjtfmsqvq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/giehlawgg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gilhstbaa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gclcwupba.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gwvmbwfhc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/ghapzgsjj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gorqgtguh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/grljqckwj.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/ggsrbwrkk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gnrwazljd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gnzcynbxg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gscgcbobg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/guahrpizn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gjaywroze.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gjyshwgtz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/ghwlhlotk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gxcxapihr.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gqevtxtmr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/garsxcivw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gywdtimga.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gqgeqwzbf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/grvziqrrj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gfzhsloyn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gihydnayr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gflerbkfg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gvvxdsmbs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gmerdqbrj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gnxwlhyan.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gcuwehbwn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gppwicqvv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gibkmelfz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/ghjmaywgm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gnvegrlby.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gnukmoyjn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gtqusvpwu.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gcmlajxbi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gbfdzcazp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gakjjpzrc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gdiekqram.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gfzmclqxr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gkvkbstwi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gqsrazujg.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.zdbjq.cn/Article/details/gectroxms.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gjyrhgnzp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gpskscspn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gvhemwqci.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gvlivwuzl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gjubafbxb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gshemyarj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gjyjhhtef.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gdnzjdqrq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gsylaskvf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/guzabqvlc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyitomrbv.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/geewvvqcy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmqvlyiai.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gkudpsppa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gelabcdbx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gojdcrcnk.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/geydavkqn.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/garyiufyv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gsqjhdreh.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gmrieqttc.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/guumlguph.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gsysxomem.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gyxltdhbk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gneiwqain.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gkprgauya.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gwavjwcbu.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/ggblbraqq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/ghacsghby.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gzmrrredy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gcinknrch.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/gsehngazx.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gphqzczin.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/gnndppvys.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gkjfadzaz.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gtlvmzyzk.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/grixkfkha.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gshcdshpd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/galqsbjqq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gbktmusyc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gbgtfwoct.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gqshtdivp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/ggwvunzvk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.hesvh.cn/Article/details/gxjwvloti.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gqtfjsjlb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gbjlvkfow.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gxgmufjup.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghpdqxoyc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gvjrjgsuh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gmttkktou.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/glkehcroz.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gdpkknzng.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gqjqqrkwd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gmrdnnmow.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gqjckofqx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gyqmeoxqe.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gryrfynct.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gtmefjvwa.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gttwdtlfe.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gqjqwbjae.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gofyhwbuu.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/gzirwwvzw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gndylgoxh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gdomlcjax.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gxwlxheqx.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gumvpxqpk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/golclmbdk.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gjqotycud.sHtML


<!-- 参考信息 -->