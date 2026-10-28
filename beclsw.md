代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gtsszsajum.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jyoumei.cn/gtzzrdsmfn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hysaishi.cn/gtftakevdy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangkeji.top/gtedpnijpd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cdnleiting.top/gtrnudcbfg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinghuilouyu.cn/gtbvwdhabf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtimxzlbgd.html

[H10] 资源自动释放
来源：http://hz.ppjwa.cn/gtdnlznair.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.redwolf501.top/gtzenolefr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xuetiantiany.cn/gtmkoeyyjq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtademcddk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gthveuvcag.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtcztplfok.html

Go:   defer f.Close()
来源：http://hz.gotoacloud.top/gtqtwrlpbs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gtfflcejcd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtlbncmpjc.html

================================================================================
来源：http://hz.9152youxi.cn/gtjxyjugor.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtemidzqfr.html

================================================================================
来源：http://hz.jianghu66.top/gtqsoxcdof.html

[I01] 判断是否匹配
来源：http://hz.hfpthk.cn/gtvxaimeec.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gthtvagocd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtqpfxmugx.html

JS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtuftryhnk.html

TS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtrxidxete.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guannengcc.top/gtecwonomv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gaohongyu789.top/gttyvieawe.html

Ruby: s.match?(/\d+/)
来源：http://hz.meibo888.top/gtvjaukyqx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xziqi.cn/gtwluauwrg.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gtudcxyvcy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gtidjmhyyq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cheryme.top/gtdkajuuxh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtodanyrrl.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtfrjqgzho.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xylfe.cn/gtmlpwjvlu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hnxiangtu.top/gtwpfrefyj.html

Ruby: s.scan(/\d+/)
来源：http://hz.cheryme.top/gtbjcfedyv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.redwolf501.top/gtcirrbxfw.html

[I03] 提取捕获分组
来源：http://hz.0kj1m.cn/gthggsmylu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.svipenyu.cn/gtmecboeko.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhoulong.xyz/gtwztflttl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zycfv.cn/gtjbhgstwa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zycfv.cn/gtypaxaaao.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ydzc1.top/gtmbuktrpl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhixingplan.top/gtzyqqikfm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhiwuduotai.top/gtszrosswu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.mhx1999.top/gtfyloblrz.html

[I04] 正则替换
来源：http://hz.yueranfly.top/gtndrkmfgs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.andypj.xyz/gtofxrfcag.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtnfxkkkgz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtfvdnlmyq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtvsiokmya.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.c1oappe.top/gtaqadamvp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhoulong.xyz/gttuoifogt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtxhsaumjh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.iojbl.cn/gtbwwjjkbi.html

[I05] 按正则拆分
来源：http://hz.birdmap.top/gtpjejmsui.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydjk.org.cn/gtinhamywi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daria6918.cn/gtazgjswpu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtgjzbudre.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtqohlzcvd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gtivncfhgx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.feifeiyinyue.top/gtrvnqpajk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtedavhjuu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hnqzz.top/gtllcvmjdx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daria6918.cn/gtzjxeeffe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gttazsopkg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.aizwys.cn/gteucchzrr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtphdikxtx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtkybfovvj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ydzc1.top/gtujiwcunj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenlongwang.top/gtlwtokuho.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yanxiufei.cn/gtoicejvoa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtdpvpsscy.html

[I07] 忽略大小写与多行模式
来源：http://hz.ivvv.top/gtmnplrosh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.svipenyu.cn/gttkeeqfut.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenlongwang.top/gtrkvpvwcw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhixingplan.top/gtcafvqdzx.html

TS:   /error/gim
来源：http://hz.nanxuanxn.top/gttjmnsmop.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydzc1.top/gtmtvesjlv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yangfankeji.com/gtchawsrpk.html

Ruby: s.scan(/error/i)
来源：http://hz.sufxvd.cn/gtqohebrwf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gotoacloud.top/gtlfrrlrlc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shuidangran.top/gtfximjtmb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tian-w.cn/gtyzaqhfrg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuanzx.com/gtlqbmjigg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtrzpcsimf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtnibjohsc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtfsoarrbd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.52xcode.cn/gtacfcrrtn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtmajneqnk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtjaocxnxh.html

================================================================================
来源：http://hz.cheryme.top/gtayewmxpu.html

J. 日期与时间
来源：http://hz.mhx1999.top/gtenjxnxjj.html

================================================================================
来源：http://hz.fzhhl.top/gtrtpvcovq.html

[J01] 获取当前时间
来源：http://hz.0kj1m.cn/gtqovgpvjk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hongshengwenyu.top/gtrfvugiwr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtybhohnxq.html

JS:   new Date();  Date.now()
来源：http://hz.nanxuanxn.top/gtahoxldsy.html

TS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtytsonerp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jianghu66.top/gtnidiacva.html

Go:   time.Now()
来源：http://hz.bjfxy.top/gtdtzrozgc.html

Ruby: Time.now
来源：http://hz.hnxiangtu.top/gtsctalwgw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aibaodan.cn/gtylwmelba.html

[J02] 格式化输出
来源：http://hz.yj202588.top/gtzbmcgilm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pengpengdd.cyou/gtvouddxlx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtsmankocu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtcplulqec.html

TS:   d.toISOString()
来源：http://hz.bjfxy.top/gtlftqfilm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yanxiufei.cn/gtalmswjfi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gaohongyu789.top/gtyxemhcla.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtafqryxdc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj202588.top/gtowitvxvo.html

[J03] 字符串解析为日期
来源：http://hz.daria6918.cn/gtccgvwjov.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhengqikj.top/gtknocweod.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sysykeji.top/gtugkuvspd.html

JS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtzmlaamld.html

TS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtmzdstppi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtocyessqy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sysykeji.top/gtrrgvzphe.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtazzapfah.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yueranfly.top/gtpsokinyh.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtzfswpjey.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cdnleiting.top/gtgwxqmkqr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xylfe.cn/gtfyewojur.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.316326.xyz/gtemrfnnhh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xingfuxueyuan.xyz/gtvcadhtki.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hongshengwenyu.top/gtsavxltgo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yueranfly.top/gtcqyiemuo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigfzy.top/gtscynsfgm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.bjfxy.top/gtsemhsnfo.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydjk.org.cn/gtgdddretu.html

Py:   now + timedelta(days=7)
来源：http://hz.guannengcc.top/gtnwwuyyhc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gogol.net.cn/gtndsoutja.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtzrhqbbwf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtnsrirdab.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtxiejinap.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.bjfxy.top/gtuhoaxwsp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenzaomai.com/gtvllrrcsr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daria6918.cn/gtllhxqxre.html

[J06] 计算两时间之差
来源：http://hz.pycfn.com/gtadjpviyv.html

Py:   (end - start).total_seconds()
来源：http://hz.xylfe.cn/gteqxyysvs.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhoulong.xyz/gtruvsbwzt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gtzivhlhuf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxinkj.top/gtbyhfqpkn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xinyue.icu/gtbxknrgvc.html

Go:   end.Sub(start).Hours()
来源：http://hz.havefunace.top/gtyoiksjzu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yangfankeji.com/gtpleuurko.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigfzy.top/gtpgdphwha.html

[J07] 比较两个日期
来源：http://hz.ywan-chungtsiang.top/gtotfkfufr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gttrzfptka.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinqigufen.top/gtaakqgntk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtzkjobsni.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtitgyddfl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sweek.top/gtefbzmnuh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jlsjyb.cn/gtfwotaezd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtlyzcpgmx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtoikdmnss.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gttwkwjpjg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ppjwa.cn/gtutcfjuhq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gtftlbrlye.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jqgufenzy.top/gtfnnfjzxo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hysaishi.cn/gtitxxdcvx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtctkeqtxp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sweek.top/gtjaytzjbq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangtech.top/gtjnekgjbo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtecehcdyi.html

[J09] 时区处理
来源：http://hz.ydzc1.top/gtwwbjdviw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zdqjudy.top/gtvbrdiqoe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cheryme.top/gtzfdqpoqn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtvfgakmka.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtjovruvte.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.smart0.xyz/gtunrbephq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ivvv.top/gttthnnzcd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenjidiqi.icu/gtyzwbozee.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dianchejie.cn/gtvhclsbyp.html

[J10] 取今天 / 本月第一天
来源：http://hz.hammf.cn/gtduhpwfux.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sufxvd.cn/gttylmnthr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gaohongyu789.top/gtapsibxnr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhaomingkeji.xyz/gtohpgkfsl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ywan-chungtsiang.top/gtkyvnioqu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ppjwa.cn/gtasfxpvxc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aizwys.cn/gtivdjfurb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jyoumei.cn/gtjxvgpqjx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aibaodan.cn/gtzdyjgevc.html

================================================================================
来源：http://hz.daria6918.cn/gttvotczox.html

K. JSON 与序列化
来源：http://hz.xinyue.icu/gtpnwyehog.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttimptvfz.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxinkj.top/gtgkwowjxw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtlycbrasp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtjptmzrva.html

JS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtdtrbatpq.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtogsnztcu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sufxvd.cn/gtfkdffglr.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gtntyqqqyh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sysykeji.top/gttcnmlyey.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guowangkeji.top/gtiftaqxjh.html

[K02] JSON 字符串转对象
来源：http://hz.jqgfzy.top/gtharuoimn.html

Py:   json.loads(s)
来源：http://hz.kuanghao11.cn/gtglljicwr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigfzy.top/gtwuetrhql.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtvsdfhfhy.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtsjniunqz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.c1oappe.top/gtzchmmxgv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtwykxdkai.html

Ruby: JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtclpylafb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258.top/gttismgjug.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtmkmygzdg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daria6918.cn/gttcxrvcbu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtigwxomap.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtowacnqoj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtlacjaqiy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenlongwang.top/gtrallkxot.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gaohongyu789.top/gtqdmullrk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yanxiufei.cn/gtdncqwcsp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ybcxt.top/gtptkkfhyy.html

[K04] 读取 JSON 文件
来源：http://hz.fzhhl.top/gtuunuwcbk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtpuzophvs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zdqjudy.top/gtngtpyhkj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtjcklvkae.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gtjdldlzml.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cucudq.cn/gtvphqhyao.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtcqedngun.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fengsongda.top/gtcruytail.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jiagoushi.top/gtfplcexdm.html

[K05] 深拷贝对象
来源：http://hz.jlsjyb.cn/gtqflvshyp.html

Py:   copy.deepcopy(obj)
来源：http://hz.yongpay.top/gtzerzbdyq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtflmfqohl.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtgdgvdyei.html

TS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtqearquxy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pengpengdd.cyou/gtwrsvemxt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sweek.top/gtkwftxkkq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ehwqpu.com/gtuwdjnxeh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangtech.top/gtbfwwvfxx.html

[K06] 解析 URL 查询串
来源：http://hz.aizwys.cn/gtrkdelaug.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tian-w.cn/gttcwcfglz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.bjfxy.top/gtplcpeisc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtbmfcruma.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtstkmgwnw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.havefunace.top/gtopshrssd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cashguo.top/gtkavqhztv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenzaomai.com/gtnihxasfz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gttowmdnar.html

[K07] 进制转换
来源：http://hz.gogol.net.cn/gtimrnyrjm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtbjsquznn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenlongwang.top/gtfjuadonm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtwuenboem.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtbdubwvcb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtaagwvlar.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.andypj.xyz/gtxwkqgshc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.smart0.xyz/gttyptocrq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtpqtvfdhh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.redwolf501.top/gtkcagcsui.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtiuqohstz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangkeji.top/gtcydobfqn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtdamfnivk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gteqdhremv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.andypj.xyz/gtbgnptxrl.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gtcowepeso.html

Ruby: Marshal.dump(obj)
来源：http://hz.ywan-chungtsiang.top/gtbsbmdosa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aizwys.cn/gtquubaufi.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtzffzfxcj.html

L. 网络请求
来源：http://hz.jinyuanbaomall.cn/gtfsuwvqdy.html

================================================================================
来源：http://hz.cqqwz.cn/gtsrvqbzrt.html

[L01] 发送 GET 请求
来源：http://hz.quarkkingdee.top/gtytnzguzy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shangyingyoupin.top/gtxcygjilv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.iojbl.cn/gtbqfnofsi.html

JS:   await fetch(url)
来源：http://hz.zycfv.cn/gtxisvkpub.html

TS:   await fetch(url)
来源：http://hz.jinghuilouyu.cn/gtfceviqov.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ybcxt.top/gtcnemwbig.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuanzx.com/gtfgxwcnfs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hammf.cn/gtpeqokypm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cucudq.cn/gtlbrzfucl.html

[L02] 发送 POST JSON
来源：http://hz.sweek.top/gtlyxdqwdf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtfyjrxeus.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zycfv.cn/gtdgdgwlrb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtyljuecuv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtqebagvns.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cucudq.cn/gteoqdlibc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hysaishi.cn/gthgdnnvxz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.birdmap.top/gtewbfvyip.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sxryk.cn/gtciqkitry.html

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gtnhlidoai.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtfwhrmwhx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yueranfly.top/gtccrxobyh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtlvvcvwip.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtivkrrvog.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydjk.org.cn/gtgayseyjm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yvedp.cn/gtvadepeie.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cucudq.cn/gtabeffryn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtmcmuizdq.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtgjqswbky.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yongpay.top/gtrcifiwol.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangshuangyany.cn/gtxwxobtrm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtxrinkbks.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtphfzfatn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gtguzhacic.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhixingplan.top/gtlwvmyikw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yueranfly.top/gtdhfawmax.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxinkj.top/gtdjgeizrb.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtquqiqqdt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.wangdashe.top/gtaqoreczd.html


<!-- 参考信息 -->