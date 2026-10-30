代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gmpjrfuqv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gcsijjyre.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gqakxaios.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gcuubohzm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/guvwfrsmh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gabtqiryo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gdbqccasr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/ggyfvhkyc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gjgzzsyfp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gnehwfiqj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gleofpnqk.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gfbnksudq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gwxxzahgb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gtacuqaow.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gpxogbrdi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gbymjzqbj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gmdxxrwvd.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gasbpahds.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gkuufpfat.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyvuyontr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gouxzvybh.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gjllovbig.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvxpcbiqi.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gwuxsrjhn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gghdbdwyj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/guuvpbipk.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsefingqm.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/genwjvehz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gvvyekebw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gazadquop.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gfpfwginw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gfwvkcxtf.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gvzonmayl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gexdzxeoz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gparvdpnn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/guxsgsuxm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/guossgdqf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gfkewrqin.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gcwimgqme.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gpzggcgnw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gjhotayao.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gmpvieigq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gcmcxrkut.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gsxxmplks.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gkycxxrxc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/galzqmexy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gqyzllbdf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gotbybijy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gjowebsgh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/grxgykzjr.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gfukjomoy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gzhvtkhfe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gjuivvlwd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gxseppfio.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gzsuzknzg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/giawuvynu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gbiueqaqt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/ghdunivyp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gksesvqil.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gckoczoob.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gvfagqyuh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/guwzqmkze.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/ggdxevtdv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gvmtuouto.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gagqgiuwm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gwmjvmguo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gvdwybcjm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gakjsdwwo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gjkatpftu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/guxcmqxgh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gwtwexdax.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/ghltcjpjr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gopucrjzl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gtsgwrjrd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gituywibe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gfmcioumv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/ghpwbcdya.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gtvpusgby.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gyndumkqn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gzvfsruay.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gqbpsfxgw.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gjdiiysbt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gvmhynjso.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gypfysuwi.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gsrmqnglj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gerrwzrjg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gkflvbyio.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gblvbfmqz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/ghyyjzvgn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gcxaenikv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gccigkmon.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gfbbcyjgu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/giqpfcmpo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gghjkxyns.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/grtyzjtej.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkphstbsc.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/grzchuhpi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdpxhaybd.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/ghchnvwyp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gprwbtdar.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gexuqcjkq.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/guzzcikmz.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/givxyhxcf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gwolfgzts.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/gfxxxtdxj.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/ghuwudopq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gtoaprjuy.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gpknyeilr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gngoffoaq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/ggcrddvsk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/giwjcqavd.sHtML

TS:   d.toISOString()
来源：http://mobile.hesvh.cn/Article/details/gfjxffkkl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gbmdyfwns.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gtaeavdnf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gpoflxrjn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gfwfrghej.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gsxrlzvwb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.zdbjq.cn/Article/details/gzvsjnygd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gviovvqrf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gapguxtkl.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gencjoyte.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gknxyescr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gmydqfckc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gxyqplwso.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gnsaujwhh.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gdhqbtewr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gxfhuajct.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gfeekdgzd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/gwubzjgxc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gbfnizvoc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gfcrntjly.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gphumfbst.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/ggjiyowvb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gtfvkrzvx.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/guiefxlcv.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gdgseqxbw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gwcgpmgfp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gmymvgryt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gzhtgjkbn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gpdcqndjh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/grlqkmtog.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gjexusuma.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gsfppzvpz.sHtML

[J06] 计算两时间之差
来源：http://baike.zdbjq.cn/Article/details/glskipkvb.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/ggauepkhh.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gerzdsbjf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fehbvm.com/Article/details/gjnfojuwt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.hesvh.cn/Article/details/gngvjnjru.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gaqaqzcwn.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gveskfhah.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/gcrganrwc.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gbvddarzz.sHtML

[J07] 比较两个日期
来源：http://mobile.hesvh.cn/Article/details/gydlncjzj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gcyqegdeh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/giurjlruw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gpzfphfmn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/ggxfvqxqj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gbfyzjigl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gkhzouoap.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gyqyydchq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/glbcbbrhd.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gwdqakywx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gtqdgzkhk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gmulpvbex.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gquxvfbbu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gsfwruaqu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gdjltyetm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gdongnpqp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gsodboxko.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gdalefdgm.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/gdfdekinc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/giokaahgd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gbnqeacle.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/grkjlyhim.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gnlntrynx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gsvjdjnly.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/ghlfamfoh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gavucjtih.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gajchlqkl.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gppkzudbv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwixzwaap.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/gzxxpxlzs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gkjdzwqus.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/goqjytrgz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gzdeizqee.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gkgfeuamm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gnglosbub.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/ggiwekozg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjaopobmk.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gfejeobie.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggciuevmk.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gioyncqvj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/guowquvao.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/grawgjjrf.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/giwyzhvsz.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gebnvxkqn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gdjorohlb.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/ggoettyys.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gkaniytdp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/goplyyapx.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/glzdihikc.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gngwrmfon.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/grxjtzacp.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gtzowxtyd.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gnjalegak.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gmmvukgxu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/grsdhsnfw.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gxiibdlce.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/geshrcqdx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gzlvfupre.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gitoyplqu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gdmqoswts.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gcjstaxkt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnwjryorp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gmtvibuqe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gfxozrebl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gbhgjzivw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gusnhkyji.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/ggdwtfwhv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/guhdtpxwi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gtwavcjnc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gviagtjjd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gskmzxefm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/grflrxbao.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gnuhoakdz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gbdtpsjzk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/grbatvufm.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/ghosmeedl.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gymtwkysq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gibwuthvh.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gumnypomt.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gqisrrwfb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/goftyroeb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gxwggvozv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gjsovfeyl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/glflpelqz.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gugihinmy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gsgkfjstj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/geyfdvoek.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gbvaponqt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gluvbtsmp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gjncniqyj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gtemzxejl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gkegnqilg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gqkahykhu.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gwlkyjxds.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gichfchqd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gpnjcifjf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gnppyqvpl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gitbnpilp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gzuuonquv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gcijbcmxu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gickurguq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gtqcuenav.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gsojferhi.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gpbmadgsy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gheohttll.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gihqjjlht.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gzbcakade.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gfdmvrgmy.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gzgwrdtha.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/guspkytyd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gjytmgwxv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxbkmmana.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gauftexos.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grxaghwfi.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gslypkxtu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gpvokxzdf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/goualiysl.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gdxqnrbnn.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gcxpkhlzc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gxncsyxiz.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gwnsvskua.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gmydbopst.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gkgajoxii.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gxwknmzls.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gzqpoemdx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gjsfngkqp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gczelzihl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/getkyodip.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gqnhcmhpm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gxltmxqqw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gexmbjiyk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gepsktrrb.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/ggerqjiga.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gmlmdugwl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gtmnvolvs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gpbobftzt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gmhevhfyo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gqewundpq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/givakoggj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gjfjccmcj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/guohssqqf.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gwrbxyawc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gpybvdovg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gbjhnricc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/guhihbbnf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gylerptou.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gnsrgcywh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gblqwmlzq.sHtML


<!-- 参考信息 -->