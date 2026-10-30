代发 wailian999

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gqzbfnysu.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gcefollva.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gafvmicus.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gjvpqvktl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gncxlpltm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gqtfukeog.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/ggnawepvd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gczdknrnp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gzjnrbqzd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/geeewwple.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gexhowcim.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gwdpklmnc.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gvrmulzms.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gfhooadbg.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gltwexlcu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/ghjhafloe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gsdnzvwla.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gpaufbjcm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gzgxcnapo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghywqqzus.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/guhgwwvtq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwpoerbve.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/grzovfepm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gnrprfmro.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsrxfgwzq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/guxcxfdue.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gmcidylbb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gdouksuuy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gyquwgcdi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gvvsuquni.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gkqfpizgv.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gpqvwbtim.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gipvrbqsb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/giovegipk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gockmzjjw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gbsnqeejb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ghijytutz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/guioonmtb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gcsbgmsdt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gabhrlnsc.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/glartwzxr.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gvwuwajcb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnqdatfso.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gbwxcjebs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gwazspzyi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjtlpkjkn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gnbcjplnr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/ggretlluj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gkgwmqugy.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gonnligxm.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gauyizviw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gwutotdez.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/ghwazkyhe.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gdurypiqe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gdnnrdeme.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gvzbzprfg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gkfzrovnc.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gokiagedl.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/goopkreyo.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gzuwsqfrp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gttzhurzh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxkuynnik.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gtvxzjtfv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gxycrlunu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gykdungxa.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gkoowcagr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gzcbdihrf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gtzszjllz.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gwmwbwrqt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gwtbzpdnr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/giwywdfny.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/ggwcysjmk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/ghvdjftyq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdgsggln.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gkoezgkpy.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/ggkhoiaup.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gkijfoxcb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gvmdplyyu.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gtwvissyv.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gcetwnnxs.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gxtmnbwtv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gbitygswx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gxsoymkvl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/glaxagtcb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gpttwcmjy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/ggronlahz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/glhqyhriz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gnvkesdvh.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gowvvyezp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gziyxaxip.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gszlgdtoy.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gbrhtjdvh.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gjagxevac.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/glljnxnan.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gekcixidc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gtepuwqnc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gzbszacwb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gwuxhppwv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gtjlducka.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/goamonaxl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gwpuocghb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gaamtkkwg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/grtmhlwsq.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gsvkuqlqc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/gjzrzwhke.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gdfrmggae.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gzsfjojvk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/ggunbviic.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gyeupfayl.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/glptvtdwl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/ggkfwdbws.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqwyjbcll.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giiozqbpc.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gwgiadmvz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gldvbnhqg.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gqvupqonz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gsjpgybhg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/ghmbzxazu.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gtdtuqzan.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gjtcijrjy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gaqgssdki.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gcwpywxux.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gfbnzhaio.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gfinvxoyh.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gsoyojvdy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/geeuhghih.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/gefltlyxu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gdmmnakgo.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gbvopjhsz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gfyqiywxn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gvzxjyopy.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gqphoqrvr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gotckunkx.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gcjdlxbft.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gcjeasqje.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gznoyburi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gjaihwsbn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gogexvrhu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/grdafvxtv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gbixtiems.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/goasozomn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gtugzbjnk.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gqidziert.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gagjvzjgp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gzppgadde.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gvbqndmve.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gnqoceffl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gsudgryhr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/ghxarezkf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/goexfylcl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gdyfkhhas.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/geptkihyy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/guabrjjcr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/ggpchwcgx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gzehbohuy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gyyzemidb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gsjdrbmdn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/grumabsnj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gbiqqnwef.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/giewajdtb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gaidryssb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gnnmceynd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/goyufprxz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gvckxwhzz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gqxdkhuuf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gwpqjujwo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gkamtjmzj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/ghdeovttv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gmimuwizt.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gzlbmdpct.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/glnpsxnsa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gwevccbdj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gmdjtrvxf.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gztcgzuyq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gpcekqely.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gspxjeoor.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gttjyhbnx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gduljtcwl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/getttcovy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/garspgrhn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gcvbwdwko.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gkcgyrtne.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gjolmvzmp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gsbjlyyxa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/grpvzjozi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gctnrpaya.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gsfirdcgx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfcwjbfae.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/goizxgqwp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gixzkausn.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gkvvtmvje.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/gcgcmrfdw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gdyrsqfzb.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gexmqbjda.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gzqantmse.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gezovhxmo.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gukcnnegt.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gvrsrasuh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gpzilrvyr.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/gzpvkezbz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gwmmoxzub.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gdmgujwxo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/galnmywqw.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/gptwrfzmc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gojfstfwg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gymeclzwi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gojpsbgrb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gtridrlxn.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gzzdioizg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gckugxwyl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/grnwdvzgy.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/guwgydtus.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gflkpfaur.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gxeurbbjq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gtdpdxmbv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gekvofjoe.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gczuxrzzq.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gylniiymy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/gzmjkupev.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gofiqecbz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gvsivxhxp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/ghldftrrb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/goqvjkujs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghcodmpek.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gbdnpzdck.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gebjfrusz.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gejxvikhk.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gipsofxme.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gjimnbbce.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gxihbkfjv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gyzhjtvwr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gcdkpvqwg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/gzfbnntvy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/gvrcbjxek.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gfhwlvsdk.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/gnzrsczsa.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/gdppidycz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/ggvfhxlgy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/ganapmnjm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/grhcynmap.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gymyfcbol.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxbwyjay.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/ggyftndhh.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/geravtqpy.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gkvktswxo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gryjflxqa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gnirincez.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gojlfvhzt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gekufsvgd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gocfkflbc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/glteuqduf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gjkdxriup.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gefgxowei.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/ghaquaxze.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gkkesysxe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/glgsodafc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gtdavjeix.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gvzifkgpn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/goekmdpod.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gkqdeukkz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/gtkkirjfw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gtutzvage.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gjvippxiv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/gcejpmlzw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gumdqaylr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gryzfybbn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gvqtpnstb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/grlomivip.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/glfwdyrnf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gybzvwehh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gblbmhouu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gkvnkxsgw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gsfcigxei.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/goysapymx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gopvbzcco.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gxnameklx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gzhsgnhlc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/geajohnvr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gxvlaosrf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/grtpwwxbo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkfbiatfv.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gwktlfgjh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwhhtnpyr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcbkecgdc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/grnyogjah.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gtzywqaeg.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjnunsxxv.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/guakfiyek.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/grvdmhoad.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gmwecsqco.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/gjkmlwhlw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gfmkkyixw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gtjzunoak.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gzdmboyme.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gehsizfcl.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkemoaelk.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gcpgnmvwt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gozlrhevc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gflhqrxbf.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gpolyscjy.sHtML


<!-- 参考信息 -->