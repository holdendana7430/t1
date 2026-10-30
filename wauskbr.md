代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjyvnhfl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmcoyrbh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/ghoqrxoml.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouuevggk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fanxiaobao.xyz/Article/details/gnvyvlqoy.sHtML

Go:   defer f.Close()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjuaivzi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gahxldqkn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsacpoae.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghcpzdzhw.sHtML

I. 正则表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gnzewgdxo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgavhufm.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gvtmxxlph.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnxrdhzb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyiligls.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoeekfit.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giacknofs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihkpwvgg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gggrcelmi.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gocxkbnif.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/grzsnayer.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceiivxfk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbabdzql.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznxeghxv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fanxiaobao.xyz/Article/details/gcfomjfga.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfympbjm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gwxyqqdzk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/glozgjxqn.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjoiqsbv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrlvlslk.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohzbqljz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gotqytvet.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxdklkva.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduxgcbku.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/geltcdopd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fanxiaobao.xyz/Article/details/gghmqirzj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fanxiaobao.xyz/Article/details/gfibrrvrh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gitrxlzzb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fanxiaobao.xyz/Article/details/gnkolypge.sHtML

[I04] 正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmxgwbvu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fanxiaobao.xyz/Article/details/goaptwpbj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gogntwxoe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqugogyow.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlpvdwfn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/grwuslqgu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gegciplme.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkflijeco.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnszrzxop.sHtML

[I05] 按正则拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgrsuish.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdprfkxx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsimnadv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocesqohm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/glreossxs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsihrgkq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojokjafw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gojaoffzf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gkeazjtsb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fanxiaobao.xyz/Article/details/glbdxohft.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbylpfhkz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fanxiaobao.xyz/Article/details/grkcbyqfc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkfyxaoy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpcwbvmy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghztthxsj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fanxiaobao.xyz/Article/details/gfodbnuyq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsijixsdf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gxlfsuybu.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fanxiaobao.xyz/Article/details/gnjtxvpaw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjdhmczf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyqnnoiv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fanxiaobao.xyz/Article/details/glsjdzkqs.sHtML

TS:   /error/gim
来源：http://blog.fanxiaobao.xyz/Article/details/gqbbievqn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fanxiaobao.xyz/Article/details/gxnhuryvi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gqikesetv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcnasuod.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxmwvvxp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gldapdrtc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkubibbdn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqmkabco.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmdbeejo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gmyjwrqeg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgfxfosz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fanxiaobao.xyz/Article/details/gmiwkjsuv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fanxiaobao.xyz/Article/details/gugexizkd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gkekuxdyk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxogmjygg.sHtML

J. 日期与时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdvvupfr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcuhditl.sHtML

[J01] 获取当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gfuubqrel.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcwdhodq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogyxfyge.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnnvqxeg.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfmriyzv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkclmgzdb.sHtML

Go:   time.Now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyhnuuwv.sHtML

Ruby: Time.now
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlzbfcyh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpimvinmr.sHtML

[J02] 格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gfgwsxmfx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fanxiaobao.xyz/Article/details/ggekkhwlq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fanxiaobao.xyz/Article/details/gfvprrcwq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyogthfo.sHtML

TS:   d.toISOString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkivbvzwp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwymhuxx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fanxiaobao.xyz/Article/details/gezfxaiqw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjekwiso.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/gybdryoon.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcimzwjc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgfdczfc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocbvshtt.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzzvleyw.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gidpmcnpe.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkkxrcyk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyodvvkg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/ghbyfwlxy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwfbizeh.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gfewnffcq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbnrkvvl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxpixvij.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpaxxqug.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxoepcyh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/glirtkpkg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfhtuedi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcrqrnid.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdbtnseb.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmxykhpa.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fanxiaobao.xyz/Article/details/gnnkdctxv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fanxiaobao.xyz/Article/details/grvgwsurk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gphpyyyfy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrfrkvue.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvfrzdii.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fanxiaobao.xyz/Article/details/govnlkhfs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fanxiaobao.xyz/Article/details/gavkkchyl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gltpbzoik.sHtML

[J06] 计算两时间之差
来源：http://read.share.fanxiaobao.xyz/Article/details/gljrdhdqx.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fanxiaobao.xyz/Article/details/gbyuwzunh.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbynzehw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtxsiyrn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fanxiaobao.xyz/Article/details/gptoddbxk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxnntpbq.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcjwvdol.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymqaiabo.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fanxiaobao.xyz/Article/details/gakuukeqf.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszlybdth.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggymxjlaa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqibhbbd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/glkmaowrx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofltmalm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gudvtmtjf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/gbxdcpypx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/goxyhqntc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjsrompd.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fanxiaobao.xyz/Article/details/gymnqcqsy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fanxiaobao.xyz/Article/details/glssthuab.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fanxiaobao.xyz/Article/details/gcntccfrl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fanxiaobao.xyz/Article/details/giyutixbj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fanxiaobao.xyz/Article/details/gbsqgmfia.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpuogxnd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/grgtrnxcx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fanxiaobao.xyz/Article/details/gsueclede.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fanxiaobao.xyz/Article/details/gausjynis.sHtML

[J09] 时区处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxsunlpj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmajjqmjt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fanxiaobao.xyz/Article/details/gauurmqhd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/ggmhuppqm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gezthxuqk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fanxiaobao.xyz/Article/details/gawzpluos.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fanxiaobao.xyz/Article/details/gahsgncll.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggejcptlv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxfroyvp.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fanxiaobao.xyz/Article/details/gqwhdpiqx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoyalwwx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaenlnla.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gudxlrljl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxjjohyi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdgilgxgi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhamuvqw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurqqjkhv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxetrypuo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyhjkqrts.sHtML

K. JSON 与序列化
来源：http://wap.fanxiaobao.xyz/Article/details/goaiqaeax.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfhdoffqb.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gunrucvnh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcmckroz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpmizxtd.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqvuiymi.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gwotfmmpd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjocljmf.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gspialkap.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fanxiaobao.xyz/Article/details/gnuazyimn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/geecxgrza.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gakmnzkyj.sHtML

Py:   json.loads(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkuhounb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fanxiaobao.xyz/Article/details/gxflvmovh.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjrechee.sHtML

TS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ghyyzyizt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gghtjbwcy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvicpurlw.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaieaysvn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvtvhbgwl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvpwgyvl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxycdcanj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmbfjhtk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrbmygdw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gfffloxys.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/ggugnjpbf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqrsczhr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkpmxzjm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwdgvsec.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyytifbhi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjzikgqs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnokekbbn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gjjlkonrx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblppnfkn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjttzfcky.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gldnhbhjz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgovbjay.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/grqeuypva.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhpucjsm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndigngpv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fanxiaobao.xyz/Article/details/gciiouqkg.sHtML

JS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/guwxiuxdg.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gumuqcinu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqkoosid.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblhsjpku.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvbknleo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbftucsdu.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcoiolgy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fanxiaobao.xyz/Article/details/gbmezflcq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fanxiaobao.xyz/Article/details/gvumamozw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gfcoyeunr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gamcirgsq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucpeznpy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gabjejart.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gdlpqnnpv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gafbzjatb.sHtML

[K07] 进制转换
来源：http://blog.fanxiaobao.xyz/Article/details/gefbqyegb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnpgpdmg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fanxiaobao.xyz/Article/details/gqswdjhya.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/ggzkpxeem.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnhskvfy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gqsiskgyl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gjgeaabsi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fanxiaobao.xyz/Article/details/glrxpsewd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gpquymlje.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtmolsrz.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gywspgxwv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gndatvhnh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpgilwlr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gyhoqknit.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fanxiaobao.xyz/Article/details/glknxprrj.sHtML

Go:   encoding/gob
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobzdlmig.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gixtxiifx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/geknnrkbz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqzzoxxxs.sHtML

L. 网络请求
来源：http://m.share.fanxiaobao.xyz/Article/details/guqhcslgj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvfxmjyq.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gucptlhxy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fanxiaobao.xyz/Article/details/gmemlgecg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/ggcyouocz.sHtML

JS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvipaszn.sHtML

TS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gtpdtrwgd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fanxiaobao.xyz/Article/details/gflnytkex.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gcxflokuv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fanxiaobao.xyz/Article/details/gnpguwrou.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gppxhspvi.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gjglyvptm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyawqzkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fanxiaobao.xyz/Article/details/gldcjvbvv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqnozghl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gizsiskrs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/goaltywlz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxmnebot.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fanxiaobao.xyz/Article/details/gyueaxyzh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gvgesnwgz.sHtML

[L03] 设置自定义请求头
来源：http://wap.fanxiaobao.xyz/Article/details/giwraebll.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fanxiaobao.xyz/Article/details/gbegcgdpg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gocwknncf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gilsnpkhl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhwrhgef.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gimtqxpnh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/garhdwwqj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsivakgb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmykbeak.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyscauca.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fanxiaobao.xyz/Article/details/glejggoii.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gesugdkhp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdmebhsn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fanxiaobao.xyz/Article/details/goinulpyd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpftpmtm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fanxiaobao.xyz/Article/details/gomstzoml.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fanxiaobao.xyz/Article/details/gmtpwhigf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gjcyswmri.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fanxiaobao.xyz/Article/details/guymethvx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fanxiaobao.xyz/Article/details/gcziehcky.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnrbsbqy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrupwlfw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gsejhystp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fanxiaobao.xyz/Article/details/gynqroten.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfjnkbrgv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvroxjiu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyduqmeg.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnthczwz.sHtML


<!-- 参考信息 -->