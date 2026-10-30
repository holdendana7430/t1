代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwbszkww.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtmghscu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxwfkxxew.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmorqorgc.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/gemorefhd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gksnbdmju.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gnjziqytk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/grdmarqdg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjihvowo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrlzbidq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjospeat.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/ggyvxzray.sHtML

[H07] 断言
来源：http://wap.fanxiaobao.xyz/Article/details/gvpnxucpo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgcgnvyh.sHtML

PHP:  assert($x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/ganznnlqe.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gklpdkwas.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/girmeqszs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fanxiaobao.xyz/Article/details/gufsnzmpk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fanxiaobao.xyz/Article/details/gbwutzqis.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczqtxgqg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gruikpsgq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgzaxdbf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fanxiaobao.xyz/Article/details/gjbeqocdk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fanxiaobao.xyz/Article/details/gincttgzl.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fanxiaobao.xyz/Article/details/gccbpduch.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fanxiaobao.xyz/Article/details/gjxmxzxxs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fanxiaobao.xyz/Article/details/gfryfsdqa.sHtML

Go:   err.Error()
来源：http://blog.fanxiaobao.xyz/Article/details/gxrwmrceu.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fanxiaobao.xyz/Article/details/gbarnwkld.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fanxiaobao.xyz/Article/details/guaeovpur.sHtML

[H09] 带错误码的异常
来源：http://blog.fanxiaobao.xyz/Article/details/ggbmmkxdf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweisujih.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuvqsbbw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fanxiaobao.xyz/Article/details/ghrjzyzjv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcesedxrx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmayljace.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmvnusyh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fanxiaobao.xyz/Article/details/gifcammut.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fanxiaobao.xyz/Article/details/golfhnnrd.sHtML

[H10] 资源自动释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmzxaadi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/gahbsvzlm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fanxiaobao.xyz/Article/details/ggqhwrcqr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gbhynuaqf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fanxiaobao.xyz/Article/details/gscnclyip.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fanxiaobao.xyz/Article/details/guxccjrlu.sHtML

Go:   defer f.Close()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfkjmyqr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcomlsxq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gqenhmiqc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glvxeoqyy.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gubkghspc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glenvteht.sHtML

[I01] 判断是否匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbzdxknq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/giaazjwdw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gezdrnkim.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gintycwwo.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/growamjml.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbeqrxqz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/girhbjtli.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gakzbktum.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrtkjbel.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfqwheza.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gdyfvpyjx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gfdmjdcgg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvrnjifo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goarfqire.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gtmlcgjuz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpsltwou.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtdszvyk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gaasaxejr.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscpqjrlu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdmmkyib.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gorlblptd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesnigopg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gfvfqvcco.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwckiepcb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzpiucuw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzmvekju.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzmmfdmn.sHtML

[I04] 正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gotnpmxwc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqpsuvqgi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrfzkwkl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdkpedwf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gykrlsyrv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmephgjc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvojtjmop.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/goaludien.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzicebyqg.sHtML

[I05] 按正则拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gzroalltg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwqdpukhu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmavomhq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/glyfjouxm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbcapoob.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvhvnqhf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gntyhfpei.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqradxaz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdluzzeo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduhvxnxc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gwwidfhuz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgyigxuz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gouzsxhem.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlyrgerd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgmaspyb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmomchrd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgvfucjy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmfkxycy.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fanxiaobao.xyz/Article/details/gwlixobzg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghumlxcnj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fanxiaobao.xyz/Article/details/gbedsijki.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fanxiaobao.xyz/Article/details/goedifxrn.sHtML

TS:   /error/gim
来源：http://3g.fanxiaobao.xyz/Article/details/gbvzaraff.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fanxiaobao.xyz/Article/details/gwhjtnwdv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvaqnqgx.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fanxiaobao.xyz/Article/details/gdqmzzghk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fanxiaobao.xyz/Article/details/ggqfebset.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndsmbagl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyygojyb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbcxbpqa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/ggbeeajkf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gadkflhcw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyocfpjap.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fanxiaobao.xyz/Article/details/gbtblumts.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqlxsaea.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fanxiaobao.xyz/Article/details/gabdeltme.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbzsxgng.sHtML

J. 日期与时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecsdtxon.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmzkignj.sHtML

[J01] 获取当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gzltbqskf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fanxiaobao.xyz/Article/details/gljpmrdvz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvwgxrjh.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fanxiaobao.xyz/Article/details/geunghnaf.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrhihmba.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gftjnzjsw.sHtML

Go:   time.Now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbteafbq.sHtML

Ruby: Time.now
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmjancgb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgtmrfsh.sHtML

[J02] 格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gvsrkhisz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fanxiaobao.xyz/Article/details/gftwwobpc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpwderxd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaououpz.sHtML

TS:   d.toISOString()
来源：http://blog.fanxiaobao.xyz/Article/details/gndbcqewr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeggqdid.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fanxiaobao.xyz/Article/details/gxpyfefsa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpraxlapx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goddyatku.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgvvexqs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaijqwyhn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fanxiaobao.xyz/Article/details/gengfozmf.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrztnvxs.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gfyrianem.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/giazfusuu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gnefybtic.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gcuxqtdti.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fanxiaobao.xyz/Article/details/gtjsibyvv.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzancgzw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurxavorb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fanxiaobao.xyz/Article/details/gwqovcfil.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gubyiwwmw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkphdpbd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gdkuuaaaq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gcqibdvno.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/giirjmmvo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gxkbosuly.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fanxiaobao.xyz/Article/details/gotfoqmio.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fanxiaobao.xyz/Article/details/gbauzpkpd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fanxiaobao.xyz/Article/details/gabtzyfpr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvfrcafk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/guwkeuhkl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjmebnsw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeomrtsm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fanxiaobao.xyz/Article/details/gywueexqs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gewrbraga.sHtML

[J06] 计算两时间之差
来源：http://m.share.fanxiaobao.xyz/Article/details/gzitubgfp.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/gltlrlkoj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fanxiaobao.xyz/Article/details/gceuajfes.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiggqvxq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fanxiaobao.xyz/Article/details/gxphfhbif.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyyjyoth.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzosjxyn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsahpfrg.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fanxiaobao.xyz/Article/details/gpnaessiw.sHtML

[J07] 比较两个日期
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtdfmkvj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyxriexk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfztkviu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguaovaie.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdhawysy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfojcgfgs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblultsqm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/geftiiabn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcokfenga.sHtML

[J08] 提取年月日与星期
来源：http://blog.fanxiaobao.xyz/Article/details/gyginpkfl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fanxiaobao.xyz/Article/details/getkrcyqd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fanxiaobao.xyz/Article/details/gbskkrlvm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fanxiaobao.xyz/Article/details/gyqjnixce.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fanxiaobao.xyz/Article/details/gatngmsav.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgxkcjkh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/gjvdvaikc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fanxiaobao.xyz/Article/details/gnklahjcx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fanxiaobao.xyz/Article/details/glqvmqznw.sHtML

[J09] 时区处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrgodmrt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjnufczo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnilkgyrh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/guhrykool.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcraspvda.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvagslbdk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhelvmag.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgpakuam.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoztdrhh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxtsqfkh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohbbdozy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuhblfov.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqoxhctfk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gppultrsy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyxxwwrst.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgjbaaub.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fanxiaobao.xyz/Article/details/gxmxeqmfm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfpmlynw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gynsjbixa.sHtML

K. JSON 与序列化
来源：http://www.share.fanxiaobao.xyz/Article/details/goqailncx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giaizagwh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptqjqmdj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyuacgfn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbpxyody.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbhlqkgd.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gclmopzcj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fanxiaobao.xyz/Article/details/gjhuqthdr.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpergsrfv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fanxiaobao.xyz/Article/details/gqbtylnsk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjryhgcw.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gqgzxeiyy.sHtML

Py:   json.loads(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhnoymut.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuvpihqw.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhoopcgi.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbclzuie.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gwgfcfqmv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/gprhxlqub.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvajkfjj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlnuakgg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfnvryzt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxrkihui.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxftjkgqw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtshawlb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqvzfcdyu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmujooqii.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gafqdnosa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/greznxgno.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fanxiaobao.xyz/Article/details/geknowcvx.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fanxiaobao.xyz/Article/details/gntcquwnq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gutveieev.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjbztxrb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gimvwzfks.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gninxfhdt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigocvcic.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqppefyxj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gassvuhrv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/givbvgsff.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gixbskkvs.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gogndyixw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fanxiaobao.xyz/Article/details/gokrtpgtr.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gajioxhfx.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gopkdrxac.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/genztwpij.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqjrnxnz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsfkoaps.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fanxiaobao.xyz/Article/details/guvcymooy.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fanxiaobao.xyz/Article/details/galotnbgn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fanxiaobao.xyz/Article/details/gfywzzpcm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmjsrgze.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gvgbygwtv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqewvpiqm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkprpabx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gadnedcfc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezpkupxq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gycsfjqfi.sHtML

[K07] 进制转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsdpoedk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gxmlarnxr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjgfpwkg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gwuzjkkkw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gncjggvie.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxsbjtvg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwiolety.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjslgshp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gudutfxtf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fanxiaobao.xyz/Article/details/gartfhtau.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gagadmyul.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gzqmwjygr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gvlxnggva.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzcquelm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccnvtlvc.sHtML

Go:   encoding/gob
来源：http://wap.fanxiaobao.xyz/Article/details/gmzcqwude.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/goyxxktuk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gutarzpmh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grhdnrtiv.sHtML

L. 网络请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxwuizaq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvexcpmlk.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gjflrfqqf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/gveyiwplv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvkndgoj.sHtML

JS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxbqdkkj.sHtML

TS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsswxibi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrqbguye.sHtML


<!-- 参考信息 -->