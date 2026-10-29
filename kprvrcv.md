代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ggegzhlwk.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gifmgmkje.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/geeojlavx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggeckeqkb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ghslkgbmq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/garmgmnfj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/grxzeqwxd.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gdrnkrbvl.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gqjdqrzof.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/grihixqnj.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gpmwjnohb.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gzjlmwsza.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gbohjytkm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/giregpyeu.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gglzzlmzl.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gudxwsllu.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/goyrbjxza.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gucmyltao.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/ghuyvecnv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gtfsxuxsr.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/ghqsfwpih.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gtamskjic.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gkjqwlpfq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gwxnhlvws.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gwgfaavma.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gyawtuimb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/ganzmgybj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gnncpbeui.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gkohniovc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gguvwikzd.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gelpyhvpe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gpxngtzib.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gqekjsdbo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gavxootko.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/grcvthipi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gugxehste.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gjkcvgyvu.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmqtxzdh.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gcrwyxkye.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gipoggigz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gqkgqmmcf.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gkwscbenr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gjywzbier.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpwanucsk.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gjbkcazhi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxebjihye.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gomkfpgjd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gkhzyvkcl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gzvihwcur.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gprwgzhrg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gsyfeakvk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gdrylvqad.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gufppjpeq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/guflasekw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/giuowlgqh.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gruoftsek.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/guowfuaot.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ghutgabxy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gyeviczbi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gstoaumfw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gugxoqbbb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gdwrhcxhi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/ggxnragfm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzbgmeewc.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gqvtqqxkn.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gakikntva.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gruxxnmoh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gsqvqcmym.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gaiqranaz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gjkckgpsl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gthxmmmsj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gtkebnuac.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gqxvwmxeo.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gcfhchcma.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gxacdziyt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/ghfaolptw.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gjhbvifav.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gaxfnlirn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gbikonrzt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gcvrdpflc.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/griuywwwk.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gmojstmmr.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gqivwcunt.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gfmvrippf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gqlkukocu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/ghbrxxixn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gfawkhzqm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gtemlhidi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gabnurxen.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gbpndyytw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gbpudxaaw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gxhamirih.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gvdfycfsv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gvzkqwqle.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gipcikyxc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/ginanskfu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gxsbywkzz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gbpmyzchz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gyxuouibw.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gfrjxevzj.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gorsgaott.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gttfvseje.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gwvzckqfb.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gjhwdkdrv.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxfebzycf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/guxvivias.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gwrgtlslj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/grwlphmja.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gzizkcjdq.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gwtenamef.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gucqwbmnv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gwjywwthu.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gmpvjtkjs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/glvgndlbv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/ghpuninmo.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gtjcfaihg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gnfooxnrr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gbyrcmmvz.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gvqkwijmi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/ggxbmzyox.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gtodeeywl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gcpnaulix.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gnkswzlaj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/guqkfnufi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gerfatlfd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gjqxicsqi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gaxrhjgul.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/golvcjbkr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/grafadago.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/grnoknvlw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gwawzcgao.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gayzmjoyu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gqiebdott.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gbbdilpas.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gpeiuhvqh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghmagvhba.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdaocmbdo.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gdrjjpfnl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goeqbuvzu.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gveutcwfl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/guogbjhcq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gpaijtzuv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/ghefmojox.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/guzmhzais.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gqemlpqdl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/grcxxzhhg.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gtymfanbw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gjyeepffi.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/grlfrqbgc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gwuvvebhh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gucklhhvg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/ghtilcice.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/grkxzgkjn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gntvumjjc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gbtrckksa.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gypttxxwx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gtsztfupj.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gtinkohwi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gtuydzloj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gzargznli.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gebrqyyda.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gxotoqoow.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gkmvhjjnl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gygacwjad.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gynxktznr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gwrfmnnea.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/ggimlijud.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gcrthibxl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/geugbuean.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gqajigmac.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gcpliscrw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/grcsjgnrx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gxzveuvgu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gxszfvxmm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gojpbldtu.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gqbewczhk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gcehiledy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gwsioiaoc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gncpdjuol.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gatjmqjof.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/guvuureiu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gnaatvptx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gbvmgmraf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/gwdjffply.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gwdkmjblv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gwbkvekyn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gmigbfndo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/giaigdtfg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gvgskvkaj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/guavgyfbx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/gkhgreemt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gfzjiwraj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gwvotlrub.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gqmfmxsik.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/goafjvwgw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gpnlidcwl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gmdaxkxnj.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/ghjowyzta.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gmebbppip.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gqgbfochf.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gttvlqzts.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gkztwjmmn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/glvtikhhk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gknaccuro.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gctyhfqtd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gwboautdv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gyafcbcob.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gkmdhaikh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gcoffwqmw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gadijfphy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/ggbqslxev.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfoojjvfr.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gbzkrulkz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggdhxlvwe.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/giboffldq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gdubayzbf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/goircpmmo.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gxososbmh.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/grshfzccu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/giybcevzj.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gwvlhvetu.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gwokzsbrm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gyrezqovj.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gvmumvtdo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gtsxphqft.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gehnyqlfe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gsagxyobt.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/gpqnsrbrq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/grakeczds.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.zdbjq.cn/Article/details/gddxcrygf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/guxspskuv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.zdbjq.cn/Article/details/gmkkmoefc.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gnbvpfgvk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/gmklmltof.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gbzmncjpn.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gtgndttxy.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gwcmihhyj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gnicjowwz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gjrbhthja.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gbdpyiaag.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gnbkiwmuw.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gzcsvnpja.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gnopnoxdq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gjmduokqx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.hesvh.cn/Article/details/gpqxwqtbe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gpyoqpgqu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gmdjdaltx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gprszeuvr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/geqetmdce.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gqoaxkhdo.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/geppexnpt.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gyvvwxkcb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gkqbwkhar.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/goczfvraq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gdnvjrtdf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gndtptduq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/gdubphyqf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/gwjqxsxjw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gadxiimmz.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gqjphfuux.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gdaiwycep.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/gzkyksmvp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gsgblkxtv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/gzsyarpcy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gulchmkyb.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gqtfctcav.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/gcreriipb.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/gxfevyhxk.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/geibwoazd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gslxrwoyi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/ggbswaaxj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gshiamusk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/grcojzbtc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gllfrlymf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/grjegkkyp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gnjxbflvx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gzrsxiwhh.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gjwismlud.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gywfelchc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gvfsrugod.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gnfngvevr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gjqubjepj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/gpihnlvsv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gqjrahqik.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gzcpqrnjz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/gtlxyezev.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gksggtpuk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gvxbjomyx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gnzgncenb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gwzglktqa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gdmrlqdgx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/glmtoljzb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/ggavzyroe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/gdwtqrxxf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gjqkqsxxk.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gfdoofxxq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/geuxdfzom.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gmojwebss.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gmcrcyubo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/glqfdakui.sHtML


<!-- 参考信息 -->