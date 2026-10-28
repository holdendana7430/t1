代发 wailian999

================================================================================
来源：http://hz.quarkkingdee.top/gtbbfflxuk.html

I. 正则表达式
来源：http://hz.iojbl.cn/gttlddhbyd.html

================================================================================
来源：http://hz.zhixingplan.top/gtfyejeykt.html

[I01] 判断是否匹配
来源：http://hz.ehwqpu.com/gthevvdxxe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258.top/gtldnxspoa.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nanxuanxn.top/gtawgzubnd.html

JS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtjfbgwqqc.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtekejeoik.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.birdmap.top/gtopqczxux.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigfzy.top/gtojetwcrj.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtqelzebxf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gtrwvxnmrd.html

[I02] 提取所有匹配
来源：http://hz.yuxming.cn/gtxpljlmqz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.9152youxi.cn/gtclraguqg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gtgwazlfqv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.haohaochexian.top/gtjczstklu.html

TS:   s.match(/\d+/g)
来源：http://hz.hywenlv.cn/gtylyzmvmc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gotoacloud.top/gtqgquyfhl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtngoafdmb.html

Ruby: s.scan(/\d+/)
来源：http://hz.0kj1m.cn/gtldgvuyir.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ivvv.top/gtjqmrngzu.html

[I03] 提取捕获分组
来源：http://hz.gotoacloud.top/gtdolkbkom.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigfzy.top/gtvioiaqcu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.aibaodan.cn/gtogyjzrmz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nwbrower.top/gtxquvhtww.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydzc1.top/gtmmtnvuli.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cdnleiting.top/gtfgtlhgga.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.meibo888.top/gttrwhokvb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yangfankeji.com/gtzemzsshf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxinkj.top/gtwkxxfpbp.html

[I04] 正则替换
来源：http://hz.sweek.top/gtjkjxtxqi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.smart0.xyz/gtlmrctfni.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtqemwtjxf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtsqpwlqhc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtaikldcft.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydjk.org.cn/gtluvkkcvu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cashguo.top/gthnkpgsyp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.redwolf501.top/gtedvhivaz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hywenlv.cn/gtiyhdjrkc.html

[I05] 按正则拆分
来源：http://hz.316326.xyz/gtrqcptvvj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuxming.cn/gtddseroqd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yongpay.top/gtmwituwoy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtzkpetbft.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtxhrdvltv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinyuanbaomall.cn/gtqgyaokft.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cheryme.top/gtyqsylcix.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtwxgpapbc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yonumen.top/gtukqkcepm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hysaishi.cn/gtkxtvmlbe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yuanzhike.top/gtbfdhpwnt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtepznzdkv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtipujahbv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtnorroose.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ppjwa.cn/gtcdgfmnwx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ybcxt.top/gttotwjljh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daxiang520.top/gtcdrvcgdx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtwjfyoydv.html

[I07] 忽略大小写与多行模式
来源：http://hz.yanxiufei.cn/gtkdiactbi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ppjwa.cn/gtjpfsxdau.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cashguo.top/gtuedueyrf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258.top/gthgylwsqf.html

TS:   /error/gim
来源：http://hz.jinqigufen.top/gtymelvkjw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.9152youxi.cn/gtfxabmrjk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gotoacloud.top/gtcaergcdp.html

Ruby: s.scan(/error/i)
来源：http://hz.pengpengdd.cyou/gthfsywvai.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.havefunace.top/gtwuophcjt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gogol.net.cn/gtgahrqftg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jiagoushi.top/gtkcirobmu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.meibo888.top/gtdadcaqmj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtxvprytyn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gtyyvahkpv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fzhhl.top/gtcjftcets.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gtptloqaur.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.svipenyu.cn/gtikdprvaz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtiyqkdvua.html

================================================================================
来源：http://hz.pycfn.com/gtsducukql.html

J. 日期与时间
来源：http://hz.snrcjt.cn/gtrfxavjhq.html

================================================================================
来源：http://hz.chenzaomai.com/gtphkpdllw.html

[J01] 获取当前时间
来源：http://hz.cheryme.top/gttoppcqcf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtrzlsciyg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtirlichmr.html

JS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtjpwpjfjj.html

TS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gtrljoorsr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gtfcquydvs.html

Go:   time.Now()
来源：http://hz.pycfn.com/gtkfywkdsr.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtgfgefupi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangtech.top/gtsgqugqrd.html

[J02] 格式化输出
来源：http://hz.jinghuilouyu.cn/gtkmrimdtd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtnkcjorve.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtlbcgxbgs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtqssjqcjd.html

TS:   d.toISOString()
来源：http://hz.zhoulong.xyz/gtdhfjpdgd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhiwuduotai.top/gtwgwmupri.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnxiangtu.top/gtjqfrfots.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtlvkqwggt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.smart0.xyz/gtrcztmwfg.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtyordbazr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinyuanbaomall.cn/gtxxkyokhs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hnxiangtu.top/gtxaihsthq.html

JS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtkbgpmtqv.html

TS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtncxmfevc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gtlcwgbmxi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yueranfly.top/gtazfqjxlu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtvzmonqsp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.smart0.xyz/gtfcwwrrrp.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtemqcbzdp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tanke756.top/gtewtagxry.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.bjfxy.top/gttcxsjmzz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuxming.cn/gtwolvouaj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtiwfvirwh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cashguo.top/gtgngorgvw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ppjwa.cn/gtkqdwwudo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gthfvkbrwu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.meibo888.top/gtqaucfgjc.html

[J05] 时间加减（加 7 天）
来源：http://hz.havefunace.top/gthwjidsts.html

Py:   now + timedelta(days=7)
来源：http://hz.fzhhl.top/gtyvhspdtb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jyoumei.cn/gtwkkrjezm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gthmnpeoki.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gttxvpamas.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.52xcode.cn/gtuxnospsv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.meibo888.top/gtnehmxkdt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pycfn.com/gtyfvvfsjt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yonumen.top/gtktrdtpuh.html

[J06] 计算两时间之差
来源：http://hz.hongshengwenyu.top/gtfactzmmw.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgfzy.top/gtsocrbfib.html

PHP:  $end->diff($start)->days;
来源：http://hz.cashguo.top/gtnmjudzou.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.redwolf501.top/gtxerxcaot.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ppjwa.cn/gttrbcgjae.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.bjfxy.top/gtmqhppltk.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj202588.top/gtjqwoffqe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.9152youxi.cn/gtumomnmlv.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhengqikj.top/gtvcfjrfnb.html

[J07] 比较两个日期
来源：http://hz.guowangkeji.top/gtdturqucb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtbsqojuqk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aizwys.cn/gtdqjupdex.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtwnfuyjll.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gthxrraiaz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuetiantiany.cn/gtbmjudoqn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtzmlydrqr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtoprilodm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtleubmawc.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtprmcqnpb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnqzz.top/gtebczielj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtvepzdnbp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhengqikj.top/gtbmncxntk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ppjwa.cn/gtnrrlikpo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jlsjyb.cn/gtirswbxhp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ywan-chungtsiang.top/gtxgikokwl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtlnwlwwgd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtaejxyvpp.html

[J09] 时区处理
来源：http://hz.mhx1999.top/gttpjtmuvt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guowangkeji.top/gtltmxervd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hywenlv.cn/gtivvnxjzq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtbzndkcpa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtgysxzqhc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.redwolf501.top/gtwrqutacy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ybcxt.top/gthxggaqsl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtluyllqis.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yangfankeji.com/gtcwxhklyt.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtkeekcxxp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangtech.top/gtdoeuayla.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hongshengwenyu.top/gttsiifevc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tanke756.top/gtdgkzoyha.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.havefunace.top/gtafahuxkm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xingfuxueyuan.xyz/gteeyghlkd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yonumen.top/gtizaqaolz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.smart0.xyz/gtjcttbrah.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.kuanghao11.cn/gtejoygdth.html

================================================================================
来源：http://hz.snrcjt.cn/gthntwakbc.html

K. JSON 与序列化
来源：http://hz.ywan-chungtsiang.top/gtucknqtyr.html

================================================================================
来源：http://hz.cqqwz.cn/gthciyexiv.html

[K01] 对象转 JSON 字符串
来源：http://hz.cashguo.top/gtxtxdcphj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtzcimhqrb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtyitvpbxv.html

JS:   JSON.stringify(obj)
来源：http://hz.hnqzz.top/gtgvrooepa.html

TS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtcdvncxbc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jyoumei.cn/gtqbsarzwv.html

Go:   json.Marshal(obj)
来源：http://hz.yj202588.top/gtpsuoscsc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shzxlz.cn/gtwzghasdd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cashguo.top/gtlprmmfaa.html

[K02] JSON 字符串转对象
来源：http://hz.gaohongyu789.top/gtxuyphwlz.html

Py:   json.loads(s)
来源：http://hz.jinyuanbaomall.cn/gtfxbnmtrh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtlacvpspr.html

JS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtwcrpaqfn.html

TS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtjepcydoj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtukgcktza.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtmhabwsrv.html

Ruby: JSON.parse(s)
来源：http://hz.yangfankeji.com/gtsijfogmt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pycfn.com/gtoifafpca.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gthaftfoha.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtjanlvnji.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtevwtmahw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtrkpalewq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtimqxpybf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gttdxnqgzv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yueranfly.top/gthhadhuma.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xuetiantiany.cn/gtvvfvteli.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.316326.xyz/gtnacxjabb.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gttwyzwfyb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yonumen.top/gtjfbqpfzm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gtbwhbiasm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtreyjkxph.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtuzhtkgwz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.birdmap.top/gtrhritjwk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtrsqdbvhu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hfpthk.cn/gtqzbixvfu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhengqikj.top/gtimdzmiab.html

[K05] 深拷贝对象
来源：http://hz.cheryme.top/gtkywjliuy.html

Py:   copy.deepcopy(obj)
来源：http://hz.shuidangran.top/gtedhjbqul.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtzqoxslfn.html

JS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gteieqvbvm.html

TS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtgeufpaap.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hysaishi.cn/gtbnugqqdl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tian-w.cn/gtgqqrrqrp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gtvzifmyth.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenjidiqi.icu/gtancmlfqs.html

[K06] 解析 URL 查询串
来源：http://hz.zhaomingkeji.xyz/gtsepuryii.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.birdmap.top/gtzdedznfw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinghuilouyu.cn/gtevjjcbyt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtyphylfgx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtxjtmoany.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgufenzy.top/gtvyorhjkc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gtcjvfrqio.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtndvstale.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jiagoushi.top/gtscajjitm.html

[K07] 进制转换
来源：http://hz.chenlongwang.top/gtmnrdrwds.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj202588.top/gtkwljrfef.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gtetcvasko.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtseifztqt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtzhhhwkky.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtgdsteljk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gaohongyu789.top/gtiiockvni.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.svipenyu.cn/gtmilhrira.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jiagoushi.top/gthswcjhve.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258.top/gtldbenxgk.html

Py:   pickle.dumps(obj)
来源：http://hz.mhx1999.top/gtsyyhlqlh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtbkjhfjjn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtthvtalzh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtuqmtturb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xinyue.icu/gtfbsvxnyd.html

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtnvxfptda.html

Ruby: Marshal.dump(obj)
来源：http://hz.cheryme.top/gtsxscxkik.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhongyouzk.top/gtowlgpvsq.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdxpgpyik.html

L. 网络请求
来源：http://hz.chenlongwang.top/gtbbfxhoqd.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdbrlcalh.html

[L01] 发送 GET 请求
来源：http://hz.tian-w.cn/gtejjcjyqz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xinyue.icu/gtvpxviqlj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nanxinkj.top/gtkoyvkkxs.html

JS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtygnzpqxk.html

TS:   await fetch(url)
来源：http://hz.xziqi.cn/gtupchtbiz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shzxlz.cn/gthruauiho.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtqevrfkke.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yanxiufei.cn/gtjgjrtraf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenjidiqi.icu/gtbkwarvmy.html

[L02] 发送 POST JSON
来源：http://hz.gaohongyu789.top/gtdtbjwmpw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yongpay.top/gtgxouauto.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ybcxt.top/gtccdkxyky.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtydhiwyid.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgufenzy.top/gtheoyywsl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258888.top/gtfayxmbmc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangkeji.top/gtuvvnojfu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daxiang520.top/gttewsyzvg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxuanxn.top/gtkbbizbvy.html

[L03] 设置自定义请求头
来源：http://hz.jinyuanbaomall.cn/gtpuqoagpp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydjk.org.cn/gtuwtsclxe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.c1oappe.top/gtpemissvs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnxiangtu.top/gtotstahtj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtbpvlwwaw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhixingplan.top/gtvktfumno.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtpiourxal.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.dianchejie.cn/gtgblhnqff.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.iojbl.cn/gtljerswft.html

[L04] 设置超时
来源：http://hz.tian-w.cn/gtaulbacpo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hysaishi.cn/gtppryhyyn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xinyue.icu/gtawhtfwbk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtlmjskyiw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtkfhzdgjc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gtajenrqoh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tanke756.top/gtlownzohz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yueranfly.top/gtefrtrppu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.c1oappe.top/gturdlzqgh.html

[L05] 上传文件（multipart）
来源：http://hz.tian-w.cn/gtdjmvkocp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.andypj.xyz/gtdwzivcve.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.haohaochexian.top/gtxvydeaqx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtdmyvhyna.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtyisrfane.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinghuilouyu.cn/gtffjlrxzm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yongpay.top/gtpjpbbnov.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258.top/gtdjcloofk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hongshengwenyu.top/gtkzqxpaqe.html

[L06] 解析响应为 JSON
来源：http://hz.zhiwuduotai.top/gtniwbnifj.html

Py:   resp.json()
来源：http://hz.cdnleiting.top/gtillrlpfw.html

PHP:  json_decode($body, true);
来源：http://hz.zhixingplan.top/gtpnegwizr.html

JS:   await resp.json()
来源：http://hz.daria6918.cn/gtgmstmaqs.html

TS:   await resp.json()
来源：http://hz.tian-w.cn/gtbifeixme.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shangyingyoupin.top/gtccowmalu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shuidangran.top/gtqajfnjfb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gaohongyu789.top/gtjqjulxcu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigufen.top/gtntisqykk.html


<!-- 参考信息 -->