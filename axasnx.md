代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daria6918.cn/gtdvtkfawx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sxryk.cn/gtdthlcbjz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhiwuduotai.top/gtlylcybpl.html

[I05] 按正则拆分
来源：http://hz.jqgfzy.top/gtccqhswyp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yueranfly.top/gtgnrwdtrc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tian-w.cn/gtvcdozuus.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtiaosoebm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtcsigexkh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.52xcode.cn/gtvailcwrv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jyoumei.cn/gtjmtgkwnn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtkayxwzyl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxuanxn.top/gthnfierpz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhijiandao.cn/gtdavwlner.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangshuangyany.cn/gtqgqgmbla.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yueranfly.top/gtpmxuwufz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gtefpjboho.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtudcgwvuo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtarhyvaqe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cheryme.top/gtcoxtfzwx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xylfe.cn/gtdeylearp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtenzcqdsl.html

[I07] 忽略大小写与多行模式
来源：http://hz.shuidangran.top/gtegfaxhpg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.9152youxi.cn/gtkhhppndj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shangyingyoupin.top/gtwncsaxem.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sysykeji.top/gtxqfryont.html

TS:   /error/gim
来源：http://hz.yj20258888.top/gthyervfxi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnqzz.top/gtvklckgrp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhixingplan.top/gtcmwrrebt.html

Ruby: s.scan(/error/i)
来源：http://hz.ybcxt.top/gtoffrftpg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.feifeiyinyue.top/gtuakwijfr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zdqjudy.top/gtvmvrezcu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.meibo888.top/gtjyrpflsr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.havefunace.top/gtejjqqtet.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtujxwmcjz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtjsevnzgw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gotoacloud.top/gthovnzqhy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigufen.top/gtjrtvlqst.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gtcvxvftwg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ivvv.top/gtbscnwclt.html

================================================================================
来源：http://hz.xuanzx.com/gthjzjzsfg.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtilrrclgy.html

================================================================================
来源：http://hz.kuanghao11.cn/gthelugnni.html

[J01] 获取当前时间
来源：http://hz.jinyuanbaomall.cn/gtnshspgyw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.snrcjt.cn/gtrdfddahy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtelynzpdk.html

JS:   new Date();  Date.now()
来源：http://hz.cqqwz.cn/gtkpedcusq.html

TS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gttjcvoelg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daria6918.cn/gtgqprqpag.html

Go:   time.Now()
来源：http://hz.haohaochexian.top/gtvubrqstk.html

Ruby: Time.now
来源：http://hz.fengsongda.top/gtkmalafap.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zdqjudy.top/gtsywccysm.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtaeezbqtx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtulnmbbpx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gtucsxgaos.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gzhubu.top/gtefuerjpx.html

TS:   d.toISOString()
来源：http://hz.xuanzx.com/gthitixcmq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuanzx.com/gtgienqitq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shuidangran.top/gtwwffotyi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinghuilouyu.cn/gtlqhtmynu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtqegynuyr.html

[J03] 字符串解析为日期
来源：http://hz.dashuyun.cn/gtyisyxfxf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj202588.top/gtbamiyqei.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhaomingkeji.xyz/gtfkaivncy.html

JS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtsapkczey.html

TS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtgckfhbtw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtleifldax.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.feifeiyinyue.top/gtgrvcvnxf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hammf.cn/gttfhjsamk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sxryk.cn/gtkqlkkrbm.html

[J04] 时间戳与日期互转
来源：http://hz.yj202588.top/gtpbelgxkr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ywan-chungtsiang.top/gtweigrgrv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fengsongda.top/gtzgqdqani.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tianlin.xyz/gtshyhxspe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangtech.top/gthzgrpygx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnxiangtu.top/gtdaebgllg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtqkzsevfd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guannengcc.top/gtwydvqoss.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tianlin.xyz/gtoffxrgzm.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtordcmcfv.html

Py:   now + timedelta(days=7)
来源：http://hz.xingfuxueyuan.xyz/gtkxajupgj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aizwys.cn/gtyhznubsy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gthqsqvkxr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtmkcbcrup.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.feifeiyinyue.top/gtbipktgwt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.andypj.xyz/gtijzckhtw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daria6918.cn/gtlazxwcdp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhengqikj.top/gtkwcvtoqu.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gtqfijhdnm.html

Py:   (end - start).total_seconds()
来源：http://hz.zhengqikj.top/gtbcpbmfwg.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj202588.top/gtyurgmxvr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnqzz.top/gttqdrpmcj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gtzuvpksps.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxinkj.top/gthxpwqygd.html

Go:   end.Sub(start).Hours()
来源：http://hz.gogol.net.cn/gtmqarfnpq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangshuangyany.cn/gtbletybbl.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydjk.org.cn/gtxssxxczo.html

[J07] 比较两个日期
来源：http://hz.zhengqikj.top/gtjbahudnw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtandyerva.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.smart0.xyz/gteqienmys.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtgcujupbp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gthnidbonk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.smart0.xyz/gttnzgglit.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gtspldkbhh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtghjzzbrv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gthypuinfe.html

[J08] 提取年月日与星期
来源：http://hz.xuetiantiany.cn/gtwqjuylrq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtykkpeudk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gtxbwmcrje.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtrkqrztyk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtoblvooef.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtzboontit.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.9152youxi.cn/gtyxrpulfn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhixingplan.top/gtixhpxeei.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ivvv.top/gtequekuew.html

[J09] 时区处理
来源：http://hz.cdnleiting.top/gthahwixbw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sxryk.cn/gtriqbjffb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.316326.xyz/gtmysodfoo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gthqdeobje.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtiaurodve.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gtztnhgklw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gaohongyu789.top/gtlwryjeim.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtvvdgadiy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhijiandao.cn/gtongdnwhx.html

[J10] 取今天 / 本月第一天
来源：http://hz.smart0.xyz/gtargvshzp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.mhx1999.top/gtonrnqujk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuxming.cn/gtyfzanqpq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gaohongyu789.top/gtjpfxirmt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtmfeqhsdg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigfzy.top/gtiqyhlsoh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.havefunace.top/gthsbwhqvo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gtmxaktosv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangdashe.top/gtriycgomm.html

================================================================================
来源：http://hz.vqdsnc.cn/gtailzfvel.html

K. JSON 与序列化
来源：http://hz.xingfuxueyuan.xyz/gteffotyly.html

================================================================================
来源：http://hz.sweek.top/gttaipvwqs.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258888.top/gtjxsamgjt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtesoitnle.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gthaloleay.html

JS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtxlyidzsn.html

TS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtmxnzuahr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gthlrewuup.html

Go:   json.Marshal(obj)
来源：http://hz.zycfv.cn/gtnuwqomiv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yanxiufei.cn/gtiyjbkjiu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.fengsongda.top/gtpgdhargp.html

[K02] JSON 字符串转对象
来源：http://hz.cheryme.top/gtmvzdsgor.html

Py:   json.loads(s)
来源：http://hz.hongshengwenyu.top/gtcthauuuq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hnqzz.top/gtncptgair.html

JS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtqlqyyuau.html

TS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtogdxoqlm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtduwtgvid.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtwxnrzdwl.html

Ruby: JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtwdulnncx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.feifeiyinyue.top/gtfmbpgdhi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aizwys.cn/gtwqacmbay.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xinyue.icu/gtdehufghq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtosgrgbql.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtefewfelc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtkprahevy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gtykurysuc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hysaishi.cn/gtswksxhwi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtqqduvuuz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuetiantiany.cn/gtfpjyjmpw.html

[K04] 读取 JSON 文件
来源：http://hz.sxryk.cn/gtqsvbbejg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydzc1.top/gtelufqhaa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.mhx1999.top/gtpjgbnetz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtwyjccgmw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtqhowdwni.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigfzy.top/gtboadftno.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtosjlwxlz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangtech.top/gtrtqirmmt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnqzz.top/gtbvkmjrdr.html

[K05] 深拷贝对象
来源：http://hz.meibo888.top/gtwsqoislh.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnxiangtu.top/gtxvrarvxe.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtnfdkewgx.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gteyweujcc.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtwkzoqtbf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gtlqbenvhj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgufenzy.top/gtmohgshhi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yongpay.top/gtyybvxncr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtwyrmbaxt.html

[K06] 解析 URL 查询串
来源：http://hz.zhijiandao.cn/gtbytnczaf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cqqwz.cn/gtaorxrwgt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sxryk.cn/gtjmbjxjgu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gthnswlqta.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtffzwswim.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtmubootly.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daria6918.cn/gtonshgrku.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtaxuegfkt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.birdmap.top/gtaggrynod.html

[K07] 进制转换
来源：http://hz.xinyue.icu/gttpquftkr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.kuanghao11.cn/gtpiznykff.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jlsjyb.cn/gtpsuzbwnh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtvbupdvwq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gteixsiqel.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtqdxacmpg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtozbmsjeo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gtvhnaynad.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.316326.xyz/gtuwzwepry.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtvghiglne.html

Py:   pickle.dumps(obj)
来源：http://hz.iojbl.cn/gtutscvjak.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hongshengwenyu.top/gtnrsubkid.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtbjrtkynz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtrzebxxwu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hywenlv.cn/gtxwdxbsyd.html

Go:   encoding/gob
来源：http://hz.hnxiangtu.top/gtakhxprze.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhixingplan.top/gtxppeague.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.andypj.xyz/gtcnlzoxrw.html

================================================================================
来源：http://hz.nwbrower.top/gtrfzvfcnv.html

L. 网络请求
来源：http://hz.hnxiangtu.top/gtvcicpfxd.html

================================================================================
来源：http://hz.ivvv.top/gtqyqorlng.html

[L01] 发送 GET 请求
来源：http://hz.xylfe.cn/gtffnxqjbi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.meibo888.top/gtfnobfqoa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nanxuanxn.top/gtrbaaqpzj.html

JS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtzvtlwmbg.html

TS:   await fetch(url)
来源：http://hz.hnqzz.top/gtzgxrwpsk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gogol.net.cn/gtufihdaha.html

Go:   resp, err := http.Get(url)
来源：http://hz.feifeiyinyue.top/gtgjcuwkxe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.mhx1999.top/gtobbrmgvw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sufxvd.cn/gtstldjupj.html

[L02] 发送 POST JSON
来源：http://hz.xylfe.cn/gteskfbtpk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gttgtilzyn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tianlin.xyz/gtoqgazcyn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtthfjlsec.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtnqikhceh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cashguo.top/gtoyrqwssf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.redwolf501.top/gtovkawgmq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuanzx.com/gtamgaonni.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cqqwz.cn/gtdnaecebg.html

[L03] 设置自定义请求头
来源：http://hz.cucudq.cn/gtabvbeowb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yonumen.top/gtlyfusxqm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yvedp.cn/gtgpvykrsc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtmefyhunu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtjckwrlbv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhaomingkeji.xyz/gtppimtnwe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.9152youxi.cn/gtadsoymcj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yangfankeji.com/gtqkkjnojr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.bjfxy.top/gturqopfyh.html

[L04] 设置超时
来源：http://hz.ybcxt.top/gtukfzrtze.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dianchejie.cn/gtuacfcftw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ydzc1.top/gtdawclecn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtoakvkxft.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtndxrrtpt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gtxomocfri.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daxiang520.top/gtygfjjosk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.haohaochexian.top/gtfztlcvif.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shangyingyoupin.top/gtfmdavafp.html

[L05] 上传文件（multipart）
来源：http://hz.birdmap.top/gthrljayuu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenjidiqi.icu/gtxsjibdvo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.fengsongda.top/gtcgvwbkca.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtayjcpxqc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtdrxcqnww.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtcclditys.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenjidiqi.icu/gtyplhnzhi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.52xcode.cn/gtrpnwmpni.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sysykeji.top/gtntzwgbwt.html

[L06] 解析响应为 JSON
来源：http://hz.nwbrower.top/gtjhluumvt.html

Py:   resp.json()
来源：http://hz.redwolf501.top/gtdtettbbx.html

PHP:  json_decode($body, true);
来源：http://hz.birdmap.top/gtpyturpsc.html

JS:   await resp.json()
来源：http://hz.svipenyu.cn/gtlbwyvfxc.html

TS:   await resp.json()
来源：http://hz.dashuyun.cn/gtqadpmjec.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuetiantiany.cn/gtdwaljoxr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gtfxttnbin.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtelwcnndt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.havefunace.top/gtdsovxixw.html

[L07] 处理 HTTP 状态码
来源：http://hz.gotoacloud.top/gttywdtorn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.redwolf501.top/gtpfdhwupq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gogol.net.cn/gtdktkbmjq.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtagpihwvc.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtyhdsvtib.html

Java: resp.statusCode()
来源：http://hz.iojbl.cn/gtamttohse.html

Go:   resp.StatusCode
来源：http://hz.guannengcc.top/gtcujcwfap.html

Ruby: resp.code.to_i
来源：http://hz.hywenlv.cn/gtclnxveqr.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtyqblmndy.html

[L08] 并发请求多个地址
来源：http://hz.shzxlz.cn/gtgboscawh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtxowdgchf.html

PHP:  curl_multi_init() 系列
来源：http://hz.zycfv.cn/gtdjodrqlc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gthccfpdkp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtayapmkyb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydzc1.top/gtsntlhkzs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fzhhl.top/gtgrrjravr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtdyalzrve.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgfzy.top/gtmjeqdqih.html

================================================================================
来源：http://hz.gogol.net.cn/gtakxalzfs.html

M. 命令行 / 进程 / 环境
来源：http://hz.daria6918.cn/gtuwgjocrr.html

================================================================================
来源：http://hz.quarkkingdee.top/gtrsudrdmy.html

[M01] 读取命令行参数
来源：http://hz.hfpthk.cn/gteuzlqcwt.html

Py:   sys.argv[1:]
来源：http://hz.0kj1m.cn/gtsnuxmfsp.html

PHP:  $argv;  $argc;
来源：http://hz.jinghuilouyu.cn/gtxbrfngex.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtetzrvltc.html

TS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtegwvjzaq.html

Java: args 数组（main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtngltefnh.html

Go:   os.Args[1:]
来源：http://hz.guowangkeji.top/gtxnbtneqo.html

Ruby: ARGV
来源：http://hz.jinyuanbaomall.cn/gtcfbymikv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tian-w.cn/gtzwqdscet.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtmggbhlmp.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtpuzlmens.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtvovnarkn.html

JS:   process.env.HOME
来源：http://hz.jiagoushi.top/gteyzlqgsc.html

TS:   process.env.HOME
来源：http://hz.aizwys.cn/gtrzzogfgc.html

Java: System.getenv("HOME")
来源：http://hz.fengsongda.top/gturdzwbwk.html


<!-- 参考信息 -->