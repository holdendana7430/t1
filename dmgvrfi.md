代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gbwrufzla.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gikuwvyyx.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/golqaveej.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gtyyfmoiq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gdpqfoode.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/givzovfhw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/ghvfecpid.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gazcupjvc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gvcusrsef.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gitlvjvjz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gcxkebkgx.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gewkhscwj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/grazaxifj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gvukpnczb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/ghrxawltc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gcszkxhnj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gzwiyecst.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gnxfrpbtg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gjxiyacbf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gezvvbobc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvnsakqby.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gbtggzcxq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyiscvcxi.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gowpngpti.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gepvqcbwf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gsgragcbk.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gygfdtywu.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdcbmpkm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/ggfgeyhgt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gepcsrzoi.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gigqxnues.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gyfuvfknf.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/grvpvojym.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gnuacelbs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gwkaquffm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gdrqzrpmu.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gckvlvzjk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gnrunjyzg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gghnqtfqv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/guflkjash.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gwcexowgz.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/grvzobfdz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gkzrjddjn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gaczcjyvj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/gxendohyd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gvyhzdtbw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gevheptiv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gkwzugucf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gnfrnewoi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gvwztfhmc.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gcdpxyysd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/geymyrdpe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gycoximkv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gzzxlxrty.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gzdltoctf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/ghqxnsksy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/gbwavuvtd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gqaulsfzx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/grjtrvudw.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/giszzhxpq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gyyxociea.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/grlbenlvm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gpmaudbyk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gkkzqbfdl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gmqkkddhx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gthsmhvzi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/ggxmrsaes.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/groesaxkk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/ggrseudzs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gkkstpqbr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gesrtrrtl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gtflvvmvq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gdwxuquqy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gkpkrxyyj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gupjeynpa.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gtzuqytzx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gspvitdgd.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gdnrmsnmh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gxfkictyl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gksprtttn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gxydndtsz.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gmetmvmuj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gxcwwfcme.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/gvqpkmvaw.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/grsztwfwz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.hesvh.cn/Article/details/gntznwsou.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gytigrupw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvzhurg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gclljpknb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/glgzppezi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gsvceofsq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gypahuslv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gclthgscx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gfngpfwfc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gtajmjjoy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxlmkvxjr.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gvkfportq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gisytgsuh.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gkbutusoe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/grkvofmji.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gjsclkdcv.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gwoiricwo.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/givhbenbp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/gskuivxvl.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/goqpgfxtd.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gxgokvakc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gcspmathb.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/gofjearbg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gcszxexsk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gjsouesez.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gigfljrlw.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/gyccysvbm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gazllyoyz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gdysvfgqs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gohmexarx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.zdbjq.cn/Article/details/gkbpoejmb.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gpyetnavx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gdwusazgv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gonarrmpo.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gxdklevli.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gmqygmwaw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gjqyyhsfp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gjbalziom.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gtkpjmbth.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gsayllbgx.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gqkizvrya.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gfeyvsvdq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gjjmghzsc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gstgdjnig.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gemuwrmcx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqpdxdoa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gcoepreum.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gtrxglvqr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gdkpalyee.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/gdwugnfqd.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/goasdmtpq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gqlprpiel.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gphwetegk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gpaiyisff.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gjhlhjkmp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gbtevnyme.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/ghauaejts.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gjxgadobw.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/ghqdlpgwb.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/gwwkmnjzc.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gmouxkxiz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/gtavcnhpb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/gvwbwcoxj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gzcouizsg.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gvxgsuqzd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/glnpxezxg.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gqxvuvczh.sHtML

[J07] 比较两个日期
来源：http://blog.fehbvm.com/Article/details/glffokibv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gwxvphxyv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/gckfqjsbv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gwzsieioc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gzpkgrauq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/ggpwzunmd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gbhhywruy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gqalnrrzx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gvuuvslkn.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gxuqzlofb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gipzymcum.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gdggitrmf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/geombjxmw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gvpfnoibb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/gwiuvmlzs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gablwvkjq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gkscwggni.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gxrxwykvx.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/ghlcfjdpg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gkzycspmo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gphtyimcr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/grmmiauth.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gaqqipbca.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gocpanmob.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/grosuerot.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gjgsjqdzo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gwfqmbhal.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/ggwttewdr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gqhgtuzbv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/grmagfrge.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gzfvvfafa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gnpwumjzd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gplhsltuv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gnjylrcpz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gxqmkczeb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/goivzylgg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghurodkjr.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gsipydttp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfzyyqner.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/guzruuxpy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/glizvnmgr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gkhsipzge.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmsdpnrkq.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gqvfhcgfg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gebzapscw.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gfzkkinjc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gfxwacybj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gyjuagoit.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gngrhgecg.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gqswhcbjg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gaekzktoa.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/geybcfeiw.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/givoviazu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/ggzmsezqi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gnlmgwrzb.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gpsrheziv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/grvepblij.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/grmfmjxjl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/ghgmursvk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gbzbksclw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnbjjumdi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gdekyhiyz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gqpzjrurs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gwnggblxo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gtvzvxpfi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gmmyjrfdm.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gjhzojmcp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gnbymnwos.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gfqzulthq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gvwrxtcti.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/ghaimyzdv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gaxelnlqi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/glqyfwbea.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gxwesutzi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gfoeyfabn.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gaxtgebes.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gyyoahxuq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gsguumjgy.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gosozxdgd.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gobajrrbo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gvbqfhokg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gdrygfpmz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gqfegqalu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gcdpeymhr.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gxuykhvix.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gwaqnllpn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gmobgypbz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gtxnowoan.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gmgpofcom.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gqarkcnqt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gqsmayilr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gskgzvlme.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gzmuggprc.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gdccvwqba.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gfvuzoxvx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gvpzeiedn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gmzmfqfaa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gofbdlgfa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gcuaquwur.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/goypdrvbn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gwfymhcpo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gntyrhmaa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gvmylaonu.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/guazkmobo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gbtvrdelw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gsmybkrxb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gjgtrinml.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/guspiyxle.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/geiddduak.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gfuzkkeke.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gmdmlrpry.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwogmcbrr.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gbdfyndly.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gahvwvaui.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/goshygdok.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gepvetqva.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gqskgnufh.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gfuhmxnfl.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gxcklgkln.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gwqjhhilp.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gjcidcjhl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gijrqkcrg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/guqvzirnc.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gdwfmrwuo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gpyzxqphl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/ggrpmcwid.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gkxkuzggu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gjpcfskhf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gwqrcwwmn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gayejwkpo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gcdrmcyej.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gpbgcotea.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/giysrsjnm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gskqdfhhq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gbcpkluyp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gfbhndmlr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gqxfbpsue.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gwuycvtul.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gsowwotlv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gwwhymnup.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gqvagcmjv.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gljobqjsu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gncvjuxtq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gxkposnwy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gypfzvkku.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gfnxyfpsl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gkxljeqof.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gtqozpxqv.sHtML


<!-- 参考信息 -->