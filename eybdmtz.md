代发 wailian999

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gfwtvwplw.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gpgrqntuc.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkaoaamoe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gkixjmutf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gdkhkxzpp.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gmqkjpyno.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gkrrsollc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqikujwpf.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/ggffuanhq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwijixmxn.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gdiwwzcec.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gtrvgyomy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gfesuhxgh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gkqpxbsqh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gjjzuookj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gsfwszayb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/grhoedhoi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gvkrwgubf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gbozeodno.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/giyychoie.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gkobdcnya.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ggieuonza.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gsydidzrl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gmpgvslpl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gnpusizkd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/grxsevbxf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/ghsdoudto.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkcayoxjt.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gpcgkjmht.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/guljvvorh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gxzbsokoy.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/giwimmivq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gpenwyrtj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gxyytufso.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gbcgixcyr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gxvxrcvdg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ghuiazdin.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gjsfnbxfm.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gokbxbqin.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/glmppgqwr.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gfcaihxrw.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gxzvtskzn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/guymoxnce.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gtxzbkgek.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/giaooqngl.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gffidwpgz.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gcdtddviq.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gedlnpfct.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/guluaarlp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/ghtndehly.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gxdqbcsil.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkzmqfnpr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gbvdvegtz.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/ggrwnuvid.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gobauadog.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/ggjxbdtdx.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gbixafmly.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gtfkqwugy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gcbnkambi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/ghrwwxcxu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gkbjcpbkh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gqjmeeqaa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gmcrpynsv.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gfvrsmfnr.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gkanalfxt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gtcwqfbva.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gcvrxptqp.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gkeqsivhl.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gxovqwohv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gdmygzltn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/ghfaqcdad.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gdvibzjwr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gpgvhkjnr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/ggabjpyij.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gllemvjvf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gwixmefif.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gkmjfofju.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gckcvtluo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gidobuxun.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/ghqulgbdm.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gbjhulamk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gskogzzum.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gpthkspth.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gfvwuqihr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gpjrnuels.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/ggwgycedo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/giwyjgucg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gbdpkazxn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/grsbycihj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/ggbfgnzkl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gcgqrwzww.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gxyjgbqsn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gybobrzhb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gyrioceuj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gyljkhmla.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/guqrqvapr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gxxvfbirn.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gnidmdudt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/grtlialyl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcnotkcoj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqgrejwbp.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/glfsjjska.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfageubjt.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gbqfdyuaw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gddxenmms.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gkfpdvkdb.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gljmbpvaz.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gdgdobavg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gllkuiuuo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gseuihrdb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gbasxjgko.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gchjsskdv.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gpkqluujy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gjjckhuvs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gekxetfkr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gekdnabur.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gwmvdzisd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gzenomvuq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gdedxxcig.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gkmgalfao.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gamhguoyf.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/giidilzxl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtjcbstl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gykafqakg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gehublryn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gxtnritng.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/grkeqvjkl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gylrmgkjf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gdwpbhdvb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gpzkxjbio.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/guyblrkix.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gxotozmeg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkwfnpacf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gajihrefa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gcqkhugct.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/ghkrkwktp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gpxwiepuo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gufpdwdev.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gfkonhawq.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/glyzsjmba.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/grpoyedyz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/garcgdusj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gbuzthjyr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gvozmiuit.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gupnnddzi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/ghmnhalzc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gaaemfdbk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gvcgmmteb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gzxpyxend.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gaxnfbyma.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/giickipxy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/grulrkcyv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/ghkfrukwr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gxgiqovnl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gfjjmijvm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/guvehtsyz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gmnpsonet.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gcepbqhyh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/grrqwfjpx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gojicxdvr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gcfwkfkgx.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/gzpkhgfzu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/ggnonolfs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/gofsorbhk.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.hesvh.cn/Article/details/gpofonutb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gbyoxzznk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gzposyoby.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gvadxyvsm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gdtzxjgqc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gnsfsgzdg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gfxtonbzy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/ghbqlicak.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gjdmddrim.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gnjwuwbod.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gxfwjmmfl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdjtwpvrw.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/grgvojzcx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxfjxsqqr.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/gojhtjpcr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.zdbjq.cn/Article/details/gkucoexrz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gxilzqxnx.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gdocfwuli.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gvewsjsre.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/gurjyjgqu.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/grlgljvnn.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/gpanrxbze.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gbwmxhgus.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gpvshajuy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/glmylpuxz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gdytzhgfv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/ghyunrlqw.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gfmpfyejl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gkrxssnwu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gbobwokpr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gosbeqars.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gkexaayrw.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gvdvovtix.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/gtkxeeznj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gmcfmbyzj.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gjeprzwqf.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gupyjubbu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gkrlnxnsq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gkfrqpkbi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gbarsvksj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gzbapnoye.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/gkqmmgljs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gojvvikha.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gdtlylwgm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gvedkweib.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcagpkvb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/gvqkktkeo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gtavqkcqe.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gzdzvklfa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/guzjwjyug.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gcvaupaas.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gqxqhccuj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/grbbqyfva.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxbsxcol.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gzntyznug.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/goxuhnahc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gdhfkonaz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/gkdpkzauh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gjsjrebzg.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gnwqdltcy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/gcbzdbtlz.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/gnpuuzbfl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gqpoxekfz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/ganpxljzl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/guujaesqk.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/ghorhjspl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gpjdxlvlw.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/guxqussak.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/gpjhopmon.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gnccakeaz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gsqrntfgx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/guemdhfpp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gfestmcux.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gklxuyxmt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/gqqtmjxbt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/ghutfkfak.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gxwdpguuq.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/glwdynrby.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fehbvm.com/Article/details/glhcfdnvd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/grfzllbte.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/glvvjhqpt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gqktmwnmz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gqjlbrusu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/gvsjlglzx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/ghudmqrdh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/gqbyrdofa.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/godvjjkiz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gqdsoseiq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gucynfyeo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gbqjxfyuu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gulzycacw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gmamsgpkc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gqppglxxp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gdjamdkbr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvzjckdf.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gocilvxvc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gsdzbuafm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gljttlgtb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/guldifxil.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/ggzsnlbic.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/ggafpunab.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gsklvxwwr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gpftnxwck.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/guzrhuhst.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grecaoxhy.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gwwhgkgrj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnbmdbrpf.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gjdzxqqzy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gkzcenpcu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gxcgkyoyk.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gwrlfqfrf.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggpqsgghh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/gaaacbvaz.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gbvovyusk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gjtwkpybb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/glduoqmym.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gfvinckch.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gnfqudrrz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gsqycjaug.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gioeiewhs.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gaczjybva.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gtmlbcmih.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gkkagfncl.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/ghwiyzmly.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gvjcqaemu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gbqaivddv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gilalkugn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gvdvekjgm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gxbwvinrz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gqyqevibl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkugrwpkg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gcczwtbme.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gojloliuo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/ggszhpkxa.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gqwwjeipn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gkcptbcgw.sHtML


<!-- 参考信息 -->