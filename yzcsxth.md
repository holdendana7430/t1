代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gurjgaqjx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gdkwgjyuk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/ghvelqtbh.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/giecsuabf.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gadrsqmmd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gzoxzuyvm.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gelldtrkn.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gqhhzsfiu.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gsrrevtnr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gfvztxsgy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gpjgcsknu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/godflsvin.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gnajivrvk.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gtqajlsmi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gezrdmeag.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gwpughgex.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gbfbobmvw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gparnizql.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gkapwigji.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gcsmzaumy.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gedhfznmu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gosxqfqjg.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gtxdpnctf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gmrzztacm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gulmnovdv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gtigbhkpp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gtlaphddl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gjryezwop.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gijtgpzid.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gugbaqajq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gillpnfxg.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gonkuymhf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gjatkaqth.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gtmawyasw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/grwujorwx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/guonvsooj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gtjoqmugb.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/goekwnxov.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gmlnkpcyk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glupcwpbx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdyicxoku.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gglknxahy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grjemamzj.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gommzrvhc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gafzxddhq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gwkfumncz.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gtggxixof.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/goiwiehkx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gcbbjbmoy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gzyonbwkk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gpdbrqbzu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gguoifofj.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gvbslvihx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gzywdwnpb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/grgvzobqu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gobdfgyso.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gswmksafg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gnkpwdrnd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gvvkrmqzf.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gaugokyrz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gxxxpqeay.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gmdrqvnnl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gkihwjnih.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gvbmzjrvw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gaxqzbgkd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gzcxpmwqp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/gykrnmuoc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gzhqrsmxl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gwbfipfyp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/glzohldue.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gpfcoppwx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gizcugkuz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/govvnsfdy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/ggcbwtgvy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gtzznuvij.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gcdugnxrn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gvrkodgki.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/glwheosix.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/giuofvpir.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gfdzkfixn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gvxozhizf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/giewzvpye.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/ghcejbsqa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gzafpssil.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gawvhxayk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gujfsxrzr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/guncttklp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/gxqbutxmv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gtdjdyoki.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gzpqhvmrl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gvtqlldoi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/grvgycpjz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gchtlzuhs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gkhuuvddn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gycawhtcu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gqkjfjfad.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gmtmztqad.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gthxrdtqs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/gnkgygprp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxabecwh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/ghppzkize.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gpftqqnfs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gihamcdxz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gswagkqwa.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gqeccnnsw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gyhfcrpey.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/grnfaolyl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gwblkhkhi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/ghitdbili.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gxppcevgn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmfhgjyy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gapbkggxx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gwjufvkxt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gfajivthh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gxbbnemcr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkltniffe.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/glacoorxw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggalbhmwy.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gnmlchymj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gveqlfohf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/ghmdczhsu.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gowwsfqes.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gailvgmci.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gsldfueyt.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gshvmcmod.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gsfsmqbxu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/ggelirrjr.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gockcqkmx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gjernrwwt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/giqxofmtm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gmykxdydz.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gxqvqjrqk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/gcstqydiz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/ggpckaxhy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gwswffqdc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/ggdstgkiz.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/glpebrjgk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gjsfrxkxv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gqequzohi.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gjuwlvrch.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gythpwads.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gbwlcnzjp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gjjllnrjh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gqunllzih.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gldxpdooa.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gcefeddut.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/gzulplggk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gwvqfxnms.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/ghmlmxbbi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gtsvlvfzg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/ghtbeikyc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grbplprti.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/ggumnpizr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gjobzzktl.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gqiknvckm.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gdwoluqqu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/gjjblwnik.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/ghnloqmnu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gxrlywoxx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/ghhiholau.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gnmyuzwti.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gcptbwiaf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gdsoxdequ.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/grmyuzoct.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/grgcmktqy.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/ghnnocvbc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gciflhcmk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gphwrioiu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gsvljkrtr.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gwnurwrfg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gfqntuvhj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/gzzvcexcr.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/gulxnwyvs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gobgoixkt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gjwmfqpgg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gsnwyrkxc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/ggdklhles.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gbrmwsmdg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/geqpmkqvu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/ggaqroqas.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gfufsxjfc.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/ghzkjyvtp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gejmqxoqh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gpvooefsf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/geekyvsmx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gnjujfinn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/gquhhwaxx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gfdvwhaeq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/gyxdocqst.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gwnqcwins.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gisyicprh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gmlyeqeia.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gxqdujpsw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gajirmukr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrejyjlm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gymlptcwi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gekqkbhoi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/gajwywksg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/ggjoibvlj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gawqaizkf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gjorxnlnb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/ghtegxcmo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gmqttwzqc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gqnmfyypm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gpstcyaot.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gonbzkwfo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/gbkcifxzm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gwsyncfoj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwwrxlfrd.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/guetuvilf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdjjauwef.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gtydeppij.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gfxewrbcu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/ginehsgnb.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gzsfqnfej.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkrqqzef.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/ggzfenxey.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gcbavwjob.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gxxhymcbw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdnecdjxg.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/giinnorwu.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gegclrhuk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/goagplgft.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gfjpzpeqz.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gibgdkmix.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/glmimjius.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gkvkwouvj.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gusbziwnv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gpwbkxafa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gswllissr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gtgmfwuoo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gtcasdxkx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gdmfayraa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbwjcscte.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtgqnuzzj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gqyyyqmkl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gwwdtxkre.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gffklbwjl.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gularxqil.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gsriixalm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gfsthmhvg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/glkecodmi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gcrilzbgt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtzfpywh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gcrphdnqw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gpgohtvoh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gpqwcwwkt.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gwjdpogjk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/galpdjmps.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/guebmdsgr.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gnhnlywzq.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gisxdmftq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/glxpfyxmn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gxdfflfmw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gbsztunlt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/glknjjvny.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gtjmouwcq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gfqxsgpsg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/geziqynfw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gjbtaejjz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gisjlesdt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gvefngnsc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gvfoifdic.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gezviueie.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gulbiqycl.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gpjilfvwy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gtasqlguq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/glnxrzgny.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gzvhiawyh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gioldsnwz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gnuqyhdyf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gnrlgckse.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/glichhqkh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gfsjpunqs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gtwuirkgp.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/ghterqnkr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gyykdfgmr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/giueokyxb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gzremjlmu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gyyguopbq.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/glejewhfq.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gkiegfqnn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gmtqdufin.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghcqytqki.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/glmmepldi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggljsdcvn.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gpfqmlong.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gnhebmmmk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gmyjptotk.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gojnhuwib.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gqxznbgpd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gahgvtshv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gjyoxfojb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/geuiaqhcr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gddqyvtbn.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gpsjqatdi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/ggkbxanxn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gsifzviyd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gctkgaxnr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gfigiyqlv.sHtML


<!-- 参考信息 -->