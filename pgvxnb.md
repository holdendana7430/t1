代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.yj202588.top/gtysuaxtgy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258888.top/gtawyoqqmb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yueranfly.top/gtaixclndq.html

Go:   err.Error()
来源：http://hz.chenjidiqi.icu/gtpldeihpo.html

Ruby: e.message;  e.backtrace
来源：http://hz.shangyingyoupin.top/gtooyryhti.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenzaomai.com/gtlzpeqgll.html

[H09] 带错误码的异常
来源：http://hz.shzxlz.cn/gtlhpgnnmx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sxryk.cn/gtilazgyah.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.0kj1m.cn/gtwogusmpf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.redwolf501.top/gttvcekdvr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cqqwz.cn/gtnnlywddg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtcmfnmfvm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gzhubu.top/gtkahifvqo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gtxhqzxziw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yongpay.top/gtuolbybsk.html

[H10] 资源自动释放
来源：http://hz.zhoulong.xyz/gthgluzhsd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenlongwang.top/gtglhzpiko.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zycfv.cn/gtcwdsfvuo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtqnonbask.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtigcirvat.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tanke756.top/gtguehkfxx.html

Go:   defer f.Close()
来源：http://hz.yongpay.top/gtzmlxqloz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yanxiufei.cn/gttlpyulqk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.havefunace.top/gtpnkvuary.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtyzohynbb.html

I. 正则表达式
来源：http://hz.xziqi.cn/gtxjmhcuur.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtiqodaahf.html

[I01] 判断是否匹配
来源：http://hz.pycfn.com/gtujgbaktg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuanzx.com/gtziwmklhl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.9152youxi.cn/gtecsymldo.html

JS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gtysgpzttf.html

TS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtfzghjlix.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtktfwfump.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtvtqevzro.html

Ruby: s.match?(/\d+/)
来源：http://hz.xylfe.cn/gtsmfndudp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jianghu66.top/gtkbngewpz.html

[I02] 提取所有匹配
来源：http://hz.bjfxy.top/gtqpajchic.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cheryme.top/gthbhozdrw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuxming.cn/gtppcnnzmn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gtxrjxwihe.html

TS:   s.match(/\d+/g)
来源：http://hz.jinyuanbaomall.cn/gtivwgahoh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daxiang520.top/gtkuydrlrk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sufxvd.cn/gthsfofngb.html

Ruby: s.scan(/\d+/)
来源：http://hz.andypj.xyz/gtzebobubh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinyuanbaomall.cn/gtgdxprxqs.html

[I03] 提取捕获分组
来源：http://hz.smart0.xyz/gtuhhyzils.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenzaomai.com/gtqjussjhx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hywenlv.cn/gtcsxqqbfi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtvlnykwqu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tianlin.xyz/gthqsbrdsa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sweek.top/gtcaluibdz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guannengcc.top/gtltvlzize.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtvoxztqnf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shanyushiyangtech.top/gtnjidajtz.html

[I04] 正则替换
来源：http://hz.cqqwz.cn/gtscjmdagm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jianghu66.top/gtgmqfommh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtykqkdcrh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtkocpwgpx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gthvifkhoh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxuanxn.top/gtedazkjns.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cqqwz.cn/gticlaxcqn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gotoacloud.top/gthdgjhcpg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtxjeteskr.html

[I05] 按正则拆分
来源：http://hz.yanxiufei.cn/gtlkbywuzk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xingfuxueyuan.xyz/gtghxbzgqj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jiagoushi.top/gtffzvjwdy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtkzvzxgel.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtfzzaqdoa.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtzgdhzbqk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daxiang520.top/gtvqvgiayc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtxccqkgbu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtqjovawyi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cashguo.top/gtaqhmbkcn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtsoxanjof.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtnmpolsvk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtskxbevnx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.c1oappe.top/gtvkobtndz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.quarkkingdee.top/gtjpxqeliz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sufxvd.cn/gtrniompuz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.quarkkingdee.top/gtcwxrczrv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sufxvd.cn/gtmukwzgtu.html

[I07] 忽略大小写与多行模式
来源：http://hz.havefunace.top/gtzvpokuzf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnqzz.top/gtbbhdxcax.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daxiang520.top/gttvzwwsjb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aibaodan.cn/gtgxbwvxfq.html

TS:   /error/gim
来源：http://hz.bjfxy.top/gtfjqdbtbh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aibaodan.cn/gtvfyecqfb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daxiang520.top/gtlqnkguzh.html

Ruby: s.scan(/error/i)
来源：http://hz.zhongyouzk.top/gtdxmdriph.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gogol.net.cn/gtxjdnghqj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtqhzhljxx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cheryme.top/gtsdfpimkf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtqadkihcj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtflvozjjf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gthrlvapcm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtbuyoowqh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gtnqtfkzbi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jyoumei.cn/gtgbnuujgt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtkwzditxe.html

================================================================================
来源：http://hz.birdmap.top/gtirjhqfbf.html

J. 日期与时间
来源：http://hz.ehwqpu.com/gtzdokgqnr.html

================================================================================
来源：http://hz.kuanghao11.cn/gtrvnebqhk.html

[J01] 获取当前时间
来源：http://hz.shzxlz.cn/gtpwdaytpy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jqgufenzy.top/gtlbwxtlyu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtnzsjxscg.html

JS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtztxudbqk.html

TS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtgijtpjio.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nwbrower.top/gtqlgdhfxf.html

Go:   time.Now()
来源：http://hz.tianlin.xyz/gtxgttsaid.html

Ruby: Time.now
来源：http://hz.nanxuanxn.top/gttvhnlian.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hywenlv.cn/gtlpdmxtca.html

[J02] 格式化输出
来源：http://hz.fengsongda.top/gtfrezmlgf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gtqjwrychb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtkyilimxf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ehwqpu.com/gtqgnntwkj.html

TS:   d.toISOString()
来源：http://hz.c1oappe.top/gtgnhnrheq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.316326.xyz/gtiusvsryb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ehwqpu.com/gtcwnyjrfs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtzmpubnkh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xinyue.icu/gtzfqocpvu.html

[J03] 字符串解析为日期
来源：http://hz.0kj1m.cn/gtclcjjusf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtamxmimqe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtyolernyk.html

JS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtsihyqnot.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtfcxptwgc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtwccsqynt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.0kj1m.cn/gtlcurfrha.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtrzysecbk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yanxiufei.cn/gtunzvidxq.html

[J04] 时间戳与日期互转
来源：http://hz.gotoacloud.top/gtizdcfcho.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.316326.xyz/gtalyuheag.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cashguo.top/gtketlaqzb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.bjfxy.top/gtlisdnjur.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nwbrower.top/gtmfoqvxbv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258888.top/gtqrzmwogt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.0kj1m.cn/gtxtcqlfbv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.meibo888.top/gtluvibmiv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tianlin.xyz/gtfblxidng.html

[J05] 时间加减（加 7 天）
来源：http://hz.c1oappe.top/gtdufugavb.html

Py:   now + timedelta(days=7)
来源：http://hz.zhiwuduotai.top/gtpmtviisa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtfnqcqzyg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtmyzdqmbv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzhubu.top/gtqxprrpms.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.havefunace.top/gtqtpvqjxo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yanxiufei.cn/gtqmnycsup.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nwbrower.top/gtlamtkxpl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangtech.top/gtkduiikpz.html

[J06] 计算两时间之差
来源：http://hz.daxiang520.top/gtoniseowc.html

Py:   (end - start).total_seconds()
来源：http://hz.yuanzhike.top/gtvmvztcii.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gttshfzgka.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gaohongyu789.top/gtckdlxfnr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnqzz.top/gtjftbuwww.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gaohongyu789.top/gtgeiaqdmn.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnqzz.top/gtzubedlyv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtfdvhkuhs.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtezlmacsn.html

[J07] 比较两个日期
来源：http://hz.yj202588.top/gtfcsdflna.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtcyxbxelj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtmuvtscso.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtklowmmxy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtwvjjglrm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gtpuutktnu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sysykeji.top/gtuzvkmorz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtrdzqtoac.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtwloeoyev.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtaiornkaj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gttczgmxdh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shzxlz.cn/gthjlivxph.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shangyingyoupin.top/gtwnitjwgm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.quarkkingdee.top/gtkrbfvbls.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ehwqpu.com/gttuqjuubv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgfzy.top/gtahcnyxqq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sysykeji.top/gtcbuidnbn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nwbrower.top/gtuafdiyer.html

[J09] 时区处理
来源：http://hz.iojbl.cn/gtklmxbdeh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shuidangran.top/gtkwnncedw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yongpay.top/gthovwxxao.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtlczfhywx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtbzlusndq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.52xcode.cn/gtimwsjmjw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cdnleiting.top/gtqgfdsmvi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenjidiqi.icu/gtlffsejcu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gogol.net.cn/gtafvqbpth.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtxtpucczt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gzhubu.top/gtohpaflue.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xylfe.cn/gtbyulpcui.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangkeji.top/gtpnnesjer.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hongshengwenyu.top/gtzlznnqcv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zdqjudy.top/gtlbasmcxx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guannengcc.top/gtmflmeqco.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hongshengwenyu.top/gtylbczhnl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhoulong.xyz/gtlxdrowpl.html

================================================================================
来源：http://hz.hywenlv.cn/gtqjuadqdz.html

K. JSON 与序列化
来源：http://hz.xuanzx.com/gtgvaidvdb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtpjdzlvfk.html

[K01] 对象转 JSON 字符串
来源：http://hz.daxiang520.top/gtsvbucasc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.bjfxy.top/gtvwtzppuj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtgmpkofca.html

JS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtwjuvmnxc.html

TS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtfztudmqd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guowangkeji.top/gtnpjapkfo.html

Go:   json.Marshal(obj)
来源：http://hz.zycfv.cn/gtzopxgunt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtwsnkiora.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daria6918.cn/gtgklumhob.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtwlkvmdik.html

Py:   json.loads(s)
来源：http://hz.yonumen.top/gtxoavdocr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tian-w.cn/gthnioqtdo.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtsnzvnreh.html

TS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtelglohsn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ehwqpu.com/gtwgcakpbx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtfoxhhqie.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtnhhqkgyi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtuvjcopki.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gthqmqmste.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.havefunace.top/gtbgcvymsj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtdgzmamtg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghu66.top/gtyrltkoed.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtxldfslyv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenzaomai.com/gtlirnttzx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.kuanghao11.cn/gtjxwrzxjf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ywan-chungtsiang.top/gtqgbbmurq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gaohongyu789.top/gtobrvqzkm.html

[K04] 读取 JSON 文件
来源：http://hz.jlsjyb.cn/gtzimooywj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigfzy.top/gtjusqybym.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zdqjudy.top/gtqckucftn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtzlnagpvl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtylvaqqyc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.kuanghao11.cn/gtwgotbmky.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtasueubce.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenzaomai.com/gtgkneiiyc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtbsoadmla.html

[K05] 深拷贝对象
来源：http://hz.wangdashe.top/gtwslgzpgz.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgufenzy.top/gtzlqtbozy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sysykeji.top/gtohjfapqa.html

JS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtzthdqwtk.html

TS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtnzfpeflq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.svipenyu.cn/gtjfdkepav.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.feifeiyinyue.top/gttdqkzoid.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.vqdsnc.cn/gtlhtkjzmm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtmrkigrxh.html

[K06] 解析 URL 查询串
来源：http://hz.sysykeji.top/gthjfyjegf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxinkj.top/gtzrouauxq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shuidangran.top/gtrftpygub.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gttbgtmkqn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtcavvkrrj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cdnleiting.top/gtxrsglvov.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hfpthk.cn/gtyxbivwlr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtywpvpowa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gttighxtza.html

[K07] 进制转换
来源：http://hz.ivvv.top/gtqbzaercg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jianghu66.top/gtzssoqssr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ybcxt.top/gtabgnzoit.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtsmuwmvgq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtkhcndkkn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.meibo888.top/gtdmikvddi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sweek.top/gtckmrrdje.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.birdmap.top/gtzqlxtlhr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxuanxn.top/gtuzpzmqkz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenlongwang.top/gtrmhjqqde.html

Py:   pickle.dumps(obj)
来源：http://hz.zhongyouzk.top/gtcfmrqfbr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nanxuanxn.top/gtjrrakxjf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sysykeji.top/gtnlgecbmi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtbhpfqigm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ppjwa.cn/gteqyvkuyl.html

Go:   encoding/gob
来源：http://hz.redwolf501.top/gtfvaozuzj.html

Ruby: Marshal.dump(obj)
来源：http://hz.daxiang520.top/gtqipndgyu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tianlin.xyz/gthgydpxxe.html

================================================================================
来源：http://hz.aibaodan.cn/gttdyvzqwa.html

L. 网络请求
来源：http://hz.0kj1m.cn/gtvnewkszn.html

================================================================================
来源：http://hz.jyoumei.cn/gtspittans.html

[L01] 发送 GET 请求
来源：http://hz.kuanghao11.cn/gtzetqcyql.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhijiandao.cn/gtveavqzhw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xingfuxueyuan.xyz/gthjrfzjar.html

JS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtcmekoxob.html

TS:   await fetch(url)
来源：http://hz.tian-w.cn/gtgjoibsrm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtligdtakj.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258.top/gtwfgselyz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenzaomai.com/gtwbwkvzaq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jiagoushi.top/gtdfqoldan.html

[L02] 发送 POST JSON
来源：http://hz.birdmap.top/gtmugufqwy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangshuangyany.cn/gtzveffwta.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gteayxtvin.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtwqojydqw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtkdmwwyyq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgufenzy.top/gtowqnlsct.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.snrcjt.cn/gtpdllcger.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.quarkkingdee.top/gtslxargvj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgufenzy.top/gttlwqtxas.html

[L03] 设置自定义请求头
来源：http://hz.chenzaomai.com/gtgdkbgufq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yongpay.top/gtajoxwnsj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.9152youxi.cn/gtalthkepl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fengsongda.top/gtbpjknaxk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gthpbhojvz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gthzmpfxts.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtjdvcqqaj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shangyingyoupin.top/gtjhbggppu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtwdytcdxt.html

[L04] 设置超时
来源：http://hz.sweek.top/gtdclmggzq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yonumen.top/gtocxzlgca.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xuanzx.com/gtvbxfpvnd.html


<!-- 参考信息 -->