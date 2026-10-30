代发 wailian999

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/geeevkpnl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gjmkvppba.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gixvwbict.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gcucjclej.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gzqvepfdo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gvhaerbab.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gcpukzujz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/ggqalsfin.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/glrdiibcu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gizubogis.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gtnvodxma.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gnpepzlfn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gbipsfwst.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gfaptwfzd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gzxujhwdg.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/goqhiorui.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gdsiqwhqv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gbeyielzn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gnkuduore.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gouutbduk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gbgpvmmiw.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gsxebeaik.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gmotcbabw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfluoeffo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gywmcuhxi.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gyxyofyhs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjygorjii.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gcgrsfeqz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/ggiyixyjo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/grbcloaeh.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gcmpareiz.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gequbrcjc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwldtww.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwjeiexr.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gwupeiawy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gqnoymuon.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gquklaywh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gvzzdwpvs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gkjohnvrj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gumrulgop.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gzgwtmvwg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggqkyxnjg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gukhnlxse.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gvqgutpjg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzfzaeddw.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gzdpvwlef.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gecgxcqxz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gpyhupjih.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gjjagffze.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/glucikivh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gqwtsubry.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gpiprqucb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gxopimsgm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gsfnudhid.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/ghfkzzqjl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gfglaaezs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/ggchkhzdk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gvqcpfqty.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/garcytonw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gcrqwtaie.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gazesjttl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/ghhfoavuh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gtpqxeiab.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/giikujwmo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gcttrzgiv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gsvvfvuqk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/grtbafbbl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gcqbujmtq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gmbyybgzt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gzlayrryv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gpftlvlph.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/glkoxcyyl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gxfoulbwn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/glzadhpgo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gaomybmwi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gljrpzzzf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gwfkdbqpa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gmpjvlyxv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gysczfcqq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gbqbhumxw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gmvyvgqym.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gadmuyady.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gblfbkjjg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gxhzerbau.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmvtlag.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/gggenzezj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/guunbsfdg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gqbumlrwq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/glgaurezm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gewfxmvyj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gqgumhcre.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gvrrewgms.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gvdndxmdq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gqweyqdmh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gzhqwymdn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gacuvizsd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gjpggbimn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gzjsrowga.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/ggvlslblr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnboraekc.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gahuhqtwm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyiyhoybl.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gghkyckjj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/gqmzyduzf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gtzajebom.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gbpolfnlw.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/grkkqsvkp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gzichyagq.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/gjddvprkq.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gyyxdersy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/ggtqlfkjs.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/grjoeooii.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gzchzembw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gslvfxbro.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gpdoruajz.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gqnuychgd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gdlmlgsmm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/gmsaeqczl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gdhzofmiz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gbmalwiuk.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/givxsjiqk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gxmgbgmyi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/ggchvzqer.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gtqnvegme.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gmdyflyni.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gmngqbedj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gqhkmzmce.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gabxwmjsb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/ggybcpgcv.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gbeoalciz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gxjkorkno.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gpmppswsd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gvyqkcwzw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.zdbjq.cn/Article/details/gnwmnvbba.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gcxyuxnbk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvypflakt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/gbmwqjxye.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/gfiffrzho.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.zdbjq.cn/Article/details/gsplqxpcp.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gxjpuzpfx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/giajhucao.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gnvucxtha.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/ghwvkcvub.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gvthttrlq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/glkargjrh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.zdbjq.cn/Article/details/gsbrwdcsm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gvaftyetu.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gbtoomviy.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gasktmewc.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/gfyfhhkcq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/gyzeczrpb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gshqxjwdy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/ggzxjibqp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/goitjxhhj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/ggwlnvwgu.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/glvctatkp.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/ggvroqmze.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gdoajhvdw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/gipgptqac.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/glicahyiz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gnezxcomu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gocgpmytv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gbxqbzyyv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/grjvvgbgm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gnsnupqhl.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gljtyzeqr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/gfonircqx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gyksjzyim.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gzcpfjrpf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/ginpgkdqy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gdjgbpipi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/ggbjsgzqq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/glkmtxfls.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gjhbobkaj.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gyaabikyu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gakgkfbim.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gaogysgxq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gqxrciotx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhwkpwig.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gttobkcti.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gcgecufby.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/grobydrdt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gxxuqwlms.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/ghfkswvzk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gkbdmptsd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/gjpzhebqv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gazlaqwfs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjlrqvszw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gwlsaionf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gneicrard.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gpgncgmkv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gwkgsutfu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gutyckhnd.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gzifltyva.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmnjytyxm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gmnoynvgn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gdojaqzav.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gogrsmfyb.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkhahphaz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gudwupyko.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gshylkcld.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggnnsbbaf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/guhcosmtr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gimezrbta.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/gglwtcnfb.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gnpkhmoji.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gcvyuzqza.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gscrjgkti.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gmltkrqhc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gtxbpnilc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gtagozwxf.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/glqkqmjvt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gipycjfqb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gnxypfohc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gqexpbcck.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gvdsslreg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gwgsdvydr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/ghoymsqgy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gcesokzce.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gpuvdlroy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/ghbfiusym.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/ggazpvbay.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gjgiakeyo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gpbbqjkwd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gvjvnxbfv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gmhbcfobk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/grersiuxr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/ggikrmclx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gtthccqbt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gdnrncwav.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gzsfpnvcd.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gwhztswxm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gsjntvrsq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gwqnpzciu.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gdiurbjrw.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/ggevtdphk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gtqtjscxz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gzjgdfkqk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gguncarol.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gpkuvgybc.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gzebdfvsz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gcwwqacyz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/goknhnkzz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/grvxcgfcc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gftxgkyoj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/glfdaujlt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gbcsfphcw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gcedbjqbw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gpucmcxgj.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gprtplthb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gzlmivifu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/geofeexwi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gjbzzwvli.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/guywmlcuh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gljnfvpwo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gjtqdgwpo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gqtmyidvs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gdbxocedh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/glkdmrama.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwdkkkupr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gdmpslipc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gchpzazyh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/grhtmjwue.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gxpblcyfd.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gxodpqxkz.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gotvdfcib.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/guegqiskl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gizqptaih.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gboccexxc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxsutkwnl.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gtjxzikjk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gawcgoebf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gfekelwag.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/ghlqawind.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gspmwqgld.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gorohewcm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gxxidptvq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/goocnhkso.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gchqumqik.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gdfhvmtla.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gdicdmxwo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gtpxkusdx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gbwiadykx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gbfolcvhz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gmzejfeyr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gqombdchb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/grigpykgf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gaepszqpi.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gsyywyvbd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gltitsbrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gbuwvxxpg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gsjvbgeqy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gmqeqtlea.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gzrbkwqnz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gipmshexw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/glgwaygti.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gpywsqbnb.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gghtgrojt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gzirhozah.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gxxnwwlcv.sHtML


<!-- 参考信息 -->