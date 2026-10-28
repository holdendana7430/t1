代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jyoumei.cn/gtgzhjpenz.html

[I03] 提取捕获分组
来源：http://hz.shangyingyoupin.top/gtgxtijlee.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shuidangran.top/gtcvuywquc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hongshengwenyu.top/gtnamjdfuv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhoulong.xyz/gtwnolhyaa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jiagoushi.top/gtrakrqtwd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.snrcjt.cn/gtdrrhqbrt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cheryme.top/gttvwcvspc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.havefunace.top/gtaywfswsj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenlongwang.top/gtgpccraje.html

[I04] 正则替换
来源：http://hz.yvedp.cn/gtzieeegii.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yangfankeji.com/gtowfbwrsr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtpmyzkzyf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtlohbrafy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtbxhgwxvb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.mhx1999.top/gtvswuvfex.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangkeji.top/gtzifuohee.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhongyouzk.top/gtgrxiqtbn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ehwqpu.com/gtetjvsjjs.html

[I05] 按正则拆分
来源：http://hz.ppjwa.cn/gtvbaljqep.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ivvv.top/gtaezosmln.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shangyingyoupin.top/gtbkskxbmd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gthjobcova.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtqyoehmsr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gtvumfyukj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.9152youxi.cn/gttaxkxeij.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtrtpjvsnt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gtmkqfukxl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtokzqseqk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtbqneuzdx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tanke756.top/gtsmhedkyb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtmwondceg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtupqyuqcz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhijiandao.cn/gtygkilcce.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nwbrower.top/gtbquocybz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hongshengwenyu.top/gtijrjlwlp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zdqjudy.top/gtjsrmmzjp.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gtvbaihzif.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yvedp.cn/gtvypdvosi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj202588.top/gtdbyrkqyd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gtljaqwedk.html

TS:   /error/gim
来源：http://hz.yj202588.top/gtmpovujnm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.52xcode.cn/gtltgmcfae.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhixingplan.top/gtoeocqdey.html

Ruby: s.scan(/error/i)
来源：http://hz.hfpthk.cn/gtfsjxedpr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xziqi.cn/gtzjxowvuk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigfzy.top/gtbydxwnig.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhiwuduotai.top/gtbvytuhbk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.dashuyun.cn/gtbcwyqztc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.redwolf501.top/gtmpyfsobl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtfzpqqaui.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.bjfxy.top/gtwpfmryaw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hysaishi.cn/gttavxgxgr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cucudq.cn/gtbbfbwlho.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yvedp.cn/gtyelixqlx.html

================================================================================
来源：http://hz.yangfankeji.com/gttscfpgln.html

J. 日期与时间
来源：http://hz.ydjk.org.cn/gtnbtgnxjq.html

================================================================================
来源：http://hz.yuxming.cn/gtqdnahejj.html

[J01] 获取当前时间
来源：http://hz.aizwys.cn/gtutybrdjs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zdqjudy.top/gtenmorbpa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtwfhjiuyk.html

JS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gtcirpthsc.html

TS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtgnkfbmnk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fzhhl.top/gtcvvahsir.html

Go:   time.Now()
来源：http://hz.ydzc1.top/gtscnrlckt.html

Ruby: Time.now
来源：http://hz.jqgufenzy.top/gtiuiytrvc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinghuilouyu.cn/gtzrupflzz.html

[J02] 格式化输出
来源：http://hz.redwolf501.top/gtjncnypmz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.birdmap.top/gtrolxnzdn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gttoglaagg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.snrcjt.cn/gttoovplmn.html

TS:   d.toISOString()
来源：http://hz.316326.xyz/gtbgcyowgx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.snrcjt.cn/gttjypcfua.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhiwuduotai.top/gtgpsrwwjq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtciyorndz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cashguo.top/gtmyzluecq.html

[J03] 字符串解析为日期
来源：http://hz.tianlin.xyz/gtjgsvfuwo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnxiangtu.top/gttvaabola.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.guannengcc.top/gtzoloeild.html

JS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gtwmcrrxzc.html

TS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtioiuwwdb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258.top/gtbcznanws.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cucudq.cn/gtadubrrpj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xinyue.icu/gttjzymtst.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jiagoushi.top/gtxoinvvdu.html

[J04] 时间戳与日期互转
来源：http://hz.smart0.xyz/gtvluvqscj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.snrcjt.cn/gtrrhyuggg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydzc1.top/gtiqzsbfzg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ybcxt.top/gtwmxmwcpc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xingfuxueyuan.xyz/gtxujmlfxw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtnolfjlkc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jiagoushi.top/gtiabumlzq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cucudq.cn/gtqwukrtfm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gtpzvzwcaq.html

[J05] 时间加减（加 7 天）
来源：http://hz.52xcode.cn/gtikaumbrv.html

Py:   now + timedelta(days=7)
来源：http://hz.gaohongyu789.top/gtomprwxpa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.mhx1999.top/gtawibrluf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtybaimceh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtdjroksbe.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yonumen.top/gtrdkirlpv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinghuilouyu.cn/gthybofxyo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gotoacloud.top/gtigwxfqdj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sweek.top/gtggioutti.html

[J06] 计算两时间之差
来源：http://hz.dianchejie.cn/gtnwtakivt.html

Py:   (end - start).total_seconds()
来源：http://hz.birdmap.top/gtazkxfvdg.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gtjbhjcbaq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.havefunace.top/gtndntligt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhixingplan.top/gtxklbbmlb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.havefunace.top/gtczkfxaxy.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtxwdtmcqb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhiwuduotai.top/gthjpeszbv.html

C#:   (end - start).TotalSeconds
来源：http://hz.0kj1m.cn/gtyyprykow.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtwghtflyh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gttmcmtvlv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ppjwa.cn/gtkyrkwjwr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gthoptcwse.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cashguo.top/gtwbdwjerl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.9152youxi.cn/gtfbbonkyz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xuetiantiany.cn/gticovqbay.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtgycvnpjv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtkmgdxasa.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtxsggjkhf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangdashe.top/gtnxtvwoei.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgufenzy.top/gtuuvkezmt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jiagoushi.top/gtigmoeswt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gzhubu.top/gthhbcwhyn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yongpay.top/gtbwnancmk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xinyue.icu/gteovqxosm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtfakfjogy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sufxvd.cn/gttjrriofr.html

[J09] 时区处理
来源：http://hz.dianchejie.cn/gthgyoibfd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.andypj.xyz/gtmxcrrqqj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.meibo888.top/gtccgqaumj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jianghu66.top/gtieeczqyp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cdnleiting.top/gtbemgfrzs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cqqwz.cn/gtejntjotc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.meibo888.top/gtljuvajfd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhaomingkeji.xyz/gtkbljvwsn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gtnllozrzw.html

[J10] 取今天 / 本月第一天
来源：http://hz.iojbl.cn/gtxzewcbvz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gtatppstps.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnxiangtu.top/gtduasuorj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuxming.cn/gtlgnjqdct.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhijiandao.cn/gthpjctpgy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtnwygwojw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jiagoushi.top/gthufsfbeg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gtteohrgjo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gaohongyu789.top/gtusqacvsq.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtncnwklsr.html

K. JSON 与序列化
来源：http://hz.jinyuanbaomall.cn/gtndootocu.html

================================================================================
来源：http://hz.xuanzx.com/gtoqstwcwm.html

[K01] 对象转 JSON 字符串
来源：http://hz.cashguo.top/gtjwzxvfqq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtpzfbblhu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gttmmjltbm.html

JS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtyzukglsx.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtnguoakbb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xinyue.icu/gtridfshob.html

Go:   json.Marshal(obj)
来源：http://hz.zhixingplan.top/gtihisgmmt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gtypyclhej.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258.top/gttlgbdyim.html

[K02] JSON 字符串转对象
来源：http://hz.zdqjudy.top/gtgjkecebp.html

Py:   json.loads(s)
来源：http://hz.c1oappe.top/gtjdvrxivv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhijiandao.cn/gtyccohbjq.html

JS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtlknttdjk.html

TS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtkusjdcvr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xinyue.icu/gtlorgsjap.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtvdihqhzw.html

Ruby: JSON.parse(s)
来源：http://hz.redwolf501.top/gthsgyxxfn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.iojbl.cn/gttgbxzfzm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hfpthk.cn/gtiunavtio.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pengpengdd.cyou/gtmtiuputg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtdbpzpdmw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daxiang520.top/gtbkkpcgdq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtdxayathn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtbgkgivtb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tanke756.top/gtwtbclthm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhaomingkeji.xyz/gtgttxqhdk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xylfe.cn/gtcrrzrtiy.html

[K04] 读取 JSON 文件
来源：http://hz.jyoumei.cn/gtsmzyzbnt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.feifeiyinyue.top/gtegqelklj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtsmmrwdrl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gtvubrkooj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtgmgnpqpt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenzaomai.com/gtvgqjyzdw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtxivhdbuo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gttuypxfmh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hfpthk.cn/gterqholkv.html

[K05] 深拷贝对象
来源：http://hz.bjfxy.top/gtmuedhpdd.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gtituvtpnw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.smart0.xyz/gtyjnnbavp.html

JS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtxryooqsw.html

TS:   structuredClone(obj)
来源：http://hz.pycfn.com/gtnvtrzvqn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.andypj.xyz/gtohnxsvwg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ppjwa.cn/gtygadihbv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtmttdvysg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangdashe.top/gtgjzaunnb.html

[K06] 解析 URL 查询串
来源：http://hz.zycfv.cn/gtpzecvshi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shangyingyoupin.top/gtrkowzlki.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydjk.org.cn/gtykjiifrl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtvagqaabw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtrrmiotuz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.pycfn.com/gtvmoywccf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tianlin.xyz/gthfcstsxm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtsxezpemo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yangfankeji.com/gtpipoxzok.html

[K07] 进制转换
来源：http://hz.pycfn.com/gtjjnzwiri.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhijiandao.cn/gtfnrkzxli.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtmqyanrek.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtyflceryf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtmpoklwby.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtcmujljic.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shzxlz.cn/gtxafzbwpv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuxming.cn/gtrdgcbftx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.wangdashe.top/gtdrkhggfc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yonumen.top/gtalsprttl.html

Py:   pickle.dumps(obj)
来源：http://hz.jqgufenzy.top/gthrhmsila.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gtdzqqgxpj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gttsnularb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gttlhhfugo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tianlin.xyz/gteptfaftl.html

Go:   encoding/gob
来源：http://hz.yuanzhike.top/gttdfxvhpu.html

Ruby: Marshal.dump(obj)
来源：http://hz.ppjwa.cn/gtmewkrffl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangshuangyany.cn/gtdezxtrfm.html

================================================================================
来源：http://hz.jinqigfzy.top/gtrzgpjpri.html

L. 网络请求
来源：http://hz.sysykeji.top/gttfuulteg.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtvtiswpyu.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gtmcfagehl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gtamaoutpo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.snrcjt.cn/gtmhuvqmbt.html

JS:   await fetch(url)
来源：http://hz.cheryme.top/gthdiikspy.html

TS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gtnuzntfxu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daxiang520.top/gthncqcwzr.html

Go:   resp, err := http.Get(url)
来源：http://hz.haohaochexian.top/gtirzcmyvh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shangyingyoupin.top/gtgzahiddd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtnsxzssrl.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gtumwrbffv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigfzy.top/gtfmxpnbow.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gtchcfczts.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtyqghcrmw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtfvpvkcgm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangdashe.top/gtvpeyqpjy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gaohongyu789.top/gtnheqhpdt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhiwuduotai.top/gtnfskeldq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guowangkeji.top/gtmzkfgaqp.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtghqkumpq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuetiantiany.cn/gtqvtelosu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cdnleiting.top/gtivfczitn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtzpjwkemu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydzc1.top/gtiepsvnta.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shuidangran.top/gthrqqbmda.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtmpuzxpge.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aibaodan.cn/gtqgcakjst.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtfyxltfak.html

[L04] 设置超时
来源：http://hz.sweek.top/gtzcwglcwr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.meibo888.top/gtuamvaykm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ivvv.top/gtynrjemmb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtsfjcusss.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtshmtuklf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cqqwz.cn/gtshbjfyil.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhaomingkeji.xyz/gtvavedgks.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cheryme.top/gtjlnypmsi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jianghu66.top/gtlfqhwclh.html

[L05] 上传文件（multipart）
来源：http://hz.smart0.xyz/gtqaobzdeb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guowangkeji.top/gtsozfsfvk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.mhx1999.top/gthktvjhcv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtobpajmqd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigufen.top/gtaehgfigx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj202588.top/gtwrohaxal.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tian-w.cn/gtshvcvdue.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cheryme.top/gtalfybijq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cucudq.cn/gtyhxdfhlv.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258.top/gtouhhmpcy.html

Py:   resp.json()
来源：http://hz.tian-w.cn/gthedjqcyg.html

PHP:  json_decode($body, true);
来源：http://hz.sxryk.cn/gttkwueoxo.html

JS:   await resp.json()
来源：http://hz.fzhhl.top/gtxydsuhti.html

TS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtqjvusrbu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.svipenyu.cn/gtiasthifh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guowangkeji.top/gthqsdleaj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xylfe.cn/gtiqflhdzn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pengpengdd.cyou/gtkwbqodcw.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj202588.top/gtkokcdjgw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuetiantiany.cn/gtmjqthetf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuanzx.com/gtczfashcb.html

JS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtpvyxpgwl.html

TS:   resp.ok;  resp.status
来源：http://hz.ywan-chungtsiang.top/gtvsnjkgtz.html

Java: resp.statusCode()
来源：http://hz.zhijiandao.cn/gtxqvczrqn.html

Go:   resp.StatusCode
来源：http://hz.yj202588.top/gtdoyfcaiv.html

Ruby: resp.code.to_i
来源：http://hz.9152youxi.cn/gtlbwkartq.html

C#:   (int)resp.StatusCode
来源：http://hz.tanke756.top/gtalerpkoz.html

[L08] 并发请求多个地址
来源：http://hz.daxiang520.top/gtwudcliey.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.fengsongda.top/gtnmmtzeli.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gttanjqwns.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtazormmxa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gtylqcvwkx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.52xcode.cn/gtezhmgxlf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtzmnpdpkp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.birdmap.top/gtgufoquby.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gtqnjufhmx.html

================================================================================
来源：http://hz.aizwys.cn/gtdpsnfcpw.html

M. 命令行 / 进程 / 环境
来源：http://hz.ivvv.top/gtjddacfjv.html


<!-- 参考信息 -->