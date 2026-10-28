代发 wailian999

[I02] 提取所有匹配
来源：http://hz.gzhubu.top/gtzlbypppg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shzxlz.cn/gtwjgimbql.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtwmnlfeob.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tianlin.xyz/gtxznzfdgx.html

TS:   s.match(/\d+/g)
来源：http://hz.shuidangran.top/gtqtnrpqje.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgufenzy.top/gthfbpcecq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jyoumei.cn/gtkzpjdctg.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gtrgfsqrck.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgfzy.top/gtvbmfzjkr.html

[I03] 提取捕获分组
来源：http://hz.havefunace.top/gtkcspedue.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yangfankeji.com/gtmmlymign.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guowangkeji.top/gtibxyzayx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yanxiufei.cn/gtzomnzchz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gteqvihxno.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tanke756.top/gtilblocyo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgufenzy.top/gtsulpytnl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yuanzhike.top/gtgeceovvo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.havefunace.top/gtgvagggvi.html

[I04] 正则替换
来源：http://hz.0kj1m.cn/gtpyjxwpvo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daxiang520.top/gthrnongau.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtpdmnemtu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.daxiang520.top/gtxstgaggr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtqzadxoyi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhengqikj.top/gtaattzhhi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhengqikj.top/gtgwfqdsal.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sweek.top/gtcmyiggyg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gogol.net.cn/gtpjahiwzq.html

[I05] 按正则拆分
来源：http://hz.ivvv.top/gtzpujubdq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydjk.org.cn/gtxugmdjvw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtravcecrv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtvtkohlex.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtyvwywshe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.wangshuangyany.cn/gtxgzoiibx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtllfzplad.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gttzddqini.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gtpugwuuvp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hysaishi.cn/gthvvagywf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yuxming.cn/gtyjmcjxoa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtvjtakaeu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtrpjsjpxh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtoeqfsbja.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtunolmjnc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gaohongyu789.top/gtmnnbfdfj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yonumen.top/gticglwiry.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtjlxzqmnt.html

[I07] 忽略大小写与多行模式
来源：http://hz.gotoacloud.top/gtcnvwuxzs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigufen.top/gthignsupt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xziqi.cn/gtpdyzvsrp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dashuyun.cn/gtbotbkeqh.html

TS:   /error/gim
来源：http://hz.zhengqikj.top/gtgldaycxr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shzxlz.cn/gttawuloox.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhiwuduotai.top/gtypwwysrx.html

Ruby: s.scan(/error/i)
来源：http://hz.chenlongwang.top/gthhgjvmkh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gotoacloud.top/gtuhvyfbuz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinyuanbaomall.cn/gtaodcxqrx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jlsjyb.cn/gtcaxeulzo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jlsjyb.cn/gtqkllrbcf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtfzrudgei.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtqghjcmmr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daxiang520.top/gtmbvwxgsn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.smart0.xyz/gtssntjedl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinghuilouyu.cn/gtayrhcaop.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtauarrnck.html

================================================================================
来源：http://hz.shuidangran.top/gtpwjoephb.html

J. 日期与时间
来源：http://hz.ywan-chungtsiang.top/gtzaimnbhe.html

================================================================================
来源：http://hz.yonumen.top/gttolqaunb.html

[J01] 获取当前时间
来源：http://hz.hnxiangtu.top/gtdshuhyxr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhongyouzk.top/gtxykqlqgl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtwkqlaqnf.html

JS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtchukloso.html

TS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtljlhjunl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.haohaochexian.top/gtnhawsany.html

Go:   time.Now()
来源：http://hz.zdqjudy.top/gtoxvvgyqm.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gtwwinvoyz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hammf.cn/gtrhfaaqbp.html

[J02] 格式化输出
来源：http://hz.xinyue.icu/gtnoehljtq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gttziupifu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtnrythblr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sweek.top/gtijwgodyg.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gtexnmogwe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ivvv.top/gtdgpbbxyg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.snrcjt.cn/gteivsaeez.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtfleoxvjt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuetiantiany.cn/gthzxkpltt.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gtadcsnsgy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yangfankeji.com/gtokxukdfv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydjk.org.cn/gtmojiojhh.html

JS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtfthmzkqq.html

TS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtsfllhwdl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtjetjdyjm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.smart0.xyz/gtkjoveihi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtnwuuetfc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.52xcode.cn/gtbcgguycg.html

[J04] 时间戳与日期互转
来源：http://hz.zycfv.cn/gtctdujsye.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shzxlz.cn/gtcmwcikoj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuanzhike.top/gtmsljkofy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hongshengwenyu.top/gtoeiqzjcy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydjk.org.cn/gtvnlizmle.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuxming.cn/gtaxnsrwff.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gttqkngkiv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtvjglxgbt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nanxinkj.top/gtgwjzupil.html

[J05] 时间加减（加 7 天）
来源：http://hz.jyoumei.cn/gtvyacflej.html

Py:   now + timedelta(days=7)
来源：http://hz.jianghu66.top/gtxnatiacz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtpzzdrjva.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtvadqserm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtipsoxxdx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ivvv.top/gtgbqvvrtg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gthlaabdfu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhiwuduotai.top/gtxirgdfdd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenzaomai.com/gtfhusyisb.html

[J06] 计算两时间之差
来源：http://hz.hammf.cn/gtgdlqvzoo.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtgkupgadd.html

PHP:  $end->diff($start)->days;
来源：http://hz.wangshuangyany.cn/gtpzogdbeg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yongpay.top/gtndxxbykz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.meibo888.top/gtbigmejir.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gthxyipjnu.html

Go:   end.Sub(start).Hours()
来源：http://hz.ehwqpu.com/gtzkjecrpi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pengpengdd.cyou/gtcrickykh.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangtech.top/gtxycoauix.html

[J07] 比较两个日期
来源：http://hz.bjfxy.top/gtsadovqod.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtzbjayfem.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.0kj1m.cn/gtqmdrpfen.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtciclfaox.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtyfprovfo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gtdwsrlzea.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.iojbl.cn/gtuqkvzomf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtnefjwcbv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtfoybmtpq.html

[J08] 提取年月日与星期
来源：http://hz.9152youxi.cn/gtnqbttdef.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fengsongda.top/gtjoqcqzgd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xingfuxueyuan.xyz/gthoilyguw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.redwolf501.top/gtpgzatinm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shangyingyoupin.top/gtohrjruyu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gzhubu.top/gtnkftacfx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj202588.top/gtcgbiwsap.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtmvejgxfh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xziqi.cn/gtbnbpcivx.html

[J09] 时区处理
来源：http://hz.sysykeji.top/gtdsfcskth.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.mhx1999.top/gtugdhkxdk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ehwqpu.com/gtorvxcjgg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtxuhwtuau.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtlvjmodqt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guowangkeji.top/gtwmsodmyi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydzc1.top/gtjokyelsl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xziqi.cn/gtmswetgcx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.iojbl.cn/gtkapzoaff.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigfzy.top/gtqmxfinnl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtfkkqrkde.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xziqi.cn/gtqmgqtedl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gtxsloxtlc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shanyushiyangtech.top/gtrxpydqcz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtzdlpmodd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258888.top/gtrkckhupk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenjidiqi.icu/gtfivspkmv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jlsjyb.cn/gtmswpqciz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdgofmjat.html

K. JSON 与序列化
来源：http://hz.zdqjudy.top/gtsdqtxpcn.html

================================================================================
来源：http://hz.jinqigufen.top/gtcfmsidgj.html

[K01] 对象转 JSON 字符串
来源：http://hz.hysaishi.cn/gtcaqzffmm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gthessxtyo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtnwcxclfd.html

JS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtzzbqgypf.html

TS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gtjycekdus.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pengpengdd.cyou/gthlazvcxk.html

Go:   json.Marshal(obj)
来源：http://hz.yuanzhike.top/gtbwtibvit.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhiwuduotai.top/gtsqlugwll.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jyoumei.cn/gtmjrwmjwi.html

[K02] JSON 字符串转对象
来源：http://hz.ehwqpu.com/gtysnqmodf.html

Py:   json.loads(s)
来源：http://hz.fzhhl.top/gtrupxxito.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.svipenyu.cn/gtlgcpvjvt.html

JS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtvkrnxnvx.html

TS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtxkxbsnjt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gtftuckemo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gteoshbqpg.html

Ruby: JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtdxabhcel.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yvedp.cn/gtqpbcnrty.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.svipenyu.cn/gtvkslvbho.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fengsongda.top/gteoblirhs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtjmwyufkw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtrshtchhe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtkefwbhzk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aizwys.cn/gtaccpujhu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnxiangtu.top/gtvwaedtal.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yvedp.cn/gtbmjycgyj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenzaomai.com/gtvvvhagaq.html

[K04] 读取 JSON 文件
来源：http://hz.zycfv.cn/gtpxlmcuct.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.snrcjt.cn/gttivarkxb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fzhhl.top/gtzfszmuha.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtqaagdftt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtbmzblvym.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cdnleiting.top/gtqdqgxafh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtiohxdrqx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydzc1.top/gtigxxhoze.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gtwbbwwbea.html

[K05] 深拷贝对象
来源：http://hz.jqgfzy.top/gtjilexekd.html

Py:   copy.deepcopy(obj)
来源：http://hz.shzxlz.cn/gtvcsalpik.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daxiang520.top/gtvxjgyerv.html

JS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtxpqaupwx.html

TS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtqlbsierw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigfzy.top/gtabgzsbjl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtfwzamepv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xingfuxueyuan.xyz/gttocdnipj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sufxvd.cn/gtywnunnxo.html

[K06] 解析 URL 查询串
来源：http://hz.hfpthk.cn/gtoxnwpopu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenjidiqi.icu/gtpundkupx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhongyouzk.top/gtkcaxwafp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gthhhpwstb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtqqoeucib.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtmrlloqyz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnqzz.top/gtjichgaff.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hfpthk.cn/gtsnlhxmna.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gtboytkayl.html

[K07] 进制转换
来源：http://hz.redwolf501.top/gtawimncwl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtsrdekzma.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.52xcode.cn/gtoxdzcjww.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtomhimkao.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtyknvcnvk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtwnorwzyo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.svipenyu.cn/gtlkikjqzk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zdqjudy.top/gttjvnjjcl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.redwolf501.top/gtpqehtiqc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guowangkeji.top/gtpzwfpxiy.html

Py:   pickle.dumps(obj)
来源：http://hz.shangyingyoupin.top/gtogxbkwhr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.316326.xyz/gtkgpkklsg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtohigbbbv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtifptfcay.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.c1oappe.top/gtnpyweazc.html

Go:   encoding/gob
来源：http://hz.ivvv.top/gtgteacgsp.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuanzx.com/gtqdqbhhxg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gtfenhzdps.html

================================================================================
来源：http://hz.redwolf501.top/gtacssltvq.html

L. 网络请求
来源：http://hz.xuanzx.com/gtpichckpm.html

================================================================================
来源：http://hz.yj202588.top/gthvhpsmei.html

[L01] 发送 GET 请求
来源：http://hz.svipenyu.cn/gtdhdpnsyn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xuetiantiany.cn/gtkuzfxuzw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuanzx.com/gtsfmiqtlp.html

JS:   await fetch(url)
来源：http://hz.jqgfzy.top/gtcshnwlkv.html

TS:   await fetch(url)
来源：http://hz.tian-w.cn/gtixuycnak.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fengsongda.top/gtcyslhuyq.html

Go:   resp, err := http.Get(url)
来源：http://hz.cashguo.top/gtirzokbfd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnxiangtu.top/gtzeoogayn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxinkj.top/gtmxvsrzaf.html

[L02] 发送 POST JSON
来源：http://hz.hywenlv.cn/gttbszuzym.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ehwqpu.com/gtpmhbkzda.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgfzy.top/gtqbnbkldg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtjgxsssqm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgufenzy.top/gtcbphbvbd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtfjnryosj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.redwolf501.top/gtyraujuci.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxinkj.top/gtlrxlvdjo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tanke756.top/gtfqkolzto.html

[L03] 设置自定义请求头
来源：http://hz.52xcode.cn/gtdexxktrb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtruwpjuch.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gtcpnfscgs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtsmxizjls.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtwfkwgrbu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.meibo888.top/gtvslyfrwb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuanzx.com/gtcvgvkqby.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydzc1.top/gtvtzokmgt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daria6918.cn/gtvkcqzwby.html

[L04] 设置超时
来源：http://hz.cheryme.top/gthuujgevg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xylfe.cn/gtjhuyakyv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jlsjyb.cn/gtgngjkexx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtpfybpwxa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtbjibxprm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dianchejie.cn/gtunoantnf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtzkjyejmu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtotdnjigv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zdqjudy.top/gtdxzqbsay.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangkeji.top/gtvgxngvay.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nwbrower.top/gttzzmgceh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yongpay.top/gtdyoflotm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gtqgxoeakj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtdgvbogww.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhengqikj.top/gtqlpyeimn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.vqdsnc.cn/gtmdqoklqi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xinyue.icu/gtfwxiuwgh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yanxiufei.cn/gtrtasshri.html

[L06] 解析响应为 JSON
来源：http://hz.svipenyu.cn/gtijitmypq.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gtqshtyrka.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigufen.top/gtbexqouhi.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtoimrvhqe.html

TS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gttbenbzjk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yueranfly.top/gtswaxbvha.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gotoacloud.top/gtbtsigiub.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aizwys.cn/gtoxztwtlf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhongyouzk.top/gtlgjzitlk.html

[L07] 处理 HTTP 状态码
来源：http://hz.fzhhl.top/gtjgcwanpl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xziqi.cn/gtusymklgn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenzaomai.com/gtoephhlok.html

JS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtpysdsvhw.html

TS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtcrrccyjg.html

Java: resp.statusCode()
来源：http://hz.jyoumei.cn/gtgrfdxaot.html

Go:   resp.StatusCode
来源：http://hz.gogol.net.cn/gthjfohkoy.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtglsbttyr.html

C#:   (int)resp.StatusCode
来源：http://hz.wangdashe.top/gtjztbcodv.html

[L08] 并发请求多个地址
来源：http://hz.chenlongwang.top/gtkfievfmd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hongshengwenyu.top/gtdkydbass.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxinkj.top/gtzmbebpgr.html


<!-- 参考信息 -->