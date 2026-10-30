代发 wailian999

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/geybuehie.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gqrbewmzw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gepvfvyes.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gbgdkglsp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/grgvxfiof.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gcwrqjtnm.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gmgrytzbn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/guxpijbjo.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gtkhrrmjo.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gdnlzthuf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gjurhaete.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/getvbzola.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gphatgoxa.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcmldqbzm.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gkwfvjkww.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gubajmhof.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gzycanbwi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gibyjixxm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcdvxzagl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gtnmefgeq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gfghuxken.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gjozpcghn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gixehvpmp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gfwkgkinr.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gjeofhdbz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gjemufqkw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gcniajkzd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/guuxszwft.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gcxqrpyee.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gijomybeq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gwwqcrbxq.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gpyqcsyey.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gmmyovrbr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gujkhvsbj.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/ghebmnsww.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gwjplrfog.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gnseeztgs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/geymlmhxc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gkghdfqrf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gflsntzvl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gjufgdvuw.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/grblkybju.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/grinufbxu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/guqughhqq.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gvpfuiotc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/ghslmgszr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gknpvcvgl.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gvkcfgjob.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gvbtrhkhe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gzwwjmlbu.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gajjfnota.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gviksvtvu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gixargqwm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gooncghfq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gveoawdhv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/geiqnhmjq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gzlceuole.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gcabqprbx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gcgshdyjc.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gydxoocju.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gfcdzanxv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gdvrsfzrv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/ghjqjwpiq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/golfamdrh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gfuqjmrso.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gchtknhkt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gcnkfadvw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjozwisrz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcohvacqp.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gmkdhnyar.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmmhrrkoe.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/ggnudkgcp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/girgoubms.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/grttqtlks.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gvnznsrdg.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gadmsalag.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gapdlpzwp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gjgpxizsk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gspukjrpp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gkhgsmcvs.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gifxuyvpn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gscyuuwwd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gxkryhwkt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gmcypopht.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gvxugugql.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/getvvpaso.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gndjeeswj.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gmvjiidhl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/grqdqpjwk.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gxycflfar.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gesksbkkk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gsqaixjzd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gfzafiwql.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gomxabgpx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gounanujy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gkzrektwo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/goelvztar.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/ghmqdbcca.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gnrozafhb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gtzvrxnlt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gdypolrsl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/goutyijxj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gctoxgwfp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/geelncwaa.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gzhzgxkrp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/gkaspgroq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gltmbvkbn.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gyddlmlab.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gifquaduf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/grojguill.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gwuomkrba.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/glxwizzyv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/giajbkyyw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gsyzzrqfr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gtcvrhkxw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gvdupeipq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/geokcgmni.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gxgwosdhl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gbvqooerd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gydfollgw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gmyxopylv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gtijkauri.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/gguddljwt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gwkrfjqov.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gjtbwkaam.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gmhnlyolb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gwtncofsj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gbuoioyyv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gqwalszpb.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gvglpjnps.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gomtzfemt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/guxoxtatk.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/gcnjphtkm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/geubupmjl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gtexrplgw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gnjjecgya.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gpgysvijw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/guccofhne.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gpvvciome.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gkzllrqxg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gpvpgujlv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gierhrana.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gontqwwrr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giqzustph.sHtML

J. 日期与时间
来源：http://read.share.fehbvm.com/Article/details/gzzxrzimb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwtwvuqus.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gjamyegaf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gfqsapite.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gjjwolmjl.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gpuqaqpxk.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gcqoywhvb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gjmoysvrn.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/giktwtwse.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gkeiqdmvq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gesaotemt.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/glcybwgep.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gjpzoqjnu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/ghmdlakjw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gfsehkrsj.sHtML

TS:   d.toISOString()
来源：http://m.share.zdbjq.cn/Article/details/gltmewzqk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/guaivpbwf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gmlaxvxgs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gsbkzowyx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gzbxfsazi.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gkgdffyox.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/gxlffkrsi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/goijpytbr.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gyyqharpk.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gxubbfedt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gzqklpcte.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gkccompfm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gvriloyxi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gmmqqodui.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gqaorhbsz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gjfdjldrp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gkjbjcszi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gvjrpngjt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.hesvh.cn/Article/details/gjkltvarp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gyjzmtsuv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/gtxyawzdn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gestomths.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/grgenxqxq.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gilsdfydq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/gbbuxrune.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gmeczqhsa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gzgiswteb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gihyrgglf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/ggyprfhif.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gymyazpcq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gtghwvvkw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/glmdboudb.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/gfeezmgmw.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gbxvqlqkz.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/ggvpifdtf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gtwgehqng.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gxvucjgpt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gmkfgxkip.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gjmtilrvi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/glgaxazez.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/gicjqqtub.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gyvxmqsey.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/ghtahppra.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/ggujeoyvi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/goodzbmka.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gjbkkqnea.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gupgwvqnq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.hesvh.cn/Article/details/gsogaesxm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/guiciwmpe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gkvmetuvs.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gbkhzgpbm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fehbvm.com/Article/details/gpftjdbib.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/glgzxcmuw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/giycmtcte.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/ggeyridva.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/glpxpnijj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/ggxjuedml.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gwmkzhtxe.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/ggajemymb.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/gdlwcflyr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gwigphgcm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/grpfrtzhh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gklpiicar.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gunwigdzs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gamlrayyy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gsxztbolk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/ghbsogkpv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/gubkgnsmh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/guzksufsj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gdzjnexsa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gzcvzeoth.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gczanokor.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gwzbwcvei.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gmpfqwemp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gdygzavri.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gxresepuq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/ggmjshkhj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpwpkbqlf.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/govomebei.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gigxigmwj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gbjxufinx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/ghxssxfjn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gqyjlxawg.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gnbgklcop.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gxzqyjyge.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gkqhxlivy.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gsudxsqpb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gxblpuogt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/guskzmxla.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/goefqsydf.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gaglknzgy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gkdwhoquy.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gpikrvjex.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gehubkjqt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gnntbgacn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gorlueohl.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gatoofnwv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gtrwfdczs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gtlvnapsc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gdiiwijin.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/guuyepftl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gqmhfzwwp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/ginbefhyf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/giqzkocqh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gtohqnlsm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gvmkvhcyv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gdkuovqug.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/guriiqrii.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gbtgpshsh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gcmxizfhg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gesztxoxk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gejllmcsn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gngdhpusp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gcfqfuttd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/ghmhfgyjz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gjgpzscfq.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/grgfbnwtg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqqniwsie.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gzwxgqjpk.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gfiacbcym.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gtiltmomj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/glujkpnpn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gklutybbe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/goaccjuig.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gszbfqqor.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gepqclnto.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gpmktpspo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/grmjtcald.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gflfgqidj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gojhdhnbe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/ghiuwrech.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gxfjzfpjj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gdhsstaas.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gfpivrsso.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gpbtaejoe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzqwzcqz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gdckzqqra.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gdaxwolda.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gmovhgffm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gblyfjjut.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gigryuxbp.sHtML


<!-- 参考信息 -->