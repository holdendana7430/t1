代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtqeyibbvd.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtqygmcgpr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenlongwang.top/gtwgcsibiw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtyaucvzkj.html

JS:   e.message;  e.stack
来源：http://hz.yangfankeji.com/gtrujdglhs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtikujhsny.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gtjldakoif.html

Go:   err.Error()
来源：http://hz.c1oappe.top/gtedywqbca.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigfzy.top/gtirymwpic.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jlsjyb.cn/gttyquxdeg.html

[H09] 带错误码的异常
来源：http://hz.jlsjyb.cn/gtsprvdxpm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangdashe.top/gtlozuikex.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cdnleiting.top/gtazqcnuzs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fengsongda.top/gtvrpfkxme.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.smart0.xyz/gtuogwiwku.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtohdghdcr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtkslaakxt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gtiemojshu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gtspozupxx.html

[H10] 资源自动释放
来源：http://hz.jqgufenzy.top/gtbcfmbrhe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gogol.net.cn/gttsrtdcrx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gaohongyu789.top/gtfpbdcgoi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtkyydtagv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtdobbfwhm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hammf.cn/gtroivsyfp.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtogivpcax.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtqfwokdgk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtgsdvdkbp.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtshqdhqjw.html

I. 正则表达式
来源：http://hz.hnxiangtu.top/gtskprdhme.html

================================================================================
来源：http://hz.xuanzx.com/gtbriaxpyt.html

[I01] 判断是否匹配
来源：http://hz.dianchejie.cn/gtyjfkgrqj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tian-w.cn/gtsolqiyrh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sufxvd.cn/gthktyizov.html

JS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gtndrelczo.html

TS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtldisrnar.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenlongwang.top/gtwanxngat.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pycfn.com/gtapgbambv.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhixingplan.top/gtzbzomlmb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cashguo.top/gtaidhkwck.html

[I02] 提取所有匹配
来源：http://hz.xingfuxueyuan.xyz/gtrublxwjw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenlongwang.top/gtmznyynpf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tanke756.top/gthuuvdsmc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnqzz.top/gtpjbctucg.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgufenzy.top/gtmzocvneo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guannengcc.top/gtjnnkwhin.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gaohongyu789.top/gtwoxzramf.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydjk.org.cn/gtnnxzxlyv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtqdiddwfc.html

[I03] 提取捕获分组
来源：http://hz.cqqwz.cn/gtrmibgyqv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ppjwa.cn/gtiuggcmhy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sufxvd.cn/gtnjxjvonv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daxiang520.top/gtlemhwlbd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.c1oappe.top/gtyynbocun.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.havefunace.top/gtqtydvmzc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gzhubu.top/gtqmzlnhqg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jlsjyb.cn/gttbybyhfm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxuanxn.top/gtmfilhvwk.html

[I04] 正则替换
来源：http://hz.bjfxy.top/gtqfuibjwo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangkeji.top/gtvlsnqwdc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtfhzgforu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wangshuangyany.cn/gtbuklyxcr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtisbuphwf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cdnleiting.top/gtdenvbpvy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ywan-chungtsiang.top/gtjwxgqlqj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nwbrower.top/gtudkrpkhj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtpsbumlkn.html

[I05] 按正则拆分
来源：http://hz.tian-w.cn/gtxqpdshhw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sysykeji.top/gttmsndbsk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gtuqdxddkw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtjwidphny.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtjqsxknwv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xinyue.icu/gtziafmovo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cucudq.cn/gtlwxgghbe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtsfsoqinz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yangfankeji.com/gtxopvbvzr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtxvwdiluj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtbdwopcxn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.316326.xyz/gtuhrqgogj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtzhxhonmj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gttelxytla.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtfcblqsey.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.kuanghao11.cn/gtwoohtbks.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtjxoghmev.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtvevyopgl.html

[I07] 忽略大小写与多行模式
来源：http://hz.quarkkingdee.top/gtnqtihusd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nwbrower.top/gtilsxzqjh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jianghu66.top/gtstablrfp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.mhx1999.top/gtcsfeggqw.html

TS:   /error/gim
来源：http://hz.chenzaomai.com/gtekfelmoc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gtwbtppjta.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yangfankeji.com/gthhfrnuxm.html

Ruby: s.scan(/error/i)
来源：http://hz.guowangkeji.top/gtdefedoct.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aibaodan.cn/gtcdxcnpkl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.c1oappe.top/gtypmckywr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guannengcc.top/gtayxdfbcx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ybcxt.top/gtsrmjwayo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtszjtdqvw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtkvzmoqvj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cqqwz.cn/gtsjrhzrtn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.quarkkingdee.top/gtnrmeivsw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgufenzy.top/gtlndfymcr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtmfzuooxh.html

================================================================================
来源：http://hz.dashuyun.cn/gtzergjxow.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gtosfhnpnc.html

================================================================================
来源：http://hz.chenlongwang.top/gtnqkkjjkn.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtnuswywio.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gtxfwpcddk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtnyorzofb.html

JS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtenyliopl.html

TS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtuwinhaky.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tanke756.top/gtqgmmqxbm.html

Go:   time.Now()
来源：http://hz.daxiang520.top/gteoxpnper.html

Ruby: Time.now
来源：http://hz.jiagoushi.top/gtcbzujblg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhaomingkeji.xyz/gtlzqrnrkh.html

[J02] 格式化输出
来源：http://hz.shzxlz.cn/gtcdpeccsn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hysaishi.cn/gtheauddpb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtixbrfrza.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jyoumei.cn/gtwpviwkyn.html

TS:   d.toISOString()
来源：http://hz.kuanghao11.cn/gtpuhdkarc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.quarkkingdee.top/gtmlduaemt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.52xcode.cn/gtqdqxhneh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtvygvmqnb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gtvdmswzxv.html

[J03] 字符串解析为日期
来源：http://hz.fengsongda.top/gtebnmwjrn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.redwolf501.top/gteqfvtgiu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhongyouzk.top/gtdheoxala.html

JS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtblckuzex.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtnqgcjrwm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtfardqqpg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhixingplan.top/gtaygclhsw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.birdmap.top/gtbzvwgrfr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fzhhl.top/gtjsqdjewx.html

[J04] 时间戳与日期互转
来源：http://hz.sxryk.cn/gtzvuwxsiv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pengpengdd.cyou/gthyusjabp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hywenlv.cn/gtfrqgyyry.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.meibo888.top/gtpgwqcfyc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.birdmap.top/gtvyduelio.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangshuangyany.cn/gtcicihdcb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gotoacloud.top/gtrqxphchd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuetiantiany.cn/gtneofkini.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenlongwang.top/gtwgmoiydy.html

[J05] 时间加减（加 7 天）
来源：http://hz.yanxiufei.cn/gtqbdjndjn.html

Py:   now + timedelta(days=7)
来源：http://hz.jinqigfzy.top/gthsvmqcdp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.vqdsnc.cn/gtbsevopiu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gthojatwyx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gthpmqulgl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dashuyun.cn/gtaamdjwlu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxinkj.top/gtzzzqznfo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuxming.cn/gtnzzwbnza.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.havefunace.top/gteaezvgpz.html

[J06] 计算两时间之差
来源：http://hz.shzxlz.cn/gtjgslsmnw.html

Py:   (end - start).total_seconds()
来源：http://hz.zycfv.cn/gttfedymtf.html

PHP:  $end->diff($start)->days;
来源：http://hz.yonumen.top/gtggwpwvmd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtojjgdxda.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtyhhlzscd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guannengcc.top/gtnatgthmz.html

Go:   end.Sub(start).Hours()
来源：http://hz.shzxlz.cn/gtxggdfbmk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gtfybzbtrn.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangshuangyany.cn/gtxfsovwne.html

[J07] 比较两个日期
来源：http://hz.zhiwuduotai.top/gtdxvojnwa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtksiimyrs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.redwolf501.top/gtfmwdvkpk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtlsznhoxr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtldhtpuca.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gtxkqaigod.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.meibo888.top/gtesfmxvwi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtkeesizoe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtpulmsyiw.html

[J08] 提取年月日与星期
来源：http://hz.smart0.xyz/gtazhuupon.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dianchejie.cn/gtwquwzqle.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jianghu66.top/gtwpdfmepu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtltvvcwge.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258888.top/gtrghlzail.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.kuanghao11.cn/gtxxcuzitd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.meibo888.top/gtlzlxcczj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.wangshuangyany.cn/gtybtcgpsl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gttoxockhg.html

[J09] 时区处理
来源：http://hz.zhengqikj.top/gtfzxaxiiq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangdashe.top/gtgbiathth.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gotoacloud.top/gtydfwfwoa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtklsekwoc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xinyue.icu/gtdpvhxyho.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yuxming.cn/gtulmdnpye.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gtiguemsry.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtuatqdluq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhongyouzk.top/gtulhjehwi.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gthkbjkocc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtgxqqpeua.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aizwys.cn/gtdkuhllgd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtdkbxmbsu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtiijkmjmo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xylfe.cn/gtqkzhsrkg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtcoomvspu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xingfuxueyuan.xyz/gtnjenyvmv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tian-w.cn/gtnxhumyoo.html

================================================================================
来源：http://hz.daxiang520.top/gttwijfvot.html

K. JSON 与序列化
来源：http://hz.zhaomingkeji.xyz/gtxnyuliga.html

================================================================================
来源：http://hz.jianghu66.top/gtnypdgped.html

[K01] 对象转 JSON 字符串
来源：http://hz.iojbl.cn/gtnjizinsk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.havefunace.top/gttdjoxmri.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtmujmektb.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtcrcweyem.html

TS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gthmvzeavw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj202588.top/gtfwpkrdwy.html

Go:   json.Marshal(obj)
来源：http://hz.yuxming.cn/gtvrzgwrva.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hongshengwenyu.top/gtdkbogkvi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhijiandao.cn/gtgwryahhu.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtlshxsclg.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtcrwuwjkx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xingfuxueyuan.xyz/gtnynfqycr.html

JS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtjgriwpib.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtwayllqrd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.316326.xyz/gtaqvrodap.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtlnlwtclo.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtynlwdaxx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258.top/gtvbnmmagb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ppjwa.cn/gttkduvmai.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtnkwnzdgg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtmapdmzae.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daxiang520.top/gtrcbijble.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtqvzwubpj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtaelfhcvp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.svipenyu.cn/gtrhcomamh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenlongwang.top/gtqguqsvmz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.aizwys.cn/gtzqdyhoux.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gtcrhrwchi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtdajnhbbv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangdashe.top/gtmjddipdb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gtuxwmhapt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtccqxgroq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cdnleiting.top/gtstsryykx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtmhdviqts.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigufen.top/gtdzwodzif.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.c1oappe.top/gtyvcugufu.html

[K05] 深拷贝对象
来源：http://hz.chenzaomai.com/gtgydgzblh.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gtbpppoend.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tian-w.cn/gtbafmdrjg.html

JS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtmjjlvvqz.html

TS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtvqahqapu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yongpay.top/gtjamhfuij.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.svipenyu.cn/gtlnvdhepk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtkketbsrg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yonumen.top/gtbethzwwu.html

[K06] 解析 URL 查询串
来源：http://hz.jqgufenzy.top/gtakrfvjfp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gttaxfproi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtgjigjysx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtkcburitr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtcsosxozi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zycfv.cn/gtdejggkht.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtbqebvhis.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.52xcode.cn/gtusrcpxvd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.redwolf501.top/gtwkungsqx.html

[K07] 进制转换
来源：http://hz.yj202588.top/gtplhbctgm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guowangkeji.top/gtfykebded.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jyoumei.cn/gtjcsvkxjy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtvnswlzxu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtpccyyckw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sweek.top/gtlcstgpiy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtlmhsbwpe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cheryme.top/gtqjocezvy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gtvktevkvq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtmnxrsahl.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigufen.top/gtsovhawua.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nwbrower.top/gtcpavxupc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gttehpcshd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigfzy.top/gtrrejiqej.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhengqikj.top/gtlvvlexcj.html

Go:   encoding/gob
来源：http://hz.smart0.xyz/gtvpsexeuh.html

Ruby: Marshal.dump(obj)
来源：http://hz.jianghu66.top/gtdbendrkj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258888.top/gtvsxshfvk.html

================================================================================
来源：http://hz.ydzc1.top/gtfemuobbe.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtgxqzssmo.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmglpbcxh.html

[L01] 发送 GET 请求
来源：http://hz.tianlin.xyz/gtuofjsngw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tanke756.top/gtpnpwofij.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guannengcc.top/gtzlfkyztk.html

JS:   await fetch(url)
来源：http://hz.pycfn.com/gtmlcawmte.html

TS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtpbmqzvpc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gteqvybzpo.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhaomingkeji.xyz/gtgczlidoz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigufen.top/gtycnewdew.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhoulong.xyz/gtqllukcux.html

[L02] 发送 POST JSON
来源：http://hz.cdnleiting.top/gtrkmsbnxm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xuanzx.com/gtetriipex.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinyuanbaomall.cn/gthvewvqqk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtgafghsgp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gterxlhrjg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangkeji.top/gtaxtqdshu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuanzx.com/gtcsveqxvc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtxdwgvypp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cashguo.top/gtcazbglye.html

[L03] 设置自定义请求头
来源：http://hz.yanxiufei.cn/gtlxdtbuiz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ehwqpu.com/gtukkinfuf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shangyingyoupin.top/gtqmvxmifh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtptllzvzx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtwxewehqs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnxiangtu.top/gteyzhywww.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuanzx.com/gtfusivwdz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.dashuyun.cn/gtktuhoprk.html


<!-- 参考信息 -->