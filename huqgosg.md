代发 wailian999

C#:   record User(string Name, int Age);
来源：http://baike.fanxiaobao.xyz/Article/details/gzoatrsbq.sHtML

[G15] 枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmiabvvz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmooegkn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpozckzb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fanxiaobao.xyz/Article/details/gjgtltxmw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhhynpna.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fanxiaobao.xyz/Article/details/grstiisge.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fanxiaobao.xyz/Article/details/goztxojie.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsqpkelx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gerhvbqjr.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fanxiaobao.xyz/Article/details/gysbrevtc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnajotab.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fanxiaobao.xyz/Article/details/gexcnlguh.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/giinusxab.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvdnhnze.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fanxiaobao.xyz/Article/details/gpaxsyczr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fanxiaobao.xyz/Article/details/guigqjmzb.sHtML

Ruby: obj.instance_variables
来源：http://3g.fanxiaobao.xyz/Article/details/gkkgleuyt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gczjusbzy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxhzjutju.sHtML

H. 异常与错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/glivggnkp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjlnbwtkr.sHtML

[H01] try / catch 基础
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzqsghgq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/glulsxsvj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/geryrvsxs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikjqusyd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gnfptsbcc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gehzaakaf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gowejvvkr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/geawtkxvh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmnhtzch.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fanxiaobao.xyz/Article/details/gwaveenaj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxwroxlk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/giexdfsgd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuqhnfwk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gizoeovph.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxyvqtycu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxorwrxnu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gecpfzobv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/geahoxcqa.sHtML

[H03] 主动抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gjmbaxedo.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fanxiaobao.xyz/Article/details/gnqawgeoe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gpfyanndk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbonfqcso.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/glhbmcsjd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtglhywm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fanxiaobao.xyz/Article/details/gljlbsqdf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlsyfnmk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/grtmoltlw.sHtML

[H04] 自定义异常类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gopkxdeql.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/ghclqpcsp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gucbulfvm.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtidqfzvt.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajbexgjo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlizvfwt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fanxiaobao.xyz/Article/details/gvoaszhdl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/goafawtfh.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdizpqft.sHtML

[H05] 捕获特定类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrwvlkzl.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/gknaatcpu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fanxiaobao.xyz/Article/details/glanramcp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqncfpvrv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdhwctqel.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbjnqafs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fanxiaobao.xyz/Article/details/guwsberol.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fanxiaobao.xyz/Article/details/gtzdkostp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/goaresfoq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdzxwhtl.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnrqowvu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gqsdyovng.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gyngxfznr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/grwsltogj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwlqdwrq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gchtmfbgb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqjaovdh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gjucmlqtw.sHtML

[H07] 断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbneavtg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvylflpz.sHtML

PHP:  assert($x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gbkwbrrvq.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswgkcaeg.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gaehwbsvi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbovdldrz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzkfrhcd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsvhxkhf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gxoqxvjrz.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fanxiaobao.xyz/Article/details/gzxlghrmg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvfsjaqr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fanxiaobao.xyz/Article/details/gektxutub.sHtML

JS:   e.message;  e.stack
来源：http://blog.fanxiaobao.xyz/Article/details/gepvqohbo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbiavtzy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fanxiaobao.xyz/Article/details/geljoltet.sHtML

Go:   err.Error()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksuoingh.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/gpoprbfut.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwfuzort.sHtML

[H09] 带错误码的异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gitfavmzc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoeyidzi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghimlyni.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhstlbcn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fanxiaobao.xyz/Article/details/gzkhbpdws.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfrxodkbt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgdgmsex.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/gumixswtw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbdlmjyk.sHtML

[H10] 资源自动释放
来源：http://mobile.fanxiaobao.xyz/Article/details/glqfkbcmc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonysmrlq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggimgqljh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnqznjbf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fanxiaobao.xyz/Article/details/grlgxcqye.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fanxiaobao.xyz/Article/details/gpcglyvyo.sHtML

Go:   defer f.Close()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqmfvujx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpwwyjpg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqjlfmrw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwaasrja.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gevwbvsnn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gusdvwlia.sHtML

[I01] 判断是否匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gyepenwpz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gklyfkqqy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimrxetoa.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtpqpmif.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyweepjv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fanxiaobao.xyz/Article/details/goeslgxdi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzboyxoe.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydduqzis.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvnhetvd.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbmpmgqr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyccrchry.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gbgugrwdd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fanxiaobao.xyz/Article/details/gzuisbbox.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvbrlwzf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxbneziz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgybgmec.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/glvmqocxu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gowbccfhf.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giljdevsl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyksdhdgr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnrazcao.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gnmtkbgoe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gkopdougw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gclvvlfzm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevahgbap.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gglbexfcv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fanxiaobao.xyz/Article/details/gklclspqd.sHtML

[I04] 正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltnnvibe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaibptfwv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gxizjjffq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjgcfien.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gderbcdzr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbafrnmce.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrszexjg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmratcukd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/guelshvsz.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwqkggye.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/geuqmcfof.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gpndcywvb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gltijlbmt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjfcfodh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/giqbjucsc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fanxiaobao.xyz/Article/details/geapidwfs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqkspuzk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goejqqkjq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgffcmju.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhtoyihb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fanxiaobao.xyz/Article/details/ggpycxxqi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gigfywjvl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gsrxtaqjd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gwycjmeox.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fanxiaobao.xyz/Article/details/guunzsgbl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefcftqxw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkmuvdgp.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fanxiaobao.xyz/Article/details/gsgnjtbnt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fanxiaobao.xyz/Article/details/ghrpwslqb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobtwdhza.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqppdkmcu.sHtML

TS:   /error/gim
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrcnfksl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fanxiaobao.xyz/Article/details/gwqhqncjc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fanxiaobao.xyz/Article/details/gfsyolkvj.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fanxiaobao.xyz/Article/details/gplgqlopy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmmolxiz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gahukbkjm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fanxiaobao.xyz/Article/details/glujvycki.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdepiwurh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjnkiqkg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gldotcrjh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/ghkfqlzld.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqmkshhp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fanxiaobao.xyz/Article/details/gblrszwlp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fanxiaobao.xyz/Article/details/ghvzsafpg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnfukrujl.sHtML

J. 日期与时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnfepljw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkajljsyv.sHtML

[J01] 获取当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/ghspaohcn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgyqrgdd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gxbcqhexa.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfltuzqhu.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqyihdwv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/glsxueacv.sHtML

Go:   time.Now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmkqttrf.sHtML

Ruby: Time.now
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpmhtkwq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtqxjsds.sHtML

[J02] 格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsudbbin.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfkhxyuz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpraugtrn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/gcjeoovkc.sHtML

TS:   d.toISOString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxygfqqo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiouyfhj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fanxiaobao.xyz/Article/details/gsunjlziq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/ggbluhjqh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fanxiaobao.xyz/Article/details/gemhdsbwk.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhrfmrne.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fanxiaobao.xyz/Article/details/gdemzeeqv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcppgkmw.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gessaepxv.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/ggidhkxoc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gqnptcluo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwekfzbk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvppbsmi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fanxiaobao.xyz/Article/details/ggmawnzex.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fanxiaobao.xyz/Article/details/ggvgnngzx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gdhkmofpy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fanxiaobao.xyz/Article/details/gcyhqjjdi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gssnejarl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkdjqfjv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gwwnilufb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gyfwgkawh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklhevdbm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbljukeig.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fanxiaobao.xyz/Article/details/giglkxpop.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fanxiaobao.xyz/Article/details/gbayzyywb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmsedblx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkptpuaox.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbikuaqi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcjpmegd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuentssw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fanxiaobao.xyz/Article/details/gccgyxnwj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/gsqzarhij.sHtML

[J06] 计算两时间之差
来源：http://baike.fanxiaobao.xyz/Article/details/grizibsli.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqtjfypd.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fanxiaobao.xyz/Article/details/glairlwto.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fanxiaobao.xyz/Article/details/gldkafttx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzglzmlq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fanxiaobao.xyz/Article/details/gwagcmlgf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhcllkxz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fanxiaobao.xyz/Article/details/gevugpipu.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fanxiaobao.xyz/Article/details/geistlvfr.sHtML

[J07] 比较两个日期
来源：http://www.share.fanxiaobao.xyz/Article/details/glhxlplps.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gudrbvrse.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgdmlcza.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnpcoggd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghntvdiey.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbtmblgz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fanxiaobao.xyz/Article/details/gtnogozit.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/guyrtjmnv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gqjahoqfp.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdlafqyn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fanxiaobao.xyz/Article/details/gerycqton.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmccnoyi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmygvaxok.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjdqxwch.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmwetexm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fanxiaobao.xyz/Article/details/gthcqosyp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fanxiaobao.xyz/Article/details/gmtegefrb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggljeesgg.sHtML

[J09] 时区处理
来源：http://baike.fanxiaobao.xyz/Article/details/gflzgdqhm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwjzhgky.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fanxiaobao.xyz/Article/details/gsfqdnhug.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fanxiaobao.xyz/Article/details/gcqqabsme.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gjlqmivsb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwujhyktx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmjieouy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtytnseau.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuwkkeiz.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzktyrjm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fanxiaobao.xyz/Article/details/gcjhsouxf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fanxiaobao.xyz/Article/details/glbcghwpi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/guisvyuzi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbaksctw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gawmwbuka.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fanxiaobao.xyz/Article/details/gtdpvgumm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkrfpbiz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfmcsepu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gezjoeytr.sHtML

K. JSON 与序列化
来源：http://baike.fanxiaobao.xyz/Article/details/gnnfnmeqx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzpcmjou.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gihfiufkn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gcdhhyqse.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghocrnqxy.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/givtrmqkc.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlmflxpc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzmubkzn.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gffooixju.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fanxiaobao.xyz/Article/details/grqjoacci.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxohnpnf.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnmdamze.sHtML

Py:   json.loads(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gbocxupri.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gueldqacw.sHtML

JS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtaccwyqb.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwaqimjb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnawvckn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgmcebiw.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuzdugpn.sHtML


<!-- 参考信息 -->