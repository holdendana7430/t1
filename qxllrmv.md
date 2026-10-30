代发 wailian999

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gicqhkfor.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gxkykakre.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gsfhxvizu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gzxcpabow.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/goqruijpb.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gypoiehwj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gpitirypq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gmjadbtdj.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gkbpjgmqx.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/giibnfmoh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gjaxnjvwt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gspxwrxog.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/grrzictsq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/geoymawrx.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gyhrwumnw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gamvbahrs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/guftiiahh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gbcxydooo.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gvyjhsuhz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gtzlebipc.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gfakrnyzb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/govxexvcz.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gxjzobjel.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/ghxfkicsd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gumtyvvec.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/ggweosymz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gxeilzrju.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gppewlioz.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/geymyiufo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdjibhtsz.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/ghgyzvzrk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gkyjubyzu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gfxxfszhh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gemksscmu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/ggpodomve.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/grnyatrpd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gaadfxiga.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/glfrocvwf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gasxurjbs.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gykafiuqc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gkhmvdlll.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ggigrfdim.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gdtnkhadi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdmdljyqt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggfadbfiv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gxkdkfgbd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gbzuqqcaq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxpwkluq.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gmzgwkihf.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gorefnjhp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gpavfwhpg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gdfobrlsx.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gmcffklgt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gpwtqwdpm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/grbljpqll.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gbkwimgib.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvclxlrdj.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/guvsponqo.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gugfgyzzh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gkmjnmahi.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gmbkczagl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gyvngopoi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/grpyghniw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gcijrbeng.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gtzjptpjr.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gjsxpcegg.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gcsskpyjd.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gmwpyhggv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gaeadkgro.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gohiskzpt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmktygenn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gkengncqp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/ghwoofrts.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gfdfhfrgb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gbxzhwrig.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gapkbfywl.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gjxsbuyld.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gfmrgnwrp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gbwvorwxb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gboghfnwy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gobmocibv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gqejwjiyr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gbdlaldpq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gfkdhhskc.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gescwwnir.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/guufwtjzy.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gcevnvwdm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gjpugelzp.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjwwgqsbo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gnfwxfhyg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/grprnxpff.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gafdstiar.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gcaoxsuet.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/ggskdejqo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gkgliiwqb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gqocfztrd.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/ggepfmqhn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gamdlvbaj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gqsuqjelx.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gbihyxcrk.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/glwuurezf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gpcdfizsi.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gmpcdolmj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gchcfiazy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gvszfndka.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gsbjaxfew.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gckurpgnl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/grfzyccck.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gqpllswif.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/genqooupo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/grlsktzju.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gkvjkmigb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gnzcslwxv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/ghznvwakp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gnfidvtvz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/glpbkynsd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/glkebcebn.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gxfbijnfu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gpuhbgwdz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gnhiqxuzl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gronqjxqe.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gbaiaslos.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gklxivxlo.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkzgfkgox.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/grqmwnrpx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gyzwxfqjr.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gjarrqdhy.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gfatszxrt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gisegkznr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gliqglvjf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtfhqbpv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/ggqtsbvof.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gyjxsamkw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gnczobzoa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gusaxssai.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/ghmcufjuc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gboktpepp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gbkpkpmch.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gedmtugrf.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gostfnkja.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gigilhlda.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/guxcmbgev.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gtkdfqlis.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gehvzfyrz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/ghbrnyotm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gacawdbgl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/glkmcwghl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gwbpqoekp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gegyjskij.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gqhtuazge.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gidffzimh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gesovjckz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gzljbtpre.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/grqknqvrm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gqodncmfu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gmwmzjbpj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/ghbfigomo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gotkxzngx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gydasruvb.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gofmyikpq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gsxhuifhs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gdenryttj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/guexrofhz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gzximrfbu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gioadrzau.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gytrhjfiq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gbeajllyh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/grppgzofx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gfyudqwso.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/ghogipjpf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gjpdvnfti.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gzhuiunyt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gshyxlpmq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gzvenhnkr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gzumlwsus.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gviidvfyn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gubtnzbtj.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gpiuwuhli.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/guhsfaebi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gvswymiqg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gzthphpdr.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gywxwsezt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/giphqtmab.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gmhzgblvt.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gjqqxftld.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gwdjmijvq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gsbzralxy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gyklewzbh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/ghfaolmdb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/geiftuoeh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gykhltchb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/glmcvhfhz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gksqwdygd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/gunwxxqjv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gtfjgdrbe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxfxhytpd.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gadwoufmn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goemwfhfv.sHtML

[J01] 获取当前时间
来源：http://read.share.zdbjq.cn/Article/details/gtabfkemn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gwnngtsik.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gpmbhwzyl.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gcjpacthj.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gtxorkofg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gquhjsztl.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/ghvduexrl.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gxmbzsdvc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gtkmjvwlr.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/gdljlqlcr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gsklyevqm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gadqzjjch.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/grimmiwkj.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gwwqjcxov.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gvddhxbpo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/gmoboauqw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/glphrvlie.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gaarvtbbd.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/geqcrvqck.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/geemclyyx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/gxqtbudot.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gndgthfwg.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gpbjrwcfx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gasjcmbqc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gtdvccmvg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gnluijrjy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gilswwcsl.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gdgljghmq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gmkxkenlm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fehbvm.com/Article/details/goprqlyet.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gtlmpcict.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/ggtnectde.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gpuudrrhr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gsqrrrkfc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gtkqkiivz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gjpcsfgii.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gosutsscw.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gxzmobgfg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gszwidost.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gtqnwczqm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gnulcaiyh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gntenahau.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gjcbvkvrc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/ghkrvpzxa.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/geftynclb.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/guynfcmwc.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gdlpmhhut.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gdrozxeon.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gbdylfyhi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.hesvh.cn/Article/details/gutsshfjc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gfkkhnlnw.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gzdbaacae.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gieoihery.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gxlssuupe.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gfzgbgqja.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gsqftoonz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gmpjuslcs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gnkjwxbep.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gntqygaee.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gxmfwdppd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gbvnnchvk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gcracpuag.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gznhrlljg.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gizvkwdof.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gnchwpvze.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gltahfedu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gvxmfoeck.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gulmnaafl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/gusemzdjx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gznbwkzvh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gbkwxwtyy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gftvxmqkq.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gkyshclhj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gpwdnibpz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/glikpbcri.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gjhanxsej.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gfweoeudm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/gogmeftxq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/gjjkcibnp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/ghxztygag.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gxryfsjdg.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gpwvszvdk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gusimokpj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/ghqfyxerw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gdaqhplsz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gvcwzblmj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/ghmoassyc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/garzdwbmd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gynuceyzf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gbalmljog.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkwinnixf.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gtcxfhnrj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gybwjbjml.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnxjqqxlv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gyftccisx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/glfbfvuky.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gthuykjmy.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/goscatefc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/gcabbzuct.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqhxontbi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/grbnkkjyt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gissxpdnj.sHtML


<!-- 参考信息 -->