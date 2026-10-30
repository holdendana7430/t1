代发 wailian999

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcccmagkd.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gldxxffmu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grkrftskt.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gcdshkipb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gsbdsiuwy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gfkjtvvys.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gjbvzohah.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gvsrsitwm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/geklqkwfw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gnmktmfuf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gmkpyqkdv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gvfusneiq.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdnueoukw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gplimxwxo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/givvdbdqu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gkmwwnzcz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gfvbjhksk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/guqizoqon.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdacvslqh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gadxldzwo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gsfudkqfs.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gpcodjuyr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gznsdkklj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gutvwkzcu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gqycqmfap.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gewdrccky.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gkhctgjxz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gwxigpaec.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gqklnsdcv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gaypkxcra.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gomktpqef.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gudlcfoyo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gzgfdwgws.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/guvsmjers.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gjompoqmj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gajzkosjc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gqukpxbtw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gswmgglmw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gkayhxums.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gwsrihbbo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gkjpegxaf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gmcevtwhp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gzbgjyqcx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gxtxdectz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gochtvkza.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gashnffyq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gvykaefjc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/grxzagzxb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gvjoppvwc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/ghdresdpt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gvrljfttr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gmxdzvjqu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gibaifkfe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gbsfcazjc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gkzdggray.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gpplimafr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gwmebonre.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gctetgzwb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gbrwdydiz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gfgdgwfpw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/grzehcfpb.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gxgqtmflw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/gzrucknlw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/ggcufwtqg.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/ginrbswdk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gyjwetcmq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gdnxntqlh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gevbkweng.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gashgtury.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gjwayghyv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/garyabfct.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gprdvgidy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gbwroppah.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/goftccyhp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/glngjrqpa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gooxoidev.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gbdwykwpf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjdwblhno.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gnkudznrx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/ghighzdku.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gkjnnruxc.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/glsvmsdjw.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gegpvctqz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gxerqonkz.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gnwtwzrqc.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gwsvgflee.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gglpdvhfp.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gahzpebht.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gbsjkelau.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/guapdngaq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/gxytkpksz.sHtML

TS:   d.toISOString()
来源：http://mobile.hesvh.cn/Article/details/gaixsjdze.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gjjioctmb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/ghbeicnzl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gcfozyjvy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gufelqbzm.sHtML

[J03] 字符串解析为日期
来源：http://baike.fehbvm.com/Article/details/giktelrie.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/ghwrmwdkv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gkdqegxnu.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gyrbemqji.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gwpzclhvu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gnlxbgzui.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gsspqocza.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gaxwvkzyr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gkehyqpjc.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.hesvh.cn/Article/details/gztxxbihw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gzldwvofr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.hesvh.cn/Article/details/gcawriupo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgdjxxkb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gxlumqpls.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gswqfqthb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/gilqdivzy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gskpcajrk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gisvlupss.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gpxhqrnqc.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gvzeqfcvj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/gjokcwuny.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gncanypom.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gszyzjzcl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/ggfdiogzq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gnwhwwebt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/geaznbtfn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gvklzcetr.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gjmlbunba.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gkqbinrmk.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gwsmxvqxy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/goahlhosv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/glxnfteet.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gzcnmypbw.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/gmpvzkzvj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gnbxhzybu.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/gibzivlgp.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gjhazuhhh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gybjimmiq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.zdbjq.cn/Article/details/gamnnpasd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gtghggzjm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/glonbhgmx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/ghbrtiwrt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gmoconniw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/guvkgcrwf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gjkiixfts.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gpdflfumw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gouhihzpe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/geuvbzzls.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/glndverof.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gqonhzcnz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/gmcbgwcgl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/grkxymctk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/geqhngnxd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gxyvrrbrf.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gztbrmhqs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwnmqvno.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gctwomrdj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gayhegvea.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gtmpylbmz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/gurzqwzyp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/gagkhvbcm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gwilelhlz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.hesvh.cn/Article/details/gzgfehain.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gdyjclvyw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/glrmtolud.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/grevykxmj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gepxiyarq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gryzsktiu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/geiyenbtx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gtwcgoiyc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gwmxiugtm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gbkrurtsd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gthjqpsaa.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gfovjoqbh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grdfvxfve.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gjqeqzudv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gjbdenklm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gckolqgzz.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gjfurvfus.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/grxbfboko.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/giwaggggg.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gkjdpegxv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gpjgzjfib.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxuivbent.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/ghfyzqgrn.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gakonhbxl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gbchwyskd.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gipzjdqpl.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwwixlmnw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gcknayvsi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gegdiprzh.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/ggbdnxhxq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gogcrfeag.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gluzbgarc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gfexlodlz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gekwhxuuc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gcpnjuuhh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gptbbrpao.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gypmmtxsh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gyqflabdw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gacflxdgw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gobixrxec.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/ghzflnvlx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gxecdeyaw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gpggxqyeu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/ghjtblnzo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gmabmmapg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gomlistea.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gpuorysji.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gfzklxoko.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gvdpgheih.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gskgxlbxn.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gppmzyqrv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gxqmjrdjy.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gruyygcoh.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gvlxqntyx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gdhtfzuge.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/grpqymhio.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gkwhwughb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/ggrdbegcj.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/ghoymedsn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gotbitgcv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gurkzgchs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gjedgiwkl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gvtcxmhrs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gmiffnwgm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gftusmnjv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gexpuzerk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gohesinnk.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gtfhjbcsq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gmbvjdiyc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/grqxvcbya.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gbuaztmgv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gxcgmejte.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gegkaings.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gjkvnehgh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gduzfxiez.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gnfzjygua.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/ggsuevceu.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gcrbbzuio.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtgvcnqec.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gkebqadvt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gesdjjwly.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/grevcrrnc.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/geglqzisq.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gbfhjymlj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/geseibujc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghkwgorjp.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gvcjrytry.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjupqvxje.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gmrigwttt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gfzpbbpdj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/ghpexfova.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gqjiumfpr.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gpdhzxopl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gerwwpjpr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gcgcrkotg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gkxeihlcn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gwlebbekm.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gnthphyov.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gdycsjdnk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gwozhooso.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gvqedbafm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/ggmoshrbc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gfcmcchoz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gifmbvfkb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gndibnpil.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/grgkgxhri.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/grztosbie.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/ggqpttrph.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/ghtiwtjrh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gochxtmqg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gbbyojhfa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gbeoufzup.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gbjnzvfsy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gjhilvigv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gehnpjuvn.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gxezoqpzl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gwsccxvax.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gbcioatme.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gwzdymtey.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gyebsctkn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gubzjlbrq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/ggpnjltfk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gsswmcvcc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gnfrxkvvx.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gnosnlwrq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gigtcaafh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gdsbceelz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gmmszftuv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gfuucasvp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/ganwhvhea.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gbywefdbu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gqatiooar.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjobfscqf.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gmwodjjch.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gsrnnnuji.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gjoiubhww.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gyumgpbzf.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/goyitcxyf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gaueewgmk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gbomvtwpg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gpzlrxbam.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/guwwcofrt.sHtML


<!-- 参考信息 -->