代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpyyvztd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fanxiaobao.xyz/Article/details/gjnsdzowf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fanxiaobao.xyz/Article/details/gbqndbacr.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxovswvy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkzrlzmv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fanxiaobao.xyz/Article/details/gnxmvcmzy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/gxecyfmys.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gjakinlgt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrgaqsqs.sHtML

Go:   defer f.Close()
来源：http://baike.fanxiaobao.xyz/Article/details/gussvifkw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fanxiaobao.xyz/Article/details/geoxnmvun.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrkbrfre.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbqktbka.sHtML

I. 正则表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gefdlxhsl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmmysdez.sHtML

[I01] 判断是否匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gndfliflp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/goubfiwyc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclspdxwl.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhwzqmud.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaythxufa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzosgroai.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/guccwwzhb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsbrrbcf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gdjbfhyvz.sHtML

[I02] 提取所有匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gjkabszbl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpmcsqfew.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqbqlekk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fanxiaobao.xyz/Article/details/gneksmatt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gonyeuunt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gtrqawpat.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqpknlxl.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtknennkg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuhenmjt.sHtML

[I03] 提取捕获分组
来源：http://3g.fanxiaobao.xyz/Article/details/guymwglis.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gpbaucbxc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvebfpcc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/guqstzszu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gvhqqyejd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fanxiaobao.xyz/Article/details/godcdxlsl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfperguh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gebuzbolw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fanxiaobao.xyz/Article/details/gmozzpuve.sHtML

[I04] 正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrwzvhhw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvroqfowj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gxawcwhqv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdtynyzf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqqexctt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gnpqbjdux.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvxkcinn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmujzdpmw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwgcgwzn.sHtML

[I05] 按正则拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gpdyrvuto.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiddamev.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/grtnjsike.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gkugpbvyv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaytmeix.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gwwkayjdl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gncyevhyk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhzgfddo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmftwjzwf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fanxiaobao.xyz/Article/details/gnoyygesx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulbzzawf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpityrhp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gpypinjrk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fanxiaobao.xyz/Article/details/godczvaac.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gwuggkeat.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fanxiaobao.xyz/Article/details/gntxqdrhd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fanxiaobao.xyz/Article/details/gzrdizuiw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gaowgpelf.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fanxiaobao.xyz/Article/details/gjokytcfk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfusseauk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmppeanl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcwqorjt.sHtML

TS:   /error/gim
来源：http://3g.fanxiaobao.xyz/Article/details/gejwgfgjt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fanxiaobao.xyz/Article/details/gmntwygtv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fanxiaobao.xyz/Article/details/gtbycmmbb.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlayobvt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgbsgazh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlxgbrra.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaojfhto.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gasmkuhzp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/guxibxjiy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsupjkznz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxvngicf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fanxiaobao.xyz/Article/details/gsudfoipm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxgzgbdo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gqltucjxe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glcvgswqd.sHtML

J. 日期与时间
来源：http://baike.fanxiaobao.xyz/Article/details/gxhlzuctc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmucewilr.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuefambr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzzfnpyz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/girzzfkcw.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gfuhqxthp.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvagymhkj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gncognsoc.sHtML

Go:   time.Now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gliugkfob.sHtML

Ruby: Time.now
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnpztqjm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduhdsofd.sHtML

[J02] 格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjbjcuee.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbahtuaq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gacbafzpf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fanxiaobao.xyz/Article/details/ggopgblav.sHtML

TS:   d.toISOString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxgrempz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/gokniphen.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbegiujy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnvwurbl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsxvrloa.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsgrxero.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fanxiaobao.xyz/Article/details/gbnfokyrs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmnqxeds.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gjcmpyzlo.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gxwuuloto.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbxfmtzx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/greuhastk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/guodxclad.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabetgsxp.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gmasohoeo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gvucbgapc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fanxiaobao.xyz/Article/details/gojdmyqub.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecrkbrkz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gukapgemh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakkvawir.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gkvscyeut.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvgypqbe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcunacrkw.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhpktcxu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtscdgqjw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gczyeywsl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlzcrepc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcrlibrz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtkfwnxo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gstjuqiqz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fanxiaobao.xyz/Article/details/gcwxwqrei.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/ghylsmsuh.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/ghkkdavrw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyurinqqf.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdcwrebf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fanxiaobao.xyz/Article/details/gvesypkxx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fanxiaobao.xyz/Article/details/grkjptmjm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjqjbiz.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fanxiaobao.xyz/Article/details/gawunvwzj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/gngoqmprd.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fanxiaobao.xyz/Article/details/ggnxgqgrh.sHtML

[J07] 比较两个日期
来源：http://3g.fanxiaobao.xyz/Article/details/gjwwapmkx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gdbmfviyo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fanxiaobao.xyz/Article/details/gfxnggyoy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gvvlcccuv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuczavxr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fanxiaobao.xyz/Article/details/gxdwckbuc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fanxiaobao.xyz/Article/details/gasfocwyt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrqadawb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiunshos.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfjujsvg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fanxiaobao.xyz/Article/details/gfacgljkz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fanxiaobao.xyz/Article/details/glacitsvp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fanxiaobao.xyz/Article/details/glmjhirat.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnreugqju.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeerrvua.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fanxiaobao.xyz/Article/details/gcywolnni.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrlpwxhd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlvmixky.sHtML

[J09] 时区处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswvudmmg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjangdmy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkaucvht.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnnyirps.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfmlfngz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fanxiaobao.xyz/Article/details/ggbbnokfa.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fanxiaobao.xyz/Article/details/gwtkuwvxu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfskksvz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdbyyodb.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoclffdu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fanxiaobao.xyz/Article/details/givfngyhm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fanxiaobao.xyz/Article/details/gztffbwir.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiififvz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gnjpwhvos.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbvrulpe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqsncydl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fanxiaobao.xyz/Article/details/grtpuucgr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpmlrjkn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbwescfv.sHtML

K. JSON 与序列化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdciglgen.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbepguzsa.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grqqdrlte.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gnlbdulxh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/grsmdceje.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gwosngpex.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gbvypfjys.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fanxiaobao.xyz/Article/details/gnooopsta.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glahgurqs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazpdacia.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbughfdkm.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gcsbuewzq.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlpgdthu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fanxiaobao.xyz/Article/details/gknbwzmmm.sHtML

JS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghrhyrpra.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvvjzuro.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptbbnhio.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/gykzgjbzq.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/goeiqmxxi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goovlycxu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fanxiaobao.xyz/Article/details/gbrhgzkvf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gjischued.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/ggroyvucp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckxaagwe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwzikglyh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhbkajvi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqntnqwe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gqbeaacdz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcynbbua.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfjhxzouv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gxbexekhj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fanxiaobao.xyz/Article/details/getpscrps.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqtrkvhp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gdqpuxclk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gmrxrkhmv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrttanii.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gghzlsliv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmumumlg.sHtML

[K05] 深拷贝对象
来源：http://wap.fanxiaobao.xyz/Article/details/gnmzglqev.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gseceqfhr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fanxiaobao.xyz/Article/details/glzvytbpq.sHtML

JS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gxicxtblg.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrpbpuwy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fanxiaobao.xyz/Article/details/glezcokmy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fanxiaobao.xyz/Article/details/gnytkixng.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gulspoxfy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoxajlnw.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fanxiaobao.xyz/Article/details/gapwzcjuc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/ghgfyhfux.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfnmivdx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/ginienvdg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gtkebbwfh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/ganzvgswo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaqqfuiy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gdxshtttb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gukupgcpx.sHtML

[K07] 进制转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfxkoncr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbpzkpxk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fanxiaobao.xyz/Article/details/gdsfkzhzn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/goojxijng.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzxftvli.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/glcvhfkid.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwflfqdyn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fanxiaobao.xyz/Article/details/gshpndfbj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyccmkjd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhimrjva.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobhxsivg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpwxgtob.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gfiqvpanl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gngbbzqfz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvalykvow.sHtML

Go:   encoding/gob
来源：http://read.share.fanxiaobao.xyz/Article/details/gtupmjcdk.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gobipwhla.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfkdtusw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvnjazcqf.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/gisnqdnkn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdggtngku.sHtML

[L01] 发送 GET 请求
来源：http://blog.fanxiaobao.xyz/Article/details/gakwclwkp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fanxiaobao.xyz/Article/details/goiyzmnhr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuqboyld.sHtML

JS:   await fetch(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwhvigok.sHtML

TS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/goawspkjk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqkweqdv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwthfjhc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fanxiaobao.xyz/Article/details/givjljmmj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsafdpjmg.sHtML

[L02] 发送 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/ggsywowsk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gbipvjbjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhvqlggm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/goimqwhrk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gonwfylym.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/guipduhdw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvtgizwp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fanxiaobao.xyz/Article/details/gbvfmaimf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gsylsnkhz.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fanxiaobao.xyz/Article/details/gymvowgdh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fanxiaobao.xyz/Article/details/gbxkubsfc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuxrwtxk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fanxiaobao.xyz/Article/details/grneybvns.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gaqeszgtt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawgwxlrc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxifnsyqq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfwqiqoa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqephsnfa.sHtML

[L04] 设置超时
来源：http://3g.fanxiaobao.xyz/Article/details/gbcmbddsw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjvzpdtd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gghzjwpga.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxnvqguz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gmrhcrfyv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/gxwopwrbj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fanxiaobao.xyz/Article/details/gaveluvib.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwyapkmd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gfsulzjpf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fanxiaobao.xyz/Article/details/gneqpfxwp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpuiejbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fanxiaobao.xyz/Article/details/gadgziulv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusfvjckq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujnzlhsa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpbzezrk.sHtML


<!-- 参考信息 -->