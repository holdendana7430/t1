代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.nwbrower.top/gtilwidwii.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tanke756.top/gtlvxqxwsw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtbuuuexkf.html

Go:   err.Error()
来源：http://hz.tianlin.xyz/gtqqhtxwss.html

Ruby: e.message;  e.backtrace
来源：http://hz.yvedp.cn/gtkhpzespd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cqqwz.cn/gtxzjqujag.html

[H09] 带错误码的异常
来源：http://hz.shuidangran.top/gttgvvilxu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhongyouzk.top/gtwgxnoxku.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydjk.org.cn/gtdtumfgss.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sysykeji.top/gtczzdlonh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhoulong.xyz/gtyzkqztpv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtcxqfauty.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fengsongda.top/gtmdwbianh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.meibo888.top/gtdadgyfsv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hongshengwenyu.top/gtddrqbxvk.html

[H10] 资源自动释放
来源：http://hz.andypj.xyz/gtdfhaidiw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jyoumei.cn/gtvkeplwiz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gtcmkqdqrs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtbfrorvlb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yanxiufei.cn/gtvftkqqtf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daxiang520.top/gtxyaspbpm.html

Go:   defer f.Close()
来源：http://hz.aizwys.cn/gtduymwzmn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aibaodan.cn/gtbqjduhyo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gaohongyu789.top/gtciajuwtp.html

================================================================================
来源：http://hz.yuanzhike.top/gtwskplera.html

I. 正则表达式
来源：http://hz.c1oappe.top/gtbmhjlvbz.html

================================================================================
来源：http://hz.yj20258888.top/gtwhavqjep.html

[I01] 判断是否匹配
来源：http://hz.tianlin.xyz/gtdqsfsbjy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtarbcgebs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtuybjrzyh.html

JS:   /\d+/.test(s)
来源：http://hz.svipenyu.cn/gtkghzexqg.html

TS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gtbizdgbqt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhongyouzk.top/gtshnjgyvn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daria6918.cn/gtkieduinc.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gtojumeorc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuetiantiany.cn/gtmcynauyx.html

[I02] 提取所有匹配
来源：http://hz.zhiwuduotai.top/gtbtetohmp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtnamthbxe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cucudq.cn/gtehatjiyy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxinkj.top/gtffmnhrch.html

TS:   s.match(/\d+/g)
来源：http://hz.haohaochexian.top/gtfrjqzsbh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aibaodan.cn/gtteylfeuv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gttqveqwms.html

Ruby: s.scan(/\d+/)
来源：http://hz.aizwys.cn/gthfhpfxjt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shzxlz.cn/gtgehtdzos.html

[I03] 提取捕获分组
来源：http://hz.0kj1m.cn/gtmvfaqtxg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jiagoushi.top/gtggfrstcl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tanke756.top/gtyvxwrpsb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jlsjyb.cn/gthhhwimlo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shzxlz.cn/gtgkgqsmtu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guowangkeji.top/gtymdoqvmw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtjpehthpb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guowangkeji.top/gtyahusqih.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtlrkvuxjj.html

[I04] 正则替换
来源：http://hz.chenlongwang.top/gtcphdbcba.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.0kj1m.cn/gtghknjxwm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.316326.xyz/gtlancrywd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtavzxjqdz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtameduhkf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yongpay.top/gtqqjhkrli.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhaomingkeji.xyz/gtgkmmhkiw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhijiandao.cn/gtoycbsmfm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuanzhike.top/gttejdvehp.html

[I05] 按正则拆分
来源：http://hz.fzhhl.top/gtikaaptas.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shzxlz.cn/gtkvndhpic.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.iojbl.cn/gtmzmjwkfq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtlxuktvwk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtxaqsqeup.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sysykeji.top/gtjeknjzwh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daxiang520.top/gttkmldiae.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtygudpnqc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.smart0.xyz/gtopnrheuc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sufxvd.cn/gtaabhsusb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtxkaqkenz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtfotokper.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydzc1.top/gtenznxhea.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gtxmzcguso.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gtkcnvvnkc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daxiang520.top/gtucrwqkpk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnxiangtu.top/gtqnnlvhtj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gtudivlkms.html

[I07] 忽略大小写与多行模式
来源：http://hz.kuanghao11.cn/gtwbzaxguv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenzaomai.com/gtnjfpybhm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yangfankeji.com/gteoptjgaw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jlsjyb.cn/gtvhqsgvnu.html

TS:   /error/gim
来源：http://hz.svipenyu.cn/gtajbrpome.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shuidangran.top/gtjhqdsupp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daria6918.cn/gtbogepudn.html

Ruby: s.scan(/error/i)
来源：http://hz.zhijiandao.cn/gttmunwggc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xingfuxueyuan.xyz/gtmeqgjbfb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigufen.top/gtzqujhzkx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yonumen.top/gtfrbkbtxk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.meibo888.top/gtxplrownw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtzwnmdrse.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtpvikopbh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.redwolf501.top/gtxpwjxayr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aizwys.cn/gtrnmsaeun.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigfzy.top/gtvducxzcq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.redwolf501.top/gtxaptuzfg.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthmbtvvqp.html

J. 日期与时间
来源：http://hz.sysykeji.top/gtumjxddie.html

================================================================================
来源：http://hz.yj202588.top/gtzalfjpnq.html

[J01] 获取当前时间
来源：http://hz.guowangkeji.top/gtrumzllaw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ppjwa.cn/gtndffndze.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gtqxfbfznj.html

JS:   new Date();  Date.now()
来源：http://hz.daria6918.cn/gtuqrnlrtq.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtwsjsllrv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xinyue.icu/gtbvkznrnq.html

Go:   time.Now()
来源：http://hz.havefunace.top/gtgzxyzldq.html

Ruby: Time.now
来源：http://hz.birdmap.top/gtutcskpej.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.iojbl.cn/gtrbakujce.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gtxqsdvzes.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtgnqfburr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtkbpooxem.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gtnxelpecj.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gtnxuqpqeo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aizwys.cn/gtjwayeeqb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtebqsgthf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtzyceswrt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ehwqpu.com/gtrkzslxsg.html

[J03] 字符串解析为日期
来源：http://hz.hammf.cn/gtogwfwytr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gzhubu.top/gtcbzabqdb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.mhx1999.top/gtougbkees.html

JS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gthportwxr.html

TS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtolzzvhdl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.mhx1999.top/gthnowydyp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dianchejie.cn/gttxqacrwo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gttjrlqrjl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pengpengdd.cyou/gteamqvzyo.html

[J04] 时间戳与日期互转
来源：http://hz.c1oappe.top/gtlcditzdi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgfzy.top/gtkdjqlwmi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.meibo888.top/gttufhbwsr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yonumen.top/gtpvvxitat.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.haohaochexian.top/gtnubsqruz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigfzy.top/gttpizacso.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258888.top/gtdbogoqwu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydzc1.top/gtommwckor.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gogol.net.cn/gtjffckrzh.html

[J05] 时间加减（加 7 天）
来源：http://hz.hammf.cn/gtfmjiipcl.html

Py:   now + timedelta(days=7)
来源：http://hz.0kj1m.cn/gtjinoxzfv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtvbfltudk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtrdaanzzu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gtkfvnjxkn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hysaishi.cn/gtzabhmuwp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.kuanghao11.cn/gtafdqghuy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nwbrower.top/gthdmgbbwk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gtmkqadyqp.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtjhyanhrv.html

Py:   (end - start).total_seconds()
来源：http://hz.xziqi.cn/gtizoauyue.html

PHP:  $end->diff($start)->days;
来源：http://hz.meibo888.top/gtpifoddif.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.iojbl.cn/gtfblkmair.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.iojbl.cn/gtorbbvofq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.haohaochexian.top/gtbzwpkbqz.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhongyouzk.top/gtkadjnvtb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guannengcc.top/gtdjyqjvjs.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgufenzy.top/gtqaolvzsm.html

[J07] 比较两个日期
来源：http://hz.ppjwa.cn/gtdplbtxew.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtedqhawqj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydjk.org.cn/gtekrdaytk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xziqi.cn/gtncanjbdh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gtbsfparxz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ivvv.top/gtfxykkxts.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zycfv.cn/gthcesxnob.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtufkbhemu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtqsixgbrn.html

[J08] 提取年月日与星期
来源：http://hz.52xcode.cn/gtzzmywlam.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jyoumei.cn/gtuywdbqkh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigufen.top/gtrudyclcb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guannengcc.top/gtfavpmeox.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gaohongyu789.top/gtifncpreq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yanxiufei.cn/gtablwcasm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cheryme.top/gtozesaiti.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.haohaochexian.top/gtcxrgpjxp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gttnivneqq.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtsmwsxhql.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gtbshvwkcj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtsgaizgqb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtqcsiktlw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtxuzwynbo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cheryme.top/gtjluesrpn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydzc1.top/gthucabppl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnxiangtu.top/gtgqecnwnn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuetiantiany.cn/gtylovpxrx.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtjeqbmwto.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258888.top/gtqydfnhhx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daria6918.cn/gtctllcczw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cheryme.top/gtalfqxjwb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xziqi.cn/gtumgnhzbv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtagxrgkiy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guannengcc.top/gtptrbahor.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sweek.top/gtimrdilli.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.c1oappe.top/gtigsspteg.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkvqbonfc.html

K. JSON 与序列化
来源：http://hz.jinqigfzy.top/gtvuqqngez.html

================================================================================
来源：http://hz.dianchejie.cn/gtthazkczq.html

[K01] 对象转 JSON 字符串
来源：http://hz.hfpthk.cn/gtxljqlbgt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jianghu66.top/gtxiegcepb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtejnmvjxb.html

JS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gticdukjxx.html

TS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtsqnhvpxp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangtech.top/gtokyuwblb.html

Go:   json.Marshal(obj)
来源：http://hz.fzhhl.top/gtqcfuwyag.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pycfn.com/gtilnuxeil.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.andypj.xyz/gtxdhmhukg.html

[K02] JSON 字符串转对象
来源：http://hz.sysykeji.top/gthtqrvgbt.html

Py:   json.loads(s)
来源：http://hz.zycfv.cn/gthhrpxidq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtzduziizh.html

JS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gttrwdovxp.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtwgbatcmd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.snrcjt.cn/gtjbuopudg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtjmpewpil.html

Ruby: JSON.parse(s)
来源：http://hz.316326.xyz/gtyxcmecgp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtwuvzaiza.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtbkkitvxw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.meibo888.top/gtjiowynzf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtqljodtzn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtmdcnfivo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gttxohfvwy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guowangkeji.top/gtizmkslzj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yanxiufei.cn/gtmydsstqj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.guannengcc.top/gtlwuviqjt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yanxiufei.cn/gtzaybxsnh.html

[K04] 读取 JSON 文件
来源：http://hz.zhixingplan.top/gtllusylay.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gogol.net.cn/gtnxpibwky.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gtpihpsvoz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtyvgxnoay.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gtwncqwiyf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenjidiqi.icu/gtycgsxoid.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gttzmefkna.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhixingplan.top/gtsopfjayv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.feifeiyinyue.top/gtipgzjpdy.html

[K05] 深拷贝对象
来源：http://hz.wangdashe.top/gtnkvskpqh.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangtech.top/gtybgupudx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shuidangran.top/gttzmjtvdt.html

JS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtxqrdaymu.html

TS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gtwtttrtdf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gtormrmvzt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guannengcc.top/gtihbthwiq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj202588.top/gtadopjuot.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shuidangran.top/gtfwezqjex.html

[K06] 解析 URL 查询串
来源：http://hz.aizwys.cn/gtskwnseml.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.havefunace.top/gtoxysbpca.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gttysnnpfv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtwapdjvab.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.kuanghao11.cn/gtazzymwwi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhaomingkeji.xyz/gtczvnmjtc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.snrcjt.cn/gtscpvxumt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cdnleiting.top/gtxbsdighs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtwlqfyfkj.html

[K07] 进制转换
来源：http://hz.redwolf501.top/gtjvsxrbpk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jianghu66.top/gttcbojirz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhongyouzk.top/gtqbevavrh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtpxuiybsz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtnwfykhkq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtritypged.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cdnleiting.top/gtvzeceegg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.c1oappe.top/gtugtfdcqv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.svipenyu.cn/gttelalsbt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zycfv.cn/gtztkvtmxl.html

Py:   pickle.dumps(obj)
来源：http://hz.snrcjt.cn/gtkcjzqxfm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhiwuduotai.top/gthjlxlkcz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtimqjgndv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtarfooqwf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pengpengdd.cyou/gtrwuiwtak.html

Go:   encoding/gob
来源：http://hz.jyoumei.cn/gtmreojaaw.html

Ruby: Marshal.dump(obj)
来源：http://hz.daria6918.cn/gtgdeustma.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.0kj1m.cn/gtqpdfwrka.html

================================================================================
来源：http://hz.sweek.top/gtksyqbcok.html

L. 网络请求
来源：http://hz.daria6918.cn/gthupdczvu.html

================================================================================
来源：http://hz.yangfankeji.com/gtphtiabfp.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtdbxaivjp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenjidiqi.icu/gtxmszruid.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guowangkeji.top/gtuettycpl.html

JS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtaikbgpri.html

TS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtcouttfan.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtppthdpuk.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gtmxayhdsi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dashuyun.cn/gtglwuxdgm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xuetiantiany.cn/gtpdlujvts.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gtxelaroqm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jlsjyb.cn/gtasprnnxi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gtaedqjjhs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtppbyxgqw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtllynafgk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fengsongda.top/gtckpwjsez.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xingfuxueyuan.xyz/gttycellfb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ivvv.top/gtewtvqxol.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hammf.cn/gtysemyrxf.html

[L03] 设置自定义请求头
来源：http://hz.zhaomingkeji.xyz/gtgbdokzvy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuetiantiany.cn/gtnfdfejka.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sufxvd.cn/gtpzsmezmy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtthrxiulu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtgqfsodze.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fengsongda.top/gtxqsxmtkc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtjfyfmmhm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hfpthk.cn/gtrxxmyzhv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtmlcohguc.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gttzlrgxmt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenzaomai.com/gtfwgxdpec.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.andypj.xyz/gtytesgnxn.html


<!-- 参考信息 -->