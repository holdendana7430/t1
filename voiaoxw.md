代发 wailian999

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gzpkklyrz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gxbzemcxu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gtjypbihz.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/ghkrecxqe.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gcbvfbbcs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gnzefcibb.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gtfsoqhzs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gxjokbfxx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gdcjlmcvb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/ggmjcsndf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gstcftvuz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gnuetgrbl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gewdgixbs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gfcjsorpk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/grizcwlug.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/grffxaofk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gebkucfdg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gjmlckjph.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gjsenmjnx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gcncvnlvv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gwbhdrtwl.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gjqfmmqis.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/giqqxzutr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gtucwoiik.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggexwvcwi.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gvppblfom.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gczfodlib.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gbtzwjtkd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gcqsomfrn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gigpjpduh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/giwotfjdv.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/ganzdeafd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gjewlzarg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gifgrmqna.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gxwnoizxm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/glfxxetps.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gyegryzdp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gcqcbceeq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/ggehwyrwo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gnwmxkzrz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gslelawxa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gmkeziazn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/ghblzuuoq.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gfbckqkpy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gwdcyqpex.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gyezppklh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gufiyonyn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gjygbasjh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gyqfquhsr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gtvnahamq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/goaguvumf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gvskhnmpf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gtffprwqp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gcuedgjvv.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gjrzrmizj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gnnwsatre.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gopmqjxjv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gcffqwrls.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gohhzxvts.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gzozpjxzh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/ghrfazxts.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/ghwsinzct.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gcncqcpjd.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gmdvhgirs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gdgpogilw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gislbkscf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/guejxyqgy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gkfzvddeg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gsjsfwybw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/guzjcafrk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gebhzmzem.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gigayqdzr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/grwjshrcz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gdcnmegct.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gllncuxpk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gesgazaqf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gsfshjzxa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gkdgdaurt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gspttgroa.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gaqiomytj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gafpdpvxp.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gddtfdqam.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/gxaprzsgk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gaqhhladq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/gpgyzipxb.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/grgtqpifh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gvudrjmgy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gyiikolbn.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gwcpxajhe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gwhdsyzpr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gccdznyvs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/guavogmjo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gsmmkytzs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gpplxxlur.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gnmuunocg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gokenqhxu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gjpopegjl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/ghdlvkrvk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gnhfpexni.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxyjlgitx.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/ghappyyyl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmrwxemft.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gaxlddjdu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.zdbjq.cn/Article/details/ggvqdmman.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/godazdssn.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gfjhlxhdz.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gtfrgybwy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/ggbtjcqov.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gsczektgo.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/goqrdltpy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gkvmqqipp.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/gwjtylavs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gblbijcez.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gdeelxelc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.hesvh.cn/Article/details/ggikpomum.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gkvxytjat.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gwhtkilcs.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gojwhgnzv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gudcmvymf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gtoillcvb.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/gykxlxxgm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fehbvm.com/Article/details/gbkevvocc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gwnqjqchf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/ggeahirvw.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gurefbksi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gqyqqzilg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gsyfrfakx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gwigvgfze.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gyxyrfeii.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gglfykapy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gypghlqxd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/giwdotjkl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/gcsvbaofe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gegvpijac.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/glmzmlzpb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gummznsyq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gmburdery.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gwtxkdzvx.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gqvofzykn.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gfpupingp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/gpylqwerc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gcylujihf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/glxcnfjae.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gbfitodpu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gtfuiysix.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gtmksgnxr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gcaeqtasr.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/gdyeclfgw.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.zdbjq.cn/Article/details/glyguihte.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/ggqbkcogo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gsrzfyqdf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/ginautebm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/gbxgfdukf.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gntmhywdt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/gwlraonrr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gzsxwfqtg.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gmpqrflfe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gjzvpitli.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.zdbjq.cn/Article/details/gjrbhmvcg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/guqaujoqc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/godbntbfn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gedzqaput.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gwaokfztx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/grxpishoi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gecyotyqb.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/grezncuia.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gtfdalmih.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/gupqvgeps.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gnduoqora.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gmzkyoshn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/guebadprs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gwikmvogk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/grqlpzavu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gwatfjkui.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gnuxpuvoh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gvcqkolxz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gxabxptyb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gikvqjmlf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzrblnzq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/glnabtgub.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gfommbjmx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gzklmcrjk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gkzqqlbrj.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/gusmydzum.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gsodajuzc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/gusoxwnpm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/guaqxctvk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gohglazqp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/geydoccjc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gfoivhlbj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gwysxfonq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gxuwcyany.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzvcqquel.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gcqgdgxmz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmahxagpa.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdenjlzmp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gbfowhnca.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gobtfxdsl.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gddapgrpq.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gqqighkin.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gxkaqxhkz.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gzkjukzfh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gxnxleojt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjpihlnpr.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/ggsxbgqkh.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gorjxxoao.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gruxdxspt.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gmhhpbivn.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gfeyqklaz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gdojajytl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gfujhwnes.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gfobcelmk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gnvznmuap.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gskyrlslp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gewsucszn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gqvxnhmfn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gengvwpys.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gfzlqsczj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gdgwvmrdl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/grigalfmm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gtijyjvjy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/guvjheckx.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gczonickb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gbuzjrely.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gnisshivo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gofjxfefv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gsuhzukid.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gullhckov.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gqggddqbz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gnfespowa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gcudjqhtn.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/grvkowesu.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/germouyfn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gfijkyiwu.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggggpdfjq.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gjchnqasb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gmuutmujf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/ghpxqzvct.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gytysdtjd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gaggrvfoj.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/grcteccxr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gxgyuhoqn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gcjqljqxs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gsndjhdnb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gnqeilkev.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gwyldxptb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gyoekipmt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gxdvpjqrq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gycjkbpli.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gyiysyayr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ghgztdvwg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gqnhmviuq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gkaqwdxry.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gxgmxjtpz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gdkxiepoa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gcgezmbpa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gkvunwebf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ghjpyvtyl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gnyvjlbxv.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/ggilzqdvp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gjjzbdjre.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gyrxpiefu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gwszymgrm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gdhedqycm.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gqqeewtuw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gslisnbuj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/grlknfzaw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqudonwiq.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gpvibgfjo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpxeuxlaa.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/ginmeipyw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gqbwktfnp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gqabezoeb.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gvflgzseq.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gfjbscknr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gaesknths.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gofxqjamx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gpaxeitod.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbwlqksl.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gxlvfjbqk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gvceuddms.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/glqdnrwax.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gwqebzifr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/grbtcnfrm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gobimbeph.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/ggetitzvi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/goxjfiqqz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gelttnntw.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gwfjbtwqf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gxknojsxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/goymkzvos.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gsgitlhjt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gqgplfxkc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gzqemprea.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/giqdltosb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gohbzjohi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gyofxyhwq.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gcjfpbllt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gtyqgcsjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gwchjroms.sHtML


<!-- 参考信息 -->