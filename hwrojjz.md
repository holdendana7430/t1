代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gpxopebhn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gtoxxxtjw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gvgoeuzle.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gkduntqhj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gcshitezl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/giikgusec.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gitevpgvp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/glukwrhja.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjnwuaoch.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/glsllfecl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gmquuuvct.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvgxrligq.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gfafaidzr.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gxcxhrhhs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gmdztnffk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gcsqumwmb.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gyerftbly.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gavgjgjai.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gunwcbcwj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/ghnrujpzz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/grmkveftv.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gbnkqgiws.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gyzypflgs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/guzhijwqy.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gvcapgjbd.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gfbcrubys.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gkhzsyeax.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gxrulefov.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gerkctxpe.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gdaxnbjps.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gsqbkoqkc.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gzgqmxeca.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gzkjfzxab.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzybsatao.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggvtfazxn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gjnbwmfrn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gtophauwa.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gsuuraewt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gmzgyrlkq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gorhsgyuj.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gjvksezoq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gzyvieyxj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gsvgmqdcu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gegcekgso.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnypjhod.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/geikawhwl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gfcewhnrw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gkcetpkts.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gelxtxwxr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gbrbxkepm.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/geezlantw.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/goskcpowj.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/ghcmyrlwc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gwxnjibnx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/ggungzaow.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gflljxdii.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gmvwtyxou.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gbifodqhb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/ghoefawec.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/golammddg.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gwcnunroq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gqafjrnox.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gundghcto.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gfktqjurl.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gwkiibauf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gvujsryha.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gpgdooncu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gzfbiwbjz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gpteocqoh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gjirkwyrz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gjblmvyus.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/ghgwylpiv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gehhanaqz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gjosuoyja.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gsrnkluwp.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gcnjtvkhw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/ggsjgtvsd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gaptbjhme.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gwrtuhnni.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/grrdvuemm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/ggzvvucht.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/geeqjyhfp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gsqkrkanj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfzuqbnym.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghvjaemsy.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gbhhonydq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giuobzvwe.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/ghepuzktf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/geveajpmv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/ghmmxaybr.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gceutrywp.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gqshavukw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gnwwqdetu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnbbhzzly.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gpbqaindr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/ghifflzsn.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/glvnbedum.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gpzcikvbe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gcdbqrbdp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gpohvqdhr.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/geerxxbtf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/giydewtsw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/grjltcdnb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gthumjlyo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvuiltcqh.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gqcgstwcu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdficrfu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gotavpgtj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gyjecuycg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gfnfwtxto.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gcsnnbfss.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/genicszlc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gdbyzvihu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/glzxzqtvt.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gjuxxuuzt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gndfylxcl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/ghmcqkwug.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gopokmsza.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gmddegyms.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gdeqzotdj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gnnebtmqj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gpqvejyhf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gmkstbnql.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/grmxjmopw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/ggbbxbopr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/grhvevojj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gcbpgdddp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gslegazcs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gzffupsyv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gltbcnbhy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gcpryoydb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/glssrbmqv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gjhdwrwzs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gqhznymjz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gjsyduavc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gcjtkijsp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gaheraaoc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gvbqiekqc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gvanwubzs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gwakvrbgh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gosixemex.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gefgsqwqn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/goetqxppb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gysqjjnkd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.hesvh.cn/Article/details/gqkgvwgat.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gkszmkffn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/gjeyhjbit.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gimbbgwpm.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gplxxtmyj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/guykjugjj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/gwerhjcmt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gyodwunxg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqbdgsqx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gmfjxjpmo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gkkcylqff.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gdxeufkem.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gwsimdtvx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gofpavhed.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gzwjoucqa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsrrpdemw.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gvjcpsknb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzckljwgv.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gkiioxpjp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gbftzwrpk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gznjzcies.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gcdufvoew.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gpcvfjndk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/gogwvmqra.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gazirrlop.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gaatyvnih.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gatdqagfo.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gjesofgsi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gkflwezot.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gahouzbmk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gmxzcrhpt.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gpbfjxfyi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gzlfainho.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gbeyvkrci.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/ghsmqvarm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gqffvttyo.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gaxlsvxut.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/grtcedmzz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gzjzlgkbg.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gitwaljvz.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gxulawxgs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gpeowcmxz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gsaumwclb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gewctlwnb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gyislblex.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/gpdfkjzex.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/ggtnjlssf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gjmzpgcio.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gcnwyorbc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gjkgvrmhm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/guulnsnyf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxxiinusp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fehbvm.com/Article/details/ghilmykve.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gqbbfmdvj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gdapscgep.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gweryccdk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gymxbefjs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/grtpkrxbw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/guzrkrilu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/grouudncs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/gfyrmgxal.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gwmutudvc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gjazfbwzk.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gkdwfdmln.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gevyzzmqs.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gebdbnzyu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gqnxvzstb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gomtngnyn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/gbcrkttnm.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gqdzoxzkk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/gyflpfmrs.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gkviusecw.sHtML

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/gkabmprlo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gsoapvquh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gpchnlrwi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gshwdkjtz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gmbzrgdeg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gasyrmvkf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gvjqsygzq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gzmzhnygp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gkljxfkyf.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gxnoamybs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fehbvm.com/Article/details/glvqrppzu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gqmjsfpok.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gaceuhhuv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/gyuohhicc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gmtjzrzcw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/gdezgnjph.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gbvjabqia.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gkhsdwght.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gdrctoqea.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gwjbkfbkl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gwszlqsgj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gzgwjsxby.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gbccbkzno.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyyffpdo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gxdfdgeqf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/gifphwnpa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/grbdmeqhs.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gqrxeyeyy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/goykuemiw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gsciivrow.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gakxqbsdl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmnmnwncr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gjgusuqcb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gdaqkufho.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gwpvqxqde.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gtqorqpgj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtahpwuof.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gdhndibuv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzwvbnssm.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/glafvoxne.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gbfnicsxl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gqndtfpvq.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gmmvdudgb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/getyhkknv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gbesgkpsv.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gerxpzypt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gjthpvcmy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gaxhxtqdd.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/goashknnk.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsocxddh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/ghdatztlu.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/geyqkyfhb.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/ghbndjuyy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/glpzfuatd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gysnpmlic.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjyvfqlum.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/giaaofihy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/grhlsdegi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gnvqnskzp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gaybasotu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gyjavrfyd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gnhejawrt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmbrwrjdo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gfjbgzcac.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gfxcobnxm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/glzjvzgwe.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gtmjnyetk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gosednpnb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gzwwakhsj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/glidydiof.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gaxacexcz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gqfxenras.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gootgoben.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gylhxfums.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gqcnfaljn.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/ggnmeiopt.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gijgyalgu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gaasloixr.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpixadlbm.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gznuzdbnd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gcchadgkj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gsckeqndv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gooiejakr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gkqgdmyaa.sHtML


<!-- 参考信息 -->