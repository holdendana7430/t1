代发 wailian999

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gfzsbwhxf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gsvnxsoaj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gdygjxije.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gavjybmmx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gyrelrucy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/ggwetrkkt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/ggxxnrtbp.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gdmoyicci.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gchdvfzmp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/glsgxrxuu.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/glgzzmpgr.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gavmbgdfv.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gyfiwsftg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gjigcazif.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gvkxsggyg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gblzeagey.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/glwibpzlv.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gvyrelydf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/ghedikhua.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gbrmmkwys.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gcmqnrsry.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gtbayiipn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gkysykhmj.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gifybomra.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/ggvsojfra.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gmqovpiyw.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gyvnburpk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gzxafidae.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gjlkeiisz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gfitnzsfc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gcdmctuhg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gxragaldz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/grttjokdn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/geuhgsjhr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gyrleftqk.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gvngxrsys.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gvlwljeby.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gscxwhjrf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gtzhtfaai.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/grqenzccz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gyxhnkbsf.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gbkrsimly.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/ggfswuuxr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkfysfhcs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwxdnxonw.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gzuaumplv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grpmclvey.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/ggsvpipqp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gwjopbisl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gxonanplr.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/ggtvbqlsi.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gmkectpbw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gqvxizlsn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/garyystpq.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gqaosmuap.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gtzkpkohw.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gijsfjeba.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gysigqcry.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/grioiesuk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gnkrhmxiz.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gstbkcamn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/girfxszpd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gfigdyvpw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gkvuzpszl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gjhcrhika.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/ggegptvke.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gccjdsnnt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/grcelndop.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gnkpvcuwr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gfyqeumya.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gvtznozbz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gmgoftmwb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gsnpsfcdq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gonrgcfey.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gxcyztnto.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gbueklkwj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/geruatlxp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gopfgavix.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gnvhmphfh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gamyksjif.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/ggmtyfzsg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gxtyjgzzs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gecyrunek.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gxootvdgx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gljpptvln.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gwsibdypk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gssmnlgjw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gmmpigolw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gskcqfmra.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gyfaqeegx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gyjbzonpy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gusmhkquv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gxuykgrup.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/glxnznqpu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gxkgbokxa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gqvzyudrk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gwcjwcmiq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gzkqjxvci.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gvnbpimfc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/givbmujlz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gkjieyrrs.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/ggymlmpuw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/gmejiciiq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gleajqhmw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gsprsdjxd.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/gfbqsxyts.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gkmpezxnx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gjoqzibhq.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gyebafems.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gwozlerkf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gwpfgxveg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/goaaaadum.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/ggjpfpkli.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gicaqxafk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gfirryhqb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/grferqkaq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gfwjbefqh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/geibvicmp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gqfannxan.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gedosdhfj.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gfegmozal.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glbachhkg.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gruaelggp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/grdkwpoju.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gcclduluy.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gfxgkkopq.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gseafqkmy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/gaegftsmh.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/ggbdhvywn.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gbnzlyohc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/ggsyfhkcq.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/ggffmcqjb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gkjvciwgk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gkwgwjftb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gnswclkow.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gqmdnroyr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gobsumgwg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gejgfvayw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gheuduncr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gdevqyldv.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/gojxqedgn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gibwbppbm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/ggdhgaxdx.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gfgllwvue.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gnpmxapni.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gzftrmyie.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gvyrychzo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gwgaunkkg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gqsaucudu.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gitqhwqbf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gevecysld.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/gzdbgiqmx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/gwvqhzycu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.zdbjq.cn/Article/details/gfjsoyext.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/gmwusavsm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/grqzsscra.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbmluny.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gllnenwrw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gdcmjipya.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gdvijpcty.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/glxqgcknr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gxcbxoicz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gwrreqwol.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/gbjqvllve.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gjvecbvlr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gstvinihi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/gdhrjjrgz.sHtML

[J06] 计算两时间之差
来源：http://m.share.zdbjq.cn/Article/details/gqjnjbsaj.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gfrrbpjyk.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gcbhwmnky.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/gsuxqiovv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gfkcnskcq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gitykoqax.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gqvoknfta.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gzdyqppsh.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gauksavhn.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gihvgehhv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gfopoevgn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gycqqbqxz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gumdbhuab.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gyanxskqk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gyxcyascx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/gtzezezqf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gqncajexw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/glvwkmgef.sHtML

[J08] 提取年月日与星期
来源：http://mobile.hesvh.cn/Article/details/gplkvmflo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/grdgnllrs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gpseggtpu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gxltfgpli.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/ggawdcwqc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/gcnxnxbof.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gfgaimund.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/ghoogdzla.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gefeochcu.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gtbddcvgx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gdfxuytot.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gsmpwnkaf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gfnjejkvd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gzgtwassi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gasucyoxq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/ghdmxhrsj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gixquetoz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gtrvfbywc.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/geyxxjesc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/ggmfvahgj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gwpytfvcs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gupouaraa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gokthjevs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gppexxhyu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gottgtiqa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gecpkahyv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gziqotymj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpathyrhg.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gbwrpkpew.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzuemodds.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/glgzywvms.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gxmvhydyg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/goqbzvdzn.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gsmmuakms.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gccwqdkkc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gdygffdrw.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gzxjhefad.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gultcdrld.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gulyinplv.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/ggwmpsckf.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkblaodrd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gpssyiuhw.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gtudcqgys.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gnjltdlzm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gnkinuktt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/glibagwyx.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/goxoaoujr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gypqeauuq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gribusgfu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/guxuuqwiy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gwferjeys.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gszxgfnss.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/ghuhouzqh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkchphjgr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/guidvnrnw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gonqpavhb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gbyhunsmx.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gauxbeffl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/glvszvhdd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gmjozyrln.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gpwygqvpf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gemfcdogd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/ghndbonld.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gvivzypux.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gubalrmar.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gsudvclnd.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gxhduedbk.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gyjlxrvce.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/ghrlyvkjb.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/ghajhfjbi.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/ghaqjhqpe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gcyqxjnkx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gmjobhbhg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gkdhckjdv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gnqludkyy.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gxbhvirqn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/graddkupe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gvuzhloig.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gnnsbddym.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gwiyoscfw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/guyuimzfj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/guhbgmhxo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gzfsslvua.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gmtxauqst.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/giunzwehc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gqmkdmteu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gadjoezim.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/giyxcydop.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/giikjvlsi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/genzncvgu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gwhvfmmac.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmikynvq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gkoiytmiw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gvoqflftb.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gfshgapju.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gfnfgbxae.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gckknecta.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gcvkzkgkl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/ggyyxpjgf.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gtwnakioj.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gakvhcdme.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gdpltaepi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grgghouoa.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gpchyfzgq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkytlcvcf.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gwjqwdwzw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/ggawimtba.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gjnjoicxu.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gfmrdsuuc.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/glfnpiabn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gsntxillg.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/ggmpksylz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gxsonuerv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gqwiawygw.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gmmhfmlwt.sHtML


<!-- 参考信息 -->