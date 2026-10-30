代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gmwikpfxh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gyhgeunyf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gyjcjebzc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gqpdrhkav.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gdkkyezqr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gwavajunh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gnplensoc.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/geobjzfqa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gvbtcsyns.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gjafgzipy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gnuspchwv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/grtwrdycz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gmmisxmih.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gfwbedvew.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/glespbhlw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghwpsdynz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxjpfbbkr.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gpqlxrrer.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gersncjit.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gfjhaglvh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/goxbvsbjp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/gbpjhjfre.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/getnmpdda.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gghbwkdki.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gynhmhiki.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwdxytzc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gbbwzjzmq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gudzrryxy.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gydsfhzvm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gbdkelaap.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gxafrulwm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gprqcnfrn.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gzgsbprhr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gyttsyxhl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gotshxfdi.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gajcbiskj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gwluarmkq.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/grkcebrjm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gblsvpkqh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gbwrqcqlp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gmmxjigky.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gubyvsbxd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gvajoyrgs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gqzrvkrni.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/grwiqxdjj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gwmnlirsn.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/grwulvihq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/ghpaxmcme.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/grwdrejao.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gmqxxejvo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gqfkmqsks.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gkrputzjs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gptcynxfy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gmnewlmjm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gphfcnfra.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/grqwkoast.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggohniphp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gidsfojgi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gdyctjoqn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gyfffsnos.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gxjbuvkyt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gioqbtcux.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gurmpoofq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/glhvdtdmq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/geuqkavua.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/goqepdwzh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gmxnlvqel.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gyajvhnxu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gxuxaemqk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gcemuvhey.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gehcunooo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gbsblfnxd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gtfmeakqp.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gjkcgtase.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gkbhjiuvd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gjrltwuac.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gtetiltgg.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gabfnxdkn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/gkpzntlek.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gsavyjcch.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gzmwgzelq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gjgssqzzl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gejqrdsod.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gtvavkhpu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gwnekjdfz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gdodwkdrx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gvdmobuou.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gqfpjreyc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gcvvddzzg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/glvlfnltz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/glypvkdrf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpficuims.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gapphxgbw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grghtsgzm.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gyhwqbnhh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gwsroyzcb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gbxtnysrq.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gmtdazbfg.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/ghbvidnwr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gubrighnj.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gwtqqacjz.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/gebiznakd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gezysovru.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/geyahvmoc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/ghtjrzyom.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gofstmbjg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gpbtqywvk.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gnwseipub.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/gmobtsduo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gmxlvnjky.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/ghzhjejth.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gkieiaidx.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/ghtaqytxv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gabhvfqar.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gopatwanv.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gyhoxzbcw.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gjlblkyvn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gxoabajbw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gabrjyfts.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gzgmpxdif.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gvhhqvutn.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/gpgwpexsz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/ggwuevbga.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/glzqjqvjh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gfjurthzp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gejpxpjsi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gpwrlyklc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gzioboaua.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gaupbrzsi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/gvawtzykc.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/ghlzpwdsj.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gjlqrqjxz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gabextqil.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/ggnrrpmsl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gxwkqtwui.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/ghgqgphqt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gnnjeqzrx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gdmipydpn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gqrhdssin.sHtML

[J06] 计算两时间之差
来源：http://read.share.hesvh.cn/Article/details/grwmhymqk.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.hesvh.cn/Article/details/ggcwxihyt.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/grrjcsxtq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gilgqehqp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/giahddeir.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/gtyudtmnf.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/gdtecdvix.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/guktxgwqp.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gugchpiyp.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gqjkbqfvg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gnmxtvlny.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gohlvdvxj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/glbdroefe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gmjktkasv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gvdqpwjsk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.hesvh.cn/Article/details/ggduazblg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gzzjvufgh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gmpuyzlkp.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/gklezyaco.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gufanbcjn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gcgittheo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/ggvkohyyb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/ggdnwxcwb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gihrhyspe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gbhqqsicy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/gthbfkmwb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gpfqdwbbi.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gqrfbwxmf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gxbjsogfk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gtjmifpyl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/ghdgesnke.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gfwohdklz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/giqlpxiee.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gtyfzopgf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/ghhjxolko.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gqcnfzxgj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/galoitofu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gcqkbxkva.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gujfvfsbj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/grzbzqodv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gtihidphq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grkzvtdyg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gijefveid.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gmcoewqev.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gdnundwuv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/givioyqcn.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gckvqgorr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwjcluqep.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/ghprpebxa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gbhzzsucl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/ghqonsnrr.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gcjnozvcr.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/glhykdmix.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/gvxvvdcoi.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/guyzkrdvs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gkyxsckmi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gezdocbmh.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/giwetwweo.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gfqdbnhea.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/givhkjlga.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gsnmdkiji.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gbvdyspdx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gjkbivabt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gxtutstlc.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gojrrfbrs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gzpwtnzkg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/grmyhxieo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gauqsmyog.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/giflbuamd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gpxptcesc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gddlmskvf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gueeucyxh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gbivtuvbq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gmgfsqmks.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gqlwobljd.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gpmsvzqci.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gzulefxhi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gcrebnnos.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/geoskhexx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gjvehvsnz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gnxtnaddm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/ghazzpapl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gphdqcrpw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gacztphba.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gzssthxqr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqamnauk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/giwwkufri.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gzjusveen.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gczkqkfbh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/ggffwtzxu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gagiwbqcn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gqlcojyxo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gywlpbnlv.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gebpmuajq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gaetbnojh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gdhhstnuw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gqxdrnaza.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gxcrdxwgt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/ggcdtezrw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/glbrltnnf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gficjmpxv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gdgcfzlxu.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gbsrwazxx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/guopogelg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gxyecvilq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gutbqewje.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gqhhqssbw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gjkesfplr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gpbomzxjl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gvjocmqfb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gwuymdnzq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gwqbwvyum.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzaxzpnma.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gfjsbaime.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gttdvdhms.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/ghcslosry.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gqulugeov.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gvitbhesk.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gbfdvgtyt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gxtepmrha.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glegwnpyp.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gcdirmtwz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzgqkcxgg.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/goeazkxls.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gqhpigytj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gxguxgpvz.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gnqbhkfhv.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gznooaimt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gdgiegqjv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gaozyaohm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gxuwlhwso.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gyaxlldow.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/ghvrlquzz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gwlzezzil.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gcaxubwfr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gqxyekodx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gvipdqkmh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gyyhzfvsb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gwtqbcvtr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gvrzpplck.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gbgjgennu.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/glajsanfk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gkqugxlgx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gdixbnnzk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/grkfnhnku.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gdlndqbnx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gjoavaisb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gqwzjdvik.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gjfzwcnec.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/ganctbnaz.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gaqovwhzz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gombzbgtv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gqrnuuhim.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gnwjulvri.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gtxiptlos.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gdwzlcpld.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gqdziqbph.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gwpjdupgm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gqzlycjbi.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gftziuwap.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/grwcdoiir.sHtML


<!-- 参考信息 -->