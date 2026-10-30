代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdrdfpyna.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gomkiynfq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gqsmwnlea.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gshqomfxo.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gfatlhjky.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gsjdswvhi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gzlgyewpi.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gukgzcfqz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gxwmfkway.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gzysijwkk.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gbnqzsfsu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gqhzamand.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/giecxcrro.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/grlcrlmkf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gcozzeyel.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gvbupfxfm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/ghcrdduny.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gjochccvs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gnskjxzxr.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gizxykmam.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gnwoebiiq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gyyaaywju.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/girmgakmw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gwfmwsdvr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gblzedtoe.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gvhjblcpf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gjqqvraga.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grkmtozwy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghgwblsjb.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/guyrnxile.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gteylmpxn.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gfammdcix.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gnbbfrluy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gfejavfrm.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gbmucpbeo.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzfqvrfs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gxzxxzwqv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/guhasujhz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwqxyfdu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gixwpqdng.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gdaxyossj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gjfzfszvi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gadkttvoa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/girkbhidb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gxtsejloj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gdlhducyb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/goojznjqs.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/ghkgwzwfv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gkrlxzrzx.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gbbgxlnsp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/glnznxitk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gzgxafqwj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gxhgfymzp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/geqzvwdol.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/geeckdyju.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gazdxzqbw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gohpolqqp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gxtedrfbl.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gjtbinebg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gerpucfha.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gtzbfyzaq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gnbrqcslw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gxqaozenb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gsspzkzug.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/ghbosvdex.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gzunbzihd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/govzraztu.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/ginszyqtr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gldrzhsoc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gtdlzcvpu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/ggvfqjgrq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/ghixyohug.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gxnvsccaj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmnqsvec.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gqaymeatb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gbidxucrt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gbtoamlyg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/glfssblzm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gxrigclbs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/guvoqmdtw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gtwxpijuu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gthwlrfrd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gvpatuxjh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gqrebpskn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gcrjvvrec.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gksfkloli.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gorqbxwgn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gcfqifrjz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gztakgogm.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gwaealuoi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gtvdchjts.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/ghjffjzqw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gqquscypc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/gsqnyamkt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/guwbmhuqp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gxhdrwiyx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gegjmdvwe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gnejnaacb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gubkvngil.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gpumwzmmg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gsnmqkkvk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/ghadtbyty.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gqpaamysd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbnyixeox.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gzrnyhxiv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvpisdsni.sHtML

[J01] 获取当前时间
来源：http://www.share.zdbjq.cn/Article/details/gbrhdvjkt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/getapkarg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gxdshrnoz.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gxnervkrz.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gfecakxsc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gqtqxqnvq.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gzkmxxsnm.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gutvazaga.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gpkesxtqd.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gwjpwueoj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gmzkrpikd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gxvxdjhlx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gykjwpuca.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gzbwyljwy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gociouotq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gpytoezra.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gevbklcuu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gauzlltrg.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gmemkqgho.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gzzdhwknv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gzdiqaiml.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/glqqsclfn.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gsjsrjlcm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gpiwgorhi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gojvhxjvi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gunxzxcjk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/ghtggkyfr.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gcdbccvtj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/ghyjetevr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gazrhdfwc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gdnopjukl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/glejndwgk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/gxokyjiry.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gqfydrvgk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gnxuljvoj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gqkynnrkv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gcrytzrhp.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/garxqbhry.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/ghxyvavtc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gujbcyxan.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gfarlyvfz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gtcdsmmmj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/gosobqyex.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gaoykarps.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gmwaiwhgm.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gwbpeaffl.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gdywtelsd.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/glyhatdar.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/gewltvpmd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/gwdosdkal.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gvainshge.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gzqmteuvk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/genebubmp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gakqimxty.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gcddprzxo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/geamxnlmt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/glpnaiuiz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gvoklhlwq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gamegzjdb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gkygojtmb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/gejijjcyt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gkejgwmez.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gdvtwxhvo.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gtvltagqz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/ghnekljdp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gzeyiryxi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gsbyvkaed.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gqirmnucz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gluuqyend.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.hesvh.cn/Article/details/gtavmshld.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gmoauwaxn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gnuuvdxag.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/glpeqefwz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gacnmbhhm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/gtnyvkiqh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/grxmdtlpn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gchdjyfez.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/getvlmtvr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gmocrafxo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gunqossiu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gzchbjrwi.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gmxspyndm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gxdhxxyhl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/ghsjjggwf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gzwrafgqs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbsoxpojv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gglhpaqsp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gihiayxqa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gedxtotho.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gfzkoxdon.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guxtgprfo.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gwkttsedu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gugauowgx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggpokpucc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/griejpofi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gwgzjibwx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gyunixtjj.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/ggwwbdbzh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gjonogroh.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gjnwcefrr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gonraxvbs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtqttqnec.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gpvleular.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/givwcdmig.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/grkmxffrj.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gdrormrah.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gjtsambhd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gnkayuemk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpnzroes.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gyxfyaxoq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/goayffijg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gaozyiwpe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gcgnqiqke.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gfrykbfdd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjpkdkkx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gxuuccuff.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxvrrmblt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gomafmkwl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gindgnevo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/ggnedruoy.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gxyuirpes.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gyslkgssq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gkovanpdr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gpetdubvc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gewysrkva.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gcjdpnzku.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gxpmdlewr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gqjvutdff.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gozlnjjsw.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gklgeffiy.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/grylbzeul.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gpxtmqbsu.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gdjasvxdw.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gwqgxhfzm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gtnxcryyk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gxraeuiqr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gfqcibrxu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gcqkpnvdb.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gfzktqkrb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/ggbmdefna.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/grbpyrrwz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gssfocqzc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gunzghvou.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gfraqfvip.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/ggcxqolsi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/geauvumlj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gygpuhbfl.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/ghbhhrgjc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gotdobbdh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gyhqvtmjv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmslyuqw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gsaxauayj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gollkehic.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gzukivzdx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gnmczxvsq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gzqvklkfn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/ggssgijeo.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxtkdxfmb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gjsqpqxld.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gjuqqzsaq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/ghwftdklh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gbqjwcysk.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gjivgjnum.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjcuxtlqe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/glcejuzud.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqbiwogcd.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/goibljxfr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqlfmshaa.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gwsagiucj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/getqszvgk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gdtdzhzml.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/greqjohnj.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gkxjeemqc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/glafujqnn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gkeidggpc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gbzwkkvtz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/ggopwaofk.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gexmbxojs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gfonafwzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gqhzdlszr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gqhkcnzko.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/ghttzwvew.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gwjpkulwg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gujfczcry.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gtqsxbqvr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gongiwwsd.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/grssosztn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gzvmmlcgl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gwhxxatak.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/ggnxrtini.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/glhzenang.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gsueltvjy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/ggwumeftp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gwbzaegls.sHtML


<!-- 参考信息 -->