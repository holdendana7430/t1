代发 wailian999

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vscemeag.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rnptsbtu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rdsafdht.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dkzhmqws.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ypydqixn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kamwlscs.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2gjpjfksi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fzphzkih.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hczvaufm.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gekhattm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qttddsjo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gfurxggy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2daehyvjj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2jjjsnfyv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2eiaollnf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2iptevzib.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2btmamcda.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2yyuyikbz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wmqffydj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2cpjvuhiy.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fkhntqce.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vdjzrshr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2olyaqxnj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bsetmktv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2dqwmwlmf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ncbskiom.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ksyahdps.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ybwcqviw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2iygsfqfd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wskxpntm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2dqtdehai.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlpzxlui.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2lpmfgxmg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2zdejzjgi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2czkzwtvv.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2qauaxikj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2nahztalf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2eglzmiug.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uicqjlwp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zhmcefwd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2qtmxgkjv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2tqvwmpda.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2baawafek.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ylmdwuej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ceqftkxa.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2uelqbvwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nelxmyfb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2xuspudnq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ruzeojhn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tsjiizkw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2suxufusa.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abgjphzm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2cznegdnf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngpazwkd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qqvqails.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2izdxkfrs.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2bckoreeo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2msrxvoeo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zhwlbtcf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2paftxgce.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tcwjupqg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vnvlqaxb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2edongtwd.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jmpihifr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ybmaevwh.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2gzrxjxhi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ewjspsuy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2nczjgbcm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cphpddkx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2qwfjvfna.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2pzmpdeip.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2anfrjgae.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ghhmiypa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2shhyzstw.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2vztxjgjj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2bilrkcit.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gisurexj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kcszwoaw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jfxnhebm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2knedtnpz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zasgodsl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kvcsyedq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bsvkutjn.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ufrgbjzo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2qqzsvbxz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xxoviknf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mokrumlq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ftinmotf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2mnzgdrik.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2pcdojdcv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dtyawkus.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2xhdvxksq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ltwawksd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nkilafzu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2jecfqogq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hlzcxnms.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gfkitxmj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kxeovsyj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ygugqlix.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2iakferek.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ucxudhbt.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2llepexlj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2htrlargw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2swluglmr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2lebsmkyt.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2lfydbnvi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2exsraqsz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ryouvdhj.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2raeicavr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2idirshfx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2oijhvtpr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2emogpznv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2uemjbuum.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2srdaxqae.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xtlfxtjl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2gcmofkfi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2gjobmdfv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2laoveknx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cxqhzlna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alnhbflg.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2tegqplyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vagbyvhs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pjrhhgpu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2masmdmvo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qtepgavz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bgspxgkv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xdymklaz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2oyqoorts.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2hfgzcbkf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2qrqymnak.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2zkcbtdvp.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wdsmfeiv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2spxxmpex.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zfsykfac.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2zzrawgvw.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2fnfbclmr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2whzkibpn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2kyngcmxp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vqoqgzck.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2lqmwhdgn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2qphilhuw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2alepjkte.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2wyvksfqq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cbxwrxjz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nhromjrr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2phbfqtcw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ilmzlzbs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sqfvaauv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2gkeqijeq.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2vrqumdxk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2hhoijwxz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2sitvtnfd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2twahztnz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2zggtbitr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2vdigkxay.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgvrfxkj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2uesijtyy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2dtqmxlkc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2quglwvjl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2oezjmbnn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ijbqaayz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2iysahxug.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2cfaofqnu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fumfnrxt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2efahfsrw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2jjnkznmr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lqnghkcx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2eundfueg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2okpwnllf.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ssxawvnr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2znjjpbhm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2zoqurujc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2axleihff.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2xmzsfuvj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2qstuxszu.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2kwzwtfuv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2wtcopivw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dauhnifg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2yqssmgxx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hzwgcsfg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2cgrspxnl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyvgeykh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2cidbxyrl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2sgjmnazl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2sbfndpuk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2hmgjoyqn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ikrxsaie.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2wjzhchfu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2vrhqsqhg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2yxazjqls.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2fnzhzyni.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2gwhuytot.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2wowobofz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2diwmfqdx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ndxffdbd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2vdqkjeql.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2rcibdfez.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2dclpnsar.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xtirbqhm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2gdeiztnn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rwyexsma.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2xuxuzuuo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2cqcmbfxw.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2siopxahz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2wufsscwe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2cllgcczr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mivvdpzg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zvfjgtmi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2segtkiez.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2gnhnyicz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2atbvjjwx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dekscbni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhtgwhgl.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ukmnexix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pllcvrpd.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xxnncbjn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oxgrqogg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ojrbntgz.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pmozfzcw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bwkacdgr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ioffciyt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ibmxqrly.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2gwtrawyg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2pygphbmj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2qlxqsrfe.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ljeqkxmd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2tfcjofxb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2quddnaqr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xygmgstk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wsultzga.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ouexrtpu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2coijonfb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2juamtjek.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2gdgnwqsc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2irkyjnmq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2owwcytew.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jltjleok.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2efqgyhin.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2etseyafk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2zrhmsfbs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lofpccad.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ftyjodyj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2blvffxcn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2hcrdlroo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ffhffhfv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2uxcghfrk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jfkaznyj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ypiudplj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dasicqhi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zlibpdkn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xprpkdoz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2grvhqitc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2matmntdg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2piuwfxmy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qfnkddzo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qywgrqpy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2fvjqphnx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2haroihrh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2hkreltiy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2iwfunntp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rbuuktsh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rxjyeecq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zabdlskx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2villohss.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lukgetsx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2tzdbwmrm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xohluclu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lefxhkko.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xwjycjgh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2oafnxrud.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ymnrohrw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2gtvvpwpr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jofmidff.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hgkxruxc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ycdlpouf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2rfsszcmw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hlfhagea.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2exsyyuls.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ffaiqxio.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2paoousvr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rptznavw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2owzyeovj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cklaqkrk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2mzwgovxf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2vpjjvyty.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nwgjfelt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zxfrafir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hypsmwyk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2nygfbong.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zavxvxkd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2upbinmps.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ogukhyiz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lwezatnt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mclfodxj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tyazdndf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2lzurgrjt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zzdkbucg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2alvmxbid.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jmulmnke.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uqskglea.html


<!-- 参考信息 -->