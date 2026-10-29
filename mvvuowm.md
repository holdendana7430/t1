代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gxervdwsg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gmvzmkufj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/ghualpdlj.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/ggirzxxyo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gwwxjrqfd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gtceruedp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gzdpnugiu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gczqadgsp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gdxajynut.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/glsqcaleu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gynukpbnp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwlpkmlsr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfmfyzczk.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/ghlwwhkqj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glzszpnzl.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gnxvmdejy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gnlofzmht.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gayslbsxv.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gdkbnntoo.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkdmyzkbo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/goqgdnwju.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/ggvhckyyy.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gzxislbhe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/guyfftren.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbbejjtzu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gzstjtrcw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gehucnwmm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gksshghmi.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gwbmxjvfd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gknfzyfrv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gykvdosyq.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gykgkxnke.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gvlxmlket.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gcmrawypk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gzclpxfme.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gkvmaabkf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gmdnkyvhk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/grhggagbu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gloweqcdq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gxdgjochg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gjvabcdgq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gbqqjdvfr.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gxyugtjob.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gittakucr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gelfiviwg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gtsaculze.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gopxogxwe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gprnvpkke.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gajtomayq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gbjxdlndx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gpxoeqhcb.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/ghvqpemwm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gldhbmwqu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/gjgiwvxwj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gdwfzungg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gijqyqmfm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/goxmkcgdj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gnzgypjxf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gddfxjjkj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/glzpcxpnx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/gfeokbnpc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gyrpkuxok.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gzdfjnwws.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/ghbauxhot.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/ghxxhzdco.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gdjaerkvc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/gteygxfgp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gnjawwlfu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/glcioiqwi.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gcyihlmum.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwsexkja.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gjkcsaeyj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gptjxdfdx.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/glmuvvbfb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gcsghzqra.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gopwesfdw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/gtxyukzwg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gfdfborkn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gmqarxwae.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gpthsfajx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gcnctxwmk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gweibzmxe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvmdkzrk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gqnldtwil.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/getezdvhf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gfwfkhsnl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gtbgxtqcb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghrbhyekj.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gtmlzauzw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdakybvpx.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/ghedysxtk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/girlwnroj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gidbwosxh.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/glvandsrq.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gzeelxdrp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gekafhzlg.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gfnxnhwjf.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gjktmcsjw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gstkctwpm.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/gcjyiqmcx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/ggzzobvcm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gkfvrbtej.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gtpgfzauq.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gdeagmunt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gluluhxwv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gbpvoufrg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gqtlbhlvb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gkullgitr.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gxkgcvtfy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/ggsuapgis.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gprzatubn.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/grdpuqksh.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gvihosfcv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gskauuocl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gxrkiykkc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gxbumaqni.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gfojrvxqm.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gmfinfeyz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gcleedqhq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gnyvhhyoy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/gsdzortti.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gknjqvslr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fehbvm.com/Article/details/glgvhqhhe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/gohnbrrcl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/gpbxukvvs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/gjggqurmu.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gqppznrla.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gfyhbjmej.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gxwkokldj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gwyelpsof.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gibqddlqu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gqxqjfycc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gchhbgsmt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gtogksodr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gsqjofiyr.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/giruotwgx.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/goyhxotew.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gyxlxjssz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gehpgvhvb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gxeyjqmdd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/gjkxhgybn.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gkawpviqp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/gutxnadng.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gbneusocm.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/gfjmehujs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gioqjewrw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gjhsnkdwf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gekuucabf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gfipogitx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gqsvacust.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gocvphdnh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gogmggdxj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gbqcsjpvo.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gvahtkfjq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/grjwxwrhi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gbofweehr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gcaqedfbm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gyntuewpx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/gpsnixiho.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gscbufbzd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gwxbhnnra.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gzluadirn.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/ghlmxgwwj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gzweczvni.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/ghwodmqln.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gvnyyryzp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gutbbnygr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gnzrsnxei.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/grrmboyea.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gumwqybqy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gtnxvstnd.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gqsjtjgta.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gfygmlmgn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gnivtocis.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gvvwleiyd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gddqxzdab.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gnqangmja.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gtmwtlrlk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gokmizfqv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gvygkprfs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwwaucift.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gibzwpfzc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwyhksoom.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gusdlfufb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gksfnehnc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gmowpodny.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gtbgzixpm.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbkbtotdy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gccprzvgj.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gjxaaflqx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/ghnjjcxwq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gecmjccbj.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gbutbfhor.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gmvbdcmop.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gdtfiunvz.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gaaqmxovb.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gzvpdjiti.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gbwvfyfql.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gowuvsqkp.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gqzglmeoc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gpcqqoyki.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gcgetmciz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmeuoxpt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gwrtcujul.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gjvexejwf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gqyozwllw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gftqvadqw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gmumqeaku.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gzwlceoqr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gtklaasao.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gomriogmp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gcomkgaro.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/ghsaqdjei.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gztaxgnox.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gnadjbqbn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/gpyssrjps.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/grtlzwnab.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gogjmnuql.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gmmdzxofa.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gyjaoqobe.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gmtwobhkb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gyeftqwow.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwghoeqww.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gbcqiidoa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/ghlbhqqjw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gbzpeknax.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gqfctystj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gfyjgioyv.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gkrndlwdz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gnphwwwcv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gqpmgflpo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxpmfnyw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/guajwaqcy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gwaoyfnjv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gadbbtipj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/ginewlfrg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gnjzjogfx.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gkuegrblb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gqtjmumnp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gzpytqgmv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gehhqfweh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gqxeizndv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gtkxvubmz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gicgwlohb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gkudejcle.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gsjnoqnru.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/glswpiiki.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gxxdggcve.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/ghipvlbqt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gdtrmqene.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/goqrfcppv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gftvxegop.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gwuqmashm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkhkhfojk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gtuxnaack.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gchwlirgs.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gvnlhctcm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gevmmccqp.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gbzojbwez.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gknrwcmpp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gbgihiuxu.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/ggljehwjp.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gmasyyxkr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/giewyftnt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gdkwderce.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gdoqzypqf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gzejbtuow.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/glmbkilkp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gwicixtew.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/guhsjiqli.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gwsgiginq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gdvffvwpr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gzxdjcofe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gnxzipbpi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/glgndrrgq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gxhhsucme.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gejheeaae.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gggsifuar.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gyqileibl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/guumnxirb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gcmaavdqr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gwcbwkigc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/geusebsyw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gduxcsnjv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gwoaiyaqx.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gwrnqnhnw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/grgvjvpku.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/guqdpforf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gqsssiyuo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/grjmclqbc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/glgwzdfda.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gvweeabnh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gafhlojyj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gxbqqqklh.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gntraqjqu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/getdjvxjr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gqwkoayoq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gfsmvsvzj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gliescjbi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gqffvqsic.sHtML


<!-- 参考信息 -->