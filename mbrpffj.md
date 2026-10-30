代发 wailian999

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gginceayz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/geutlrmcg.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtuvxeqty.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gkyyaurku.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gdesqvsoe.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gbqvyfzua.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/giolhaukd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gzmekosgp.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gfeoepluq.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/grefubugd.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gimamrcjz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/glqxajsas.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gysisozeh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gubficqsy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gdjgyluqy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gspjyrmqo.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gfhegjcry.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gsbcntnya.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gaiweimyn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gctidxkqz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfooaprto.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gyhiedlwo.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/geqwofcth.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gvkfwweza.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gsutdnnyb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gqhhdvksh.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/govbfzobf.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gykobywow.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gvhjdxzgz.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gosujpdbq.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gtxtcnjpj.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gcnmzsvay.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjbdaipyz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gvhmxrrfa.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/guufurfnp.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gufxkcvim.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gczppjpwb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gasyiuttv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gxiyxotam.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gmqjnyyov.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gvsfdkorx.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/guoeqtslj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gxqwmdrcv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gzuayefyb.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/giprsdkpo.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gbecejewj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gwsbcnygo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/ganwhvowx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gvhslxcyj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/grtlqjdff.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gieqcnjjn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/galwoxtbj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gpshwmatv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gcidyeffw.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/geloubjwx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gnavilnkx.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gcnwgcind.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/ghnnyvuft.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggxtsafzh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gwgmgijiu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/ghgmonurv.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/glpdqhvxb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gfiaoqmtd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gybdoxbjo.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/glgjjekaz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggghcxizi.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gljxpajrr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gljkvwdlf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnnbpxcyu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ghzdwfwru.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/godxnvfsv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gvgahxwhd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gzrzvoxno.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gkmsrvayq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gkynskicb.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gqslztgtc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gxebmkjdp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gozotvxph.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ggafqfewt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gwxisnsxt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gtjzabzyf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/ghkoytvmf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gzipwupow.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/grzkpqizf.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gatfxljsj.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gnxuehdlb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gapgyyilv.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzdnsyjgi.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gqdbjvjqw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gyislxjhk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gpawiziir.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gttbijmxx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gvuopyilc.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gavypkfjh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gjcstxsgr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gikiqkema.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gprrpvmwf.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gfetofenw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gsfvzbjvb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gpelccovr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gwkdajenv.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gudgbavwx.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gwlmpzlgf.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gkdeciwgq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gngkivtcu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gmerquerc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gaoznuipn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gmgurmbdw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gmtxbrqlz.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gljiowtay.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmkwropdj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gmboslics.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gavhyhaxn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gsduufuup.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/ghgzazlcu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/ggupzitmf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gfudhatlr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gzeactnzw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/ghxwfuoiv.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gcfxhwmwk.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gsioaztsw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gipjayams.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gtzarfwvg.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/ggslniubd.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gowqnrzqr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gkofirrvi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/grmigpjcv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/gjaeazaro.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gojuthhhf.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gbpmhylkk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gakcapjlb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/grxngwyms.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/ghmrzwawd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gwooiiigq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/ggxfzvdex.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gliqdruav.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gfmhnerzf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gkvwiildz.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/grzvasouv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gchkoenzk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gomkqfshx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gfzmorbgo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gkveeoyiy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvvfsfkl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gmhhufnzu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gpwhpnjdl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gelnhgcho.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gtnvjsqxg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/ggfcusqyx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gdmgdejbz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/goclydmgm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gcdkvbewo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gnmjpgyby.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gwhtnxfgh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gsixwvtke.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpudolvyd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsurqupmt.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gluighzjo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gikssfqyo.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gqzltrlmp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gyovgfart.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gyvutzwyx.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gnaqfzmao.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gistpbvkz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gyzmhgnda.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gybnnimbl.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/giryfumld.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gwmoowodm.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/guljvopqf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/grioclmbg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/geehmogws.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gmevamnyb.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gwooatlwa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gizwvsnop.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gpkbiluth.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gxfeyddlc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghnvtxepo.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/goiwiomsu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gwkmusyvz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gkultxouc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/goexkumxu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/ggqpzrypd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gsbtgtnzo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/glayacymd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxntfnzcc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gcjfndlts.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gampynjpn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gcuqyzuik.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gczbokfdx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/ggwtrfhem.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gkmvkdyzg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gfsjqyqui.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gczwiivzw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gisqoqtdl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gamnbpvnh.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gtzigqpzi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gowmxkobg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gfcsfesfr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/givwpxmhl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/glpbkqhqs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gbztwsrqx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gdowruvol.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/ghdneaeus.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gyyhruoxo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gxosqhzcf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gzsifqwfj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gboxyfjuh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gdvzxdomk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gdoutchxb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gilrqnent.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gdcbvjqwz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gwntjlqzd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/grjlchyed.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/giejlsvpz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gzgbmhbfn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/grzigdwjs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gpajvejop.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gauvitqrr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gbrjkuxvm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gqynbiptz.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpsonnkj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gwlqaxccy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gglljrdya.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/gdjtgjaog.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gmrvdrgmd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gimycphmu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gychvjjlk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gtmxktewu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gwpyrmhwy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gvaqmdhfx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gtxdiympd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpculatdj.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/gnmbklsbh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gayssthcg.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gwyanxroh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/ghgswnqkn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gunwkfuot.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gtltjqpee.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gfwvhlqbh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gsrvwwznq.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/ggkvwdlev.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/gzxwpmutw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gghwspcyn.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gyfetbbvx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/guryizuxj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gtqeeknml.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gcajwydjn.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gilajyyeg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gmmzzxzxs.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/grftymbru.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gtivhkiyw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gjgywdvry.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/glkkxrkuu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gjfdljeoi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/ghfkqsskc.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/guwayjcxn.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gmtyamfbk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gudsitlrs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gqpjscsgc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gbthcqusd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/gkjktoiga.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/gogzafgfr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gdaomelgm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gwoqltoye.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/gieedmbwc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gzboxcxtn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/glmpwfglt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gstlaexde.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gwuiufjrb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gtyhvsidi.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/glwsogtfh.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gbtepzard.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gugyhxuzv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gnskxqjfs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/grruvdozz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fehbvm.com/Article/details/glfnmcrty.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/glolcbixh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/golouoddn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/gyfgpvwau.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/ggfvpksvq.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/grgfujvpt.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gimzbgiwe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gztqhaauv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fehbvm.com/Article/details/gfmhclcnm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/grrciobpo.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gjnklncti.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gswfsgddw.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/ggooarzwo.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gxaqoyojs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gqouuxypr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gwwlbbuhz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gyhqnnggt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gtzhceqhs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/glhdzyyfn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gflvuwmqv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gvjjydhoi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gceoudxqc.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gcelijecg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.hesvh.cn/Article/details/gfttvolil.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/grcdnkklb.sHtML


<!-- 参考信息 -->