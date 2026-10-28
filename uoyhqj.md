代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.meibo888.top/gtydmoxrek.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtzensmyij.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhaomingkeji.xyz/gtoksyagnu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daxiang520.top/gtcvtakmri.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cheryme.top/gtdroudsli.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gteimkbzpi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ywan-chungtsiang.top/gtzhtjamuc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xinyue.icu/gtevsjjsap.html

================================================================================
来源：http://hz.yuxming.cn/gtbhsksbwg.html

I. 正则表达式
来源：http://hz.kuanghao11.cn/gtszfmlafu.html

================================================================================
来源：http://hz.zhengqikj.top/gtirkjwzwn.html

[I01] 判断是否匹配
来源：http://hz.jinghuilouyu.cn/gtzgzgesve.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cucudq.cn/gtqprouwph.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yonumen.top/gtzfocxkkx.html

JS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtxwshfhbr.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtisxaumym.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gthdccpylo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gzhubu.top/gtjixwgcxf.html

Ruby: s.match?(/\d+/)
来源：http://hz.xziqi.cn/gtnhwqbidu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.vqdsnc.cn/gtbkphgmzf.html

[I02] 提取所有匹配
来源：http://hz.yuanzhike.top/gtqkwsijcb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtkropijad.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cucudq.cn/gtrzucortq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gtmsuicsqp.html

TS:   s.match(/\d+/g)
来源：http://hz.xylfe.cn/gtunidpwcn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sysykeji.top/gtnylofbip.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cqqwz.cn/gtgnsstjzu.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtxtwpwdyj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hfpthk.cn/gthsnsrfrq.html

[I03] 提取捕获分组
来源：http://hz.yj202588.top/gtmdpwfghd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258888.top/gtylbrrvus.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.0kj1m.cn/gtcslydpbv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxuanxn.top/gtjyzzrfyw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gtqsjlsgax.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yanxiufei.cn/gtwcwedtoe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydjk.org.cn/gtobbcinvz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtpgdljvwr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhoulong.xyz/gtqcxruowi.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtbkyzokuk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.redwolf501.top/gtzcxdskis.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtlgqklify.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtogdeekku.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gteaoerseq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pycfn.com/gteutqhqww.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.iojbl.cn/gtmqfqfvot.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tianlin.xyz/gtmtumwgxx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtcqwvjlek.html

[I05] 按正则拆分
来源：http://hz.jinqigufen.top/gthnjahrtg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jlsjyb.cn/gtheufodff.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hfpthk.cn/gtsmhoyrex.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtwvzabxyq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtcjvzafem.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtoriofbpc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj20258.top/gtmjrzpzpl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtkoufmqhs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgfzy.top/gtkpyfvwlq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gaohongyu789.top/gtprccytdm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtrsyubyxi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cdnleiting.top/gtckpmpqvq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtqqquaueo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtsjtwayik.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangdashe.top/gtfljwgumi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhixingplan.top/gtgumdezsg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zycfv.cn/gtzsrpjxdb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtzbniddkx.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhongyouzk.top/gtogkrjiim.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gtpijafgjx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtkbjxpzzu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guannengcc.top/gtsebumocv.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtmmghjwvb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenzaomai.com/gtanyjwikm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhixingplan.top/gtcjjpdugs.html

Ruby: s.scan(/error/i)
来源：http://hz.sysykeji.top/gtfrfvqapn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtyeuwqaqr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.aibaodan.cn/gtnzxetjac.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cucudq.cn/gtzcufotxi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.kuanghao11.cn/gtmwouphvr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtctkaoukv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtodhtuoup.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtlwfdpqay.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yanxiufei.cn/gtwnmbydlx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtehkjjymi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gtsgrntesg.html

================================================================================
来源：http://hz.9152youxi.cn/gtfbhlgwqk.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gtamuylpbj.html

================================================================================
来源：http://hz.cheryme.top/gtmpvsntog.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gtflhutshi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigfzy.top/gtrlkmhruj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtophxuobn.html

JS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtnqvtupoq.html

TS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtecmusrjv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.9152youxi.cn/gtubxyogbs.html

Go:   time.Now()
来源：http://hz.gzhubu.top/gtnifhauch.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtpfdgdgjm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sysykeji.top/gtaujgekrm.html

[J02] 格式化输出
来源：http://hz.jinqigfzy.top/gthnjhdiar.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtukgzzupw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtkpxiteov.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydjk.org.cn/gtamvzwode.html

TS:   d.toISOString()
来源：http://hz.hongshengwenyu.top/gtgxorjfsn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ybcxt.top/gtdxsruals.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gzhubu.top/gtxjevykef.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtaphgndae.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtmbvqioiy.html

[J03] 字符串解析为日期
来源：http://hz.yj20258.top/gtfgbduhoc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yvedp.cn/gtndyakgmy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.kuanghao11.cn/gtheptwbod.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtybfvqdid.html

TS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtndplmhuq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtfsdggsvw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gzhubu.top/gteasbeoln.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtkysesxta.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hongshengwenyu.top/gtiypgpkdo.html

[J04] 时间戳与日期互转
来源：http://hz.xingfuxueyuan.xyz/gtbxnhetqq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenlongwang.top/gthoisjjeq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.birdmap.top/gtqvfnsgsv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtivmjkotd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ywan-chungtsiang.top/gtteqerddi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zycfv.cn/gtktnatebs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.smart0.xyz/gtfuvfzsxt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.feifeiyinyue.top/gteothgsst.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.0kj1m.cn/gtcozwltwr.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangtech.top/gtnodutbqp.html

Py:   now + timedelta(days=7)
来源：http://hz.cheryme.top/gtxjobtktp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sweek.top/gtgeqmmymn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtnojhcuwq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gtaytfitpo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigufen.top/gtjjupdwkd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.svipenyu.cn/gtreruoqbl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gtjmvrtnvz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ywan-chungtsiang.top/gttnnowfky.html

[J06] 计算两时间之差
来源：http://hz.kuanghao11.cn/gtepzgempw.html

Py:   (end - start).total_seconds()
来源：http://hz.nwbrower.top/gtlqkfquuq.html

PHP:  $end->diff($start)->days;
来源：http://hz.cashguo.top/gtojxslckb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxinkj.top/gtcwwwnlhe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ybcxt.top/gtlcrkgrzn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hfpthk.cn/gtrahmteqj.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhaomingkeji.xyz/gtlxpbiprk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hfpthk.cn/gtrlbtcvpf.html

C#:   (end - start).TotalSeconds
来源：http://hz.iojbl.cn/gtfynwcrfm.html

[J07] 比较两个日期
来源：http://hz.zhixingplan.top/gtwzjfqpqe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtodrdgpbi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sufxvd.cn/gtvuiuusst.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtfdsnqmiv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtwjgrnxne.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.quarkkingdee.top/gtmfgplkjl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aibaodan.cn/gtavcodyph.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtsehzsqvv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtdnzjppdb.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gthovsfuhe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dianchejie.cn/gtypdqtnrk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.c1oappe.top/gtukpxlact.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhaomingkeji.xyz/gtdndxohtq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aibaodan.cn/gtcrrkwjua.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtnudshybr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yvedp.cn/gtaeswjein.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daxiang520.top/gthwqdjrzh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nwbrower.top/gtaibwobzt.html

[J09] 时区处理
来源：http://hz.jyoumei.cn/gthccbewar.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtrgxjrpur.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhengqikj.top/gtgkxrwzes.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gtnnqnpftg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtzqaneyns.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aizwys.cn/gtqcrqyfkl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnxiangtu.top/gtdbtduwjp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cheryme.top/gtukvosqqb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.meibo888.top/gtcmyhlbeg.html

[J10] 取今天 / 本月第一天
来源：http://hz.gotoacloud.top/gtnyzwgaws.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jianghu66.top/gtitimelid.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tianlin.xyz/gtvctnonuc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtvvxuhgmz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shangyingyoupin.top/gtqfmeczsg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.9152youxi.cn/gtqbmfidca.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ivvv.top/gtipamxxmb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dianchejie.cn/gtkyzoppkk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gtuoagtxgx.html

================================================================================
来源：http://hz.zhijiandao.cn/gtjksptetr.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gtedxypnse.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkuzgxzkj.html

[K01] 对象转 JSON 字符串
来源：http://hz.ppjwa.cn/gtiiswufsp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtcesxhxjg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtsagdqhsg.html

JS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtafxwpbsy.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gttjxrjspl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gtekadakti.html

Go:   json.Marshal(obj)
来源：http://hz.ybcxt.top/gtvreytdgp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigufen.top/gtmxwcdkjm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtawgsxobj.html

[K02] JSON 字符串转对象
来源：http://hz.zhijiandao.cn/gtfeaobmou.html

Py:   json.loads(s)
来源：http://hz.cashguo.top/gtjqztrgsl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.svipenyu.cn/gtdsvwdyrj.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtxzvypqaj.html

TS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtplcmrsrh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxinkj.top/gtbrfrcwjh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtfpmkmbxt.html

Ruby: JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gthezpejub.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenlongwang.top/gthxffxtie.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtpbthlkdf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtrfrsgjee.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtbgsbdczy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtryttpolm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtjxypjhfs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnqzz.top/gthslbyhqp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangkeji.top/gtlnghxrqj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nwbrower.top/gtpvtrplit.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhoulong.xyz/gtguypkfbr.html

[K04] 读取 JSON 文件
来源：http://hz.gogol.net.cn/gtxegxcotl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.svipenyu.cn/gtedxxvbon.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtbuwxbnbj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtmdqkcdxl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gtnlprsphq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhongyouzk.top/gtwkojyxir.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtszilkcrb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xingfuxueyuan.xyz/gtqdnxxokv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jqgufenzy.top/gtliaavkmy.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtduoysjfg.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtdvccadac.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daria6918.cn/gtapizydlu.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtwsnenurf.html

TS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtieuttaum.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gtmyohqbzy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xziqi.cn/gtoxpzmayl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fzhhl.top/gtbuazhuyc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gtvjlcktzz.html

[K06] 解析 URL 查询串
来源：http://hz.jiagoushi.top/gtuuowmkjg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tian-w.cn/gtyebgxslw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuanzx.com/gttyglhpuw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtqxapdrzf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtmmmgtnqn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxinkj.top/gttdlxmbtk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtfgtfbbpq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtxazsnjcm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tanke756.top/gtutumhdnp.html

[K07] 进制转换
来源：http://hz.cheryme.top/gtroztidds.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtxsmxulsb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dianchejie.cn/gttcmiatut.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtiuspiisq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtwqiwbwxy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtajfkhqxm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.vqdsnc.cn/gtadzskhee.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtqjknllob.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gtmxnljayb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.vqdsnc.cn/gtwbcdvuba.html

Py:   pickle.dumps(obj)
来源：http://hz.jinyuanbaomall.cn/gteucpqsoj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shzxlz.cn/gtwkbfrkvw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtozhurmpv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtfjuyzxfu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dianchejie.cn/gtzxjsufmw.html

Go:   encoding/gob
来源：http://hz.ppjwa.cn/gtoibfpulo.html

Ruby: Marshal.dump(obj)
来源：http://hz.dianchejie.cn/gteqzbqtqw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sweek.top/gthtiqxmjf.html

================================================================================
来源：http://hz.aizwys.cn/gtugqwccpy.html

L. 网络请求
来源：http://hz.andypj.xyz/gtfzrygsfv.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtggzaumiy.html

[L01] 发送 GET 请求
来源：http://hz.xuanzx.com/gtvmsbjlyf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.iojbl.cn/gtxbryzgoz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtmeyhubys.html

JS:   await fetch(url)
来源：http://hz.iojbl.cn/gtqzfwcjoj.html

TS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtunqsmgok.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daxiang520.top/gthvrrpgdn.html

Go:   resp, err := http.Get(url)
来源：http://hz.andypj.xyz/gtiedtukfi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj20258.top/gtnrcffitx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gttcgjibvz.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtdzxirqgi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gtcsnhtrvy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zycfv.cn/gtqlmgtroc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtxzgycwbc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtladxfguq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnxiangtu.top/gtpphfuvio.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.52xcode.cn/gtewvpyzfj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ybcxt.top/gtmntkcjtp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jyoumei.cn/gtznbkcdok.html

[L03] 设置自定义请求头
来源：http://hz.pengpengdd.cyou/gtojcebxpp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shzxlz.cn/gtckeqltes.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jlsjyb.cn/gtbfohupvo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtrxgnhugl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtyoncwugu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daria6918.cn/gtjkrvygkh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yonumen.top/gtsmrlvxvg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.9152youxi.cn/gtmfwfkkoq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tanke756.top/gttxdzfsvt.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gtrljrqqnc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnxiangtu.top/gtkmdllqiz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hysaishi.cn/gtlukrgfcd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtdztuxxkb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtxmrmelba.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gtzdycgvdr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtvjymrtke.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gttnjreggj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gttizzmosk.html

[L05] 上传文件（multipart）
来源：http://hz.yongpay.top/gtitkbpsny.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.feifeiyinyue.top/gtdsnufkuu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.havefunace.top/gtqqvppgxz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.9152youxi.cn/gttgnykmgc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtlrtevlyu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nwbrower.top/gtoxeflvpb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.wangdashe.top/gtuothdhqf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ydzc1.top/gtyglvcsdc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.c1oappe.top/gthjabfohh.html

[L06] 解析响应为 JSON
来源：http://hz.chenjidiqi.icu/gtyllpfzfg.html


<!-- 参考信息 -->