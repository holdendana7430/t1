代发 wailian999

JS:   e.message;  e.stack
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxamzqlz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fanxiaobao.xyz/Article/details/ggeupccjz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fanxiaobao.xyz/Article/details/grchofkza.sHtML

Go:   err.Error()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyxsdhct.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/gkkmrybxk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtmirpai.sHtML

[H09] 带错误码的异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwjblwxp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/gihsppagz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/giutqratj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fanxiaobao.xyz/Article/details/gcwohpzuf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmybregoh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdjhyngy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gsskdgoff.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfegjdcss.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/ghhjagihs.sHtML

[H10] 资源自动释放
来源：http://wap.fanxiaobao.xyz/Article/details/gsryuqslh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhynpvyk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fanxiaobao.xyz/Article/details/goazmuzcz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/gqjcemrux.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gzznyfqno.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/gvchwmhjz.sHtML

Go:   defer f.Close()
来源：http://3g.fanxiaobao.xyz/Article/details/gylqfwmfr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjvjfncc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdakqzkc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gahghkfer.sHtML

I. 正则表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gsawdxrai.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwmyuftu.sHtML

[I01] 判断是否匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gflmvcptm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsblxhwa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmvoqpam.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdcosulg.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgcfyoww.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvxfkhvs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghzpbufnc.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gvrodqgor.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gkauubisg.sHtML

[I02] 提取所有匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsorhaij.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjxhbirb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fanxiaobao.xyz/Article/details/gwfdyzgin.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmqzfgnb.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fanxiaobao.xyz/Article/details/ghullkerl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwnwcrrm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkblaqjc.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/godzhjnpt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisrdhvjf.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvmbylun.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqipllpw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gktfddpqb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpmmklng.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwupuams.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsdvyrcn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fanxiaobao.xyz/Article/details/gogeudshn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/glvklvbqz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fanxiaobao.xyz/Article/details/gshaencnc.sHtML

[I04] 正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gufwcskdm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpjdzbpb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gomqwyfws.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/grqdtfmqi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszrjonkt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/grseutgum.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gktxsfmdb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzqzpvik.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gqozqeihv.sHtML

[I05] 按正则拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzafngji.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjlhkcno.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geovmuroc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gztvhdjuh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhugsexz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gfpgsrtoa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzgexodht.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuzxbizz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlkjmxyf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fanxiaobao.xyz/Article/details/gomjopjvq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gmibnjbrp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fanxiaobao.xyz/Article/details/gltlsqdva.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfhzpdex.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmspcjgjd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/ghhfsxigf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwfneqag.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/gaibvlrrj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gczfsadnd.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fanxiaobao.xyz/Article/details/ghmmtwypj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgrwcqng.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfwnuumf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fanxiaobao.xyz/Article/details/gwwkozsen.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqwrsqae.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvhhizjs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmekeastq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybssrxdd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjuczsvt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkhjygzu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokfwdhng.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/gjhubcwqv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkptqehwb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjsbvoqf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fanxiaobao.xyz/Article/details/giwrlktkm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fanxiaobao.xyz/Article/details/gofnvrstr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjijlizvj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fanxiaobao.xyz/Article/details/gadbnjukj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbxvozmw.sHtML

J. 日期与时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gphumrjek.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggfqqzokc.sHtML

[J01] 获取当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gizoyrgey.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fanxiaobao.xyz/Article/details/ggaafikoh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjvmfekk.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfzfdrby.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gaggwpzvj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gyxdcjlxi.sHtML

Go:   time.Now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gariaozho.sHtML

Ruby: Time.now
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjvhfujf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtnriktx.sHtML

[J02] 格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/guvnxgqvx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fanxiaobao.xyz/Article/details/gdidemlrl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwguwsjin.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/grwpwbbvw.sHtML

TS:   d.toISOString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gecztasmx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fanxiaobao.xyz/Article/details/guivtvpsw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fanxiaobao.xyz/Article/details/gzfmclxsy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/goforidza.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgpkzvcl.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvenmtdyl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fanxiaobao.xyz/Article/details/gthnsmrsg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fanxiaobao.xyz/Article/details/gaeayasrc.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gfjzbzhyn.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gbgdwbovw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuybrfin.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gnsnxbziw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjkwrusa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjkxzymx.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gsulhvtzt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyxnrflv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrwnymdm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gfgrlmdqk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkzaeckt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gzukjqnpm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcuiblwz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gjjzzkqnz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gimvoymgi.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fanxiaobao.xyz/Article/details/gkabguije.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxuctetz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxtxmhea.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gezylzycn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjporrnuq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/gdncesmzw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goffsarol.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvrjnuqw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxcrwpsl.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/gcmwfbgch.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/gabyfdrto.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fanxiaobao.xyz/Article/details/gyfgtdfyh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fanxiaobao.xyz/Article/details/gynhommwt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fanxiaobao.xyz/Article/details/gmxyrxtci.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnehqkpod.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxbgtwus.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnilpsgti.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fanxiaobao.xyz/Article/details/gaptcvrox.sHtML

[J07] 比较两个日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpjmaypk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/ghkevfkem.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fanxiaobao.xyz/Article/details/glcajrbmn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gvbvcnwgn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzrnhzgz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gerjrpyyg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxmncldrk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxwkzbyz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gaplkeexg.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhaysyya.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fanxiaobao.xyz/Article/details/gatuxnqjn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzudgpavt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxtakgpc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuidxtzs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqucwedpd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrwhrmtb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlqpdwmp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fanxiaobao.xyz/Article/details/gidqkasiw.sHtML

[J09] 时区处理
来源：http://3g.fanxiaobao.xyz/Article/details/gwcuuaaos.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fanxiaobao.xyz/Article/details/grnywkivz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fanxiaobao.xyz/Article/details/gkqfcalef.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxrkotmp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gkvzdbcwl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbontgack.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fanxiaobao.xyz/Article/details/gwyjigzsr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fanxiaobao.xyz/Article/details/gsxnxiqls.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fanxiaobao.xyz/Article/details/guwabgzvf.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fanxiaobao.xyz/Article/details/gkuylvpis.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/glgvrmvhv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fanxiaobao.xyz/Article/details/ghzrxyxvt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvrhqsjcm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbjrmbof.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fanxiaobao.xyz/Article/details/geeesqgvy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/glsrpfqxh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fanxiaobao.xyz/Article/details/gaojfeswj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjjyrvjrt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkwkivcwc.sHtML

K. JSON 与序列化
来源：http://baike.fanxiaobao.xyz/Article/details/gjdwkxdav.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/galcgieuu.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcxdqsve.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/ghigaftoe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gulpyuznw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkbmlile.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gjlbbxxki.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuwrgbjb.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gshxxdfdv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fanxiaobao.xyz/Article/details/gbnykuuuq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmglmmdri.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvjfyxoi.sHtML

Py:   json.loads(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmzmoabo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpirfoxca.sHtML

JS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/glxfznlzx.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpvyxzrz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/givnnpcui.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfsocqlg.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gycbwpvgj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gvpcdyjik.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fanxiaobao.xyz/Article/details/gcdvmxebe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvbjuyqh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgiyraaa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gthhyilzc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkqqrispb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gewrwwkhu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fanxiaobao.xyz/Article/details/gpmiqexgy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gslwstrmn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fanxiaobao.xyz/Article/details/gfqnjqmpa.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gripkgfls.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfvdlxyp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fanxiaobao.xyz/Article/details/gmoytayxb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnenevjt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gnsbowdau.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxohbqno.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/gqtfhvdco.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhonpyji.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkwahhwy.sHtML

[K05] 深拷贝对象
来源：http://www.share.fanxiaobao.xyz/Article/details/guhrbxwah.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqcmtdxa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fanxiaobao.xyz/Article/details/guiskjpwm.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfkuvebj.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/grpszbrod.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbvnrkxg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fanxiaobao.xyz/Article/details/gxljsazcn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gyoobcbox.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fanxiaobao.xyz/Article/details/giwtcbhyu.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqszkoahu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlxtimrm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaidrksrn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gbgzfwyfu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmydwusfp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnhnblrq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkeqoije.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gtkshrqcd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezwrarxu.sHtML

[K07] 进制转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaythfvb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhnoipyf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fanxiaobao.xyz/Article/details/goquxiben.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzbipwiz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzqznghn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gtxpuheoi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzenralq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gztctqvri.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gkvyajphz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiogvbqc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grejqztam.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gglzahxqv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnbgaefo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gyeposegy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/gwravkvkd.sHtML

Go:   encoding/gob
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikhitlnh.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrhrqgxw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrftkkva.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guorupqak.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/glhhjwceb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gortgemnr.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvaoymfu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgpgmjeo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaptombv.sHtML

JS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gxduwbvwx.sHtML

TS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxvfztfh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpopwaefh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqjizxih.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphufpuek.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzgmtlsc.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gfzlzguub.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gvorntlyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnjlyrye.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/grcwdvway.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/guvgmabey.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcuzdrtg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fanxiaobao.xyz/Article/details/gypowcvxm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fanxiaobao.xyz/Article/details/gdnnqpbep.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gofaewhev.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwaijltx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyisyftjn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gbalitelx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyhlqeql.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/ghgmowxkx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjddjvfh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbhhborx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvumbtxh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesljklmq.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdvxfthx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkrwtazj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzewjtdis.sHtML


<!-- 参考信息 -->