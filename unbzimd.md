代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gyhxlaqnq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gbxapquys.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gzrprwhhx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/ghnqyoaiu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gfhawflyv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gzhltnspq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gixlksajk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/grzmgjrng.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/ghmkzpmxm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gxlqodmue.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gpeqopmte.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gcxkirglm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/giqhwpbwk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gqrubqajf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gygqieqva.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gecpeauog.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/geqtlnpzw.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/giprzdulr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/ggmxxmnbv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gndmlnabf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqznjvwsx.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gikunbstp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcvqsclgz.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gzqakihnj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/goijpvldl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gdehlztqn.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gzrszcciz.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/ghjqhebqe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/grdpmxqjy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gtubhezod.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gcqopevej.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gmaphdrgi.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/glztdhfbq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/goqnnkysf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gjhzmxgxh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gvwiaeiuj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gtilmpfhs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gebfxtfou.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gbnuyaafh.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/goccjjdek.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gtnojyzkc.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gmebxcmis.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/guhujzetq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gkoyybvbi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gowjicjux.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gakglawwi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gnvxrffxi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gjicjnkpx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gzmmzsdjf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gtdrskyaz.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gpvwdmrho.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/ggqohslxw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/ghzpnqono.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gpiddsixe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gkfqpavgz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gxfwnshjf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gclymuqnh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gnyyuzxmj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gigbaujef.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gtyijbgpv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gucretbdv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gapipfgqc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gnjtabmwf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gpcacblop.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gvrgcrasn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/georqgglw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gdykpomvl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gibebwdbg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gfyurhhlq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gpyxsjbre.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/glmtkzuzc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/giwkhgenz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gkhwkhcik.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gnfbcsxbv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gmguskihs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/glfwveugp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/glexcffex.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gwmuboyyj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gytxalidk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/guwjxkczt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gsqcckyrk.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gxcpuemfk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gjaniblcb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/glxijahvy.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gbnuvhoie.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gcgeczuwg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gihflhcyj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/ghrqmvhle.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/geddxmqqu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gowjufchi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gxdvsvkal.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gmeqnkuws.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gszzgdlcz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gungawkrx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/ggnqaxyzd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gewtqbmnq.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gsiwsdyfy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmloakhsh.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/geidnjjjf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/giahjlmuo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gdbphzvsv.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gzecypetu.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gmibqeply.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gxzdlipgi.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/goaczavbj.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gajpgacsm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/ggloyoybb.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/gwmrutqjl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gdnrvlydc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gctamyzbb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/ghrfhymyx.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/gqqvdegnu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gdnzhcztc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/ghgscetzd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gqguiankh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gqodnmhyd.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/glhixoacq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/ggnqycajw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gjybzihsn.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gpcednixe.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gidslwmvv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gcoxmcdyw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gwndxtsir.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gimcsussa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/ghufubfef.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/gfuzqigpe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gxhwsuqbr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gzuxjepjn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/gcyokmeeg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gsesrumil.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gzdobzcgt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gepdcfnzt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gpoqnimvv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gjufputsm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/gcipchrlc.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/gxaeyetev.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gnyprozct.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gvmyswqhw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gtsuqznbi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gdcttgzms.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gmbsolncj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gguilqmrz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gsarncfpl.sHtML

[J06] 计算两时间之差
来源：http://mobile.zdbjq.cn/Article/details/grboxbxen.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/gtjvkiirp.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gdgsbykhs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gyicqzpou.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fehbvm.com/Article/details/ganhblpul.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/glxjxcfej.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gkazzlwvr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/gtyoelprm.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gjzfptwor.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/glbwopxqn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gagemfmrm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/glqzcdewx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/glcvchaxy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gzbusvxqf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fehbvm.com/Article/details/gbdzsddxw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gotvxrkst.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gtvhkhglb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/giyebgpri.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gjetfojhd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gnizaentl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gtvuqiuih.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gwplrqybc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/guwsndqlm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gdrbenuzu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/ghmlhxaos.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/glewrymzu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/glyvkwemp.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/glqzcdzdo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/gsvfuoliq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/gqgyeqtky.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gqwqvouvc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gpwxfafpr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gbgckwamx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gvwfasemr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gouedhaao.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gcigldeoo.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/guerbxtrb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gxunrrxvx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gnnlisiuk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gzygeaekh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gvimviibe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gchjhmkhg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/grzkiungs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/giquemdiy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/guhzruqwt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gancewhas.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gzmfdxgom.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvyuqiqde.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gkwzsjjyh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gyqnjrfsn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/ghrcsjnuu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gamumexzh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gxjbcpyln.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gibqnlkqs.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/giydjmqsk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gmaulwjgc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gnmbvypzo.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gewvpddje.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/goxmdyxkw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gjbekmdub.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvhnjabal.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gbvaepvpx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gltdrcxic.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gmtxgubxi.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/guslvfpay.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/guuoigeuo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gvclddnvf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gzzjimves.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gdhwlvuhm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gixtsdsjh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gropjhhqx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gflfcsszb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/ghthbuqtd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gufyrrizn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/ghifegnwk.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gbbdhrtdh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gubiaxkqx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gqambxbnk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/grhilujyx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gqlxgnpce.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gdewzzziz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gidswyrwl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gnytjrbjm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gauygegyo.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/geqqoctgs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gqnjkxvbi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gedmztxcd.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvaastxbm.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gywejoqsg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gsqewdmkw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/glwybniml.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gmzsrolbt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/govropesx.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gyykjerqf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gvrsoxkfz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gamxopqcw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/geavzbqma.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gxcpfysjj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gtwhpdwsu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/ghlvlenry.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gwjjqyerb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gptkxjfra.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gvpuygluq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gptvzwfzr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gezyxsgub.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gvmtwkkoq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gqmwjfjfm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/giajaomfz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gmcnwubdt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/ggwhtgxwg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gntcncpsp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gryhqqkre.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gacwmjrcb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gbitqknwr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gaqhmitfs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gafnahetp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gfkxpqlta.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gcverxowy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gztknljqb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gaohyuvzf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guyfiqybz.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gpnqxkgvl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmrtcngql.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/goljbuphg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gvbuatyfn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gyrbsvlhs.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gujqcixnb.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gikntnriw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gwytxklmk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gvbmykbmj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gwvqiljji.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gdbymplvx.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gmfikisds.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gpddwugnf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gahafttnc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/ggdcfdevx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gcqrtfzva.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gohimuzwq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gupizqayb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/ghnhkjxzj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gxohaxopm.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gyjkslykx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gwkifiknk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gtwzdedvz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gfsiavfja.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gpbtcogxw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gxradoxtu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gvhagexkr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gejsyhhpb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/godmquzst.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gjwfzwwyr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gekruqsyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gayqmvori.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gaeuoqzcs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/grkwlgjva.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gfrnoxuxi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gpjodqzyr.sHtML


<!-- 参考信息 -->