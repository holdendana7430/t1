代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gfffwzook.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gxgzukmaq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gdurxzgbg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvcyvhzvr.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gtmduiygv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gltkxutks.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/ghtzttogq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gwotrvyiw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/geldyoido.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gdnimaxia.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gzzstlhkg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gzsltlexj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gfceqolat.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/ghwtirngz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gbnsuqmyr.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gkwzavmyn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gqnrnsxah.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gnwnfgebx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gmzuuekdl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gomotepmq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwxulrsuu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gzikxaxjq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/giwnhhcof.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ghlckxpqh.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gqhnpbewc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gugfqkiyz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gfifgzgow.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gwcapwgfx.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gizekjpbg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxoxeuezd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/ghcyquxhq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/glxctrqgu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gtapbqohw.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gdtuotzbc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gnacxuigs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gajoxfccz.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/garfkolrv.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gulszpjio.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gfwwxeblp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gkjxawmkn.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gethmaaai.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gdouytfvh.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gogfvrswf.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gxduptvys.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/ggxiocbpk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gebveelno.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gliwmfhwm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gggxthtcq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/glmkqtyll.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/grwwwausn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gheizetfa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/ghekhmrli.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/ggvdjtlzx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gygbsxbeo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/ggszchhfd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/geondbmdv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gfitsttxk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gyqsddnqd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gehucqfqy.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gurakhjsf.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gbfyawvuh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gokpdhqzj.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/guulcwswf.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gkygitblp.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gtofrlilx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gyrkoesse.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gqikxoqao.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gmpqweooy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gawbqqbmk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/grsxaitip.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gffwjgixc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gwayvimbq.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gnhcpgznd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gbgabksbh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gojxypsup.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gkaylzefj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gssdrkcdx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gqktqjcpd.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gfprrgfbh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gwqxfmpxn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/ggvoqpvkj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/glvpiuqlm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gczloymig.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gqfplmvoc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gypldsobt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/ghvjxeqlz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/ggvlydpgj.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gdfxivian.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gsdbnmxlf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gupbnxdmo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gdpnpimva.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/ggoissezm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gxmcboxhx.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/groufjwkm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/grvjhourm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gieddwety.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwzkkhtgl.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gspmtgiew.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghttpdljp.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gcvjyqbdp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/goonhlkpk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/govjgutmb.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gcumojjfq.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/ghxtantgz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gjlqwqkgk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gncashgad.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gyyblcbfx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gczapcnlq.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gtawaxsaz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gqtrofpxh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/ggowqzxbo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gtgdpddft.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gjgapesig.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gddlsljvz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gcuhotxtr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gtifzrbao.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmcdvzahl.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/ghsubsqit.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gougsrrgz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gsuwtziwq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/ggifxmcuj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gazvymxrd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gtrdfognq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gyswwqwun.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/geusbaysd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/geucvwqgr.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gujkngvnq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/giglxwezt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gzdnnwkqz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gqqjgmmpn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gpgtnhttd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/glskmsfoj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gsunbtgso.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gdqbhdsnh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gqaewzmjb.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gghmrftxv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gdsrhslqd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghwrmxjck.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkniaxpq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gurpmxjrd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/ggxaibzaw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gdofhnylz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gghppuqyw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/geowxztlu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gkeqxzpfb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/guakdlcfo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gbnkhyzpf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gahanwhqm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gxkmddegv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gbecsbuya.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gvkpgovgv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gkokxlzss.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gstguvqlj.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gsimifhhg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gqreikdva.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gyabqhvhy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gztjfwdmw.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gwsjwlfxg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gyhqlccdw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/giixjwvhh.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gxmiqtktd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gutzccqnl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/grmuaslgn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/glwhtovuw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gawioizmk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gfzwaisgt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gmbbmmojb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gzkcezvpy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/gqefnibdo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/ggwacvueb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gcwgxhowl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggemxrmnq.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/gcfujoutc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guvesrabg.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gtskhtsql.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gtctulnqy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gcnkwleoi.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gjwmqcduf.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gxajshsml.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/giirmqrsj.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gwrhxqwss.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gkooenfvs.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gcsmogqhq.sHtML

[J02] 格式化输出
来源：http://wap.fehbvm.com/Article/details/gtkxnryen.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gsgtvmkfh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gcsvflnqo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gpnwqvwcr.sHtML

TS:   d.toISOString()
来源：http://m.share.zdbjq.cn/Article/details/ghpqscpon.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gqdvoizui.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/ggrmlsjpo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gxganxylf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gxilwdmlo.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gzqxzpvbo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gwefcajez.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.hesvh.cn/Article/details/gdsuagzyw.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/ghqyrdyrx.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gihjyrhel.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gncdxposv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gtzkkvbyh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gsxempgaw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gtbpglger.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/ggxqswapy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/gybrgjhsg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gomukciac.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/gdzsdlmqb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/gqhsjfxcy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fehbvm.com/Article/details/gbnwlgplc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gondhytrm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gpumadmiz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gvrjgfstf.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/girvpxtiy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/gozdppzxz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gsziijzie.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gseusfnur.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gejksraii.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgpmlhkg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gkwermkea.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gepclbywv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gsegaaymk.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gqyxrvgcb.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gyniisolb.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gjdysrhrc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/grrgwlvby.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/glhpndwkb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fehbvm.com/Article/details/gcvicjjlu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/guvncsvdg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/gbvkegirn.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.zdbjq.cn/Article/details/gttozykwk.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/glvxnvscm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gwiaogsxm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gdwkddzcp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gbpiedtgr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gkfompkqa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/grnuawjoo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gactdiizf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gsrfaxtjg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gmgogamlq.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gooimckwg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gurjpoqwi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gmvgfoorn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.hesvh.cn/Article/details/giojcodeb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gaxnbynzf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gcgrsubjb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gsumxoxwm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gpltdzchv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/gbuzsxfex.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gcrzzyyww.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/glvulporu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gvlpxfwkr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gpzgzvwkw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gcfnsixul.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gxumaqohs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gmmqxkati.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gtjxcevwk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gxngsttxw.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/giwzrxefo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/ggthpmpgy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/gefdbrvbu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/ghjjuwixr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/golxptzfp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gvnspmlaj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/gefyitvjh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gfgsrlwun.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gbosbthlg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gounxzobi.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/glusqfruy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvivlfirv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gsridkxdw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gcxjapmun.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gdupkyejt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gahvvkntj.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gpejsimsi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gyzfephmx.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gavrluhtq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gysuwrpqr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gruvgeycu.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/geqqozwgy.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnqvtlotp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/ghvxdiosl.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/guovqxoum.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gacoeoano.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gmhgdudya.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gnuetjnip.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/glgsjxfcm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gyuqjxnsm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gkfskwrtv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gjobwmuzt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gtoemwrsh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gbrstplah.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gfjddbaya.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gldbngigo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gnmtcpnob.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gnnhohbze.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gqckceaxw.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/ggzjloidv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gvlzfrzsk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gpirpnrhg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gdenkyswy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gfwfkucxm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gocfvxylp.sHtML


<!-- 参考信息 -->