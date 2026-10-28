代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangdashe.top/gtcclwtczx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.kuanghao11.cn/gtmjddzcqh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cashguo.top/gtuswpwxpn.html

[I05] 按正则拆分
来源：http://hz.yuxming.cn/gtmraysmtq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gtcdxxofox.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gotoacloud.top/gttkmchyci.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtccxponbg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtzismolau.html

Java: s.split("\\s*,\\s*")
来源：http://hz.andypj.xyz/gtvuzbqqjd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtnmsweglq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtxbtucncv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pengpengdd.cyou/gtwlsnuuor.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guannengcc.top/gtqhrrqnli.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtrffmwuqp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ehwqpu.com/gteremxpgh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtpigfdapk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtiwqseqsu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yvedp.cn/gtqkusxupj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.kuanghao11.cn/gtzzzeupgx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhongyouzk.top/gtnugxiaem.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtdheatfhu.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtkhcymvrv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gogol.net.cn/gtdbalsxqb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gteokumpuo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.kuanghao11.cn/gtfbbymjit.html

TS:   /error/gim
来源：http://hz.shuidangran.top/gtervcdfnj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtmkwrwgjy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.guowangkeji.top/gtguvnziac.html

Ruby: s.scan(/error/i)
来源：http://hz.zhixingplan.top/gtvncmqxhh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.316326.xyz/gtaltpzdbi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yongpay.top/gtqsmaaepk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhengqikj.top/gtscdywuad.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydzc1.top/gtpxgavywe.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gtxdrdfycc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtnupkxjmm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gttbdxefqm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.9152youxi.cn/gtylkwrxbh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xinyue.icu/gtgkwgvlpr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtnvgorqnb.html

================================================================================
来源：http://hz.chenlongwang.top/gtpasagvsr.html

J. 日期与时间
来源：http://hz.yvedp.cn/gtbwsrsazd.html

================================================================================
来源：http://hz.xziqi.cn/gtulymellk.html

[J01] 获取当前时间
来源：http://hz.yuanzhike.top/gtybnhxsia.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxinkj.top/gtklbdtkrl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gttkigawnd.html

JS:   new Date();  Date.now()
来源：http://hz.zhijiandao.cn/gtfrnczvev.html

TS:   new Date();  Date.now()
来源：http://hz.mhx1999.top/gtguqpgvma.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.kuanghao11.cn/gtpmqoclyk.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtxdinjrdh.html

Ruby: Time.now
来源：http://hz.sweek.top/gtzspnmcso.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuanzhike.top/gtkfwxkklf.html

[J02] 格式化输出
来源：http://hz.ehwqpu.com/gtyfgwikcn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtbsxvcmak.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gthgwznpwt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sweek.top/gtabkcotjy.html

TS:   d.toISOString()
来源：http://hz.zhijiandao.cn/gtlacpsnqy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangdashe.top/gtufjunjar.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtflynuxku.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtyncistbt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gogol.net.cn/gtzylwcaud.html

[J03] 字符串解析为日期
来源：http://hz.zhixingplan.top/gttexrbklo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenzaomai.com/gtehrfghxx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.havefunace.top/gtpabsjypo.html

JS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtqyqyxzai.html

TS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gtwrtmpbeb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtxyiipcfx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenjidiqi.icu/gtdedthiuv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gtmxjlpnuh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigfzy.top/gtgdikadnd.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gtnuywxinc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yonumen.top/gtjhjxgkbe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hywenlv.cn/gtorjnwnae.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtiwmgnpqh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zycfv.cn/gtgmguthjh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guowangkeji.top/gtkkiuwwdq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cucudq.cn/gtixujykny.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.birdmap.top/gtjwxrphnk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuanzx.com/gtorjsbhbo.html

[J05] 时间加减（加 7 天）
来源：http://hz.gaohongyu789.top/gtylhaplue.html

Py:   now + timedelta(days=7)
来源：http://hz.tianlin.xyz/gtsdseorxa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtkzmwzrhz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtyayxeghz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gthyxahbqv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.0kj1m.cn/gtvoryjzzn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.9152youxi.cn/gtfyfqwhfg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangdashe.top/gtnipoxxji.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258.top/gtlmmmjfkj.html

[J06] 计算两时间之差
来源：http://hz.jlsjyb.cn/gtuakqxdjb.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtqlxbnbob.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtduocpkpq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.birdmap.top/gthbbvgjdt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.9152youxi.cn/gtjsvlkadu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigufen.top/gtlehcehme.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangshuangyany.cn/gtesqpqdkj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gotoacloud.top/gtdxbksyxx.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtxwztzjie.html

[J07] 比较两个日期
来源：http://hz.zhiwuduotai.top/gtovygyxsl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtezffsxlc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhengqikj.top/gtcmkymubh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtwsvoanev.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtfwccjnzv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.0kj1m.cn/gtschsyjoo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtwjcqoeth.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtdfjhwocp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtiotkmkrj.html

[J08] 提取年月日与星期
来源：http://hz.zycfv.cn/gtmugswdny.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tian-w.cn/gtvgkaczyb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhengqikj.top/gtoapsqxyp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydzc1.top/gtxuqvrnji.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.birdmap.top/gtyllhkzor.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gtnsvbxied.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtvhzodvus.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.vqdsnc.cn/gthodewiwq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sweek.top/gthjadmzof.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtamciihnd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuanzx.com/gtxypdnxzs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guannengcc.top/gtyghknpng.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtggmtdsyy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtwgmvkeyf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gteqohhsnk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtakvttcnv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.vqdsnc.cn/gtdrmhwocr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnqzz.top/gttuvavaip.html

[J10] 取今天 / 本月第一天
来源：http://hz.guannengcc.top/gtxszdoroj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aizwys.cn/gtzdyarptp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ywan-chungtsiang.top/gtkyboevet.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yonumen.top/gtvepsbxkf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tanke756.top/gtcixqbbsj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtwpcesdyr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cdnleiting.top/gtqztzlejh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtdxxemrih.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuetiantiany.cn/gtazkmejua.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdfqucvba.html

K. JSON 与序列化
来源：http://hz.jinyuanbaomall.cn/gtsdfxhplu.html

================================================================================
来源：http://hz.gzhubu.top/gtknywaeda.html

[K01] 对象转 JSON 字符串
来源：http://hz.fengsongda.top/gtntrvxqyf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtzayhiecx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtzrzkozoz.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gttfldnbhf.html

TS:   JSON.stringify(obj)
来源：http://hz.birdmap.top/gtqtinnqal.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ydjk.org.cn/gtwsljizto.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtwdkeziim.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yanxiufei.cn/gtrfieisjh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuetiantiany.cn/gtgcgiaudw.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtetkozbtg.html

Py:   json.loads(s)
来源：http://hz.shzxlz.cn/gtcjgtpati.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuxming.cn/gtvfvlarys.html

JS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtzepsqpfr.html

TS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtswdhoztp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.haohaochexian.top/gtviefqibi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtyscoqrus.html

Ruby: JSON.parse(s)
来源：http://hz.ydzc1.top/gthjjrwfha.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gtdcuctvzt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhaomingkeji.xyz/gtuwlxkexf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ivvv.top/gtcucpcqzm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtaznlpxtk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtcwqkyhvj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtpzacnenw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sysykeji.top/gtzbjtvlpt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj202588.top/gtmwhayavq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhongyouzk.top/gtmklkfzym.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daxiang520.top/gtjqprhnai.html

[K04] 读取 JSON 文件
来源：http://hz.gogol.net.cn/gttdjjruis.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yueranfly.top/gtibsvtcau.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenlongwang.top/gtwjmhasrn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gtovpixfhx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtttopcpts.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fengsongda.top/gtmrrdnljm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtfyasaewb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hywenlv.cn/gtmogwcbsd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xylfe.cn/gtjgqaanbz.html

[K05] 深拷贝对象
来源：http://hz.ehwqpu.com/gtigjtjncq.html

Py:   copy.deepcopy(obj)
来源：http://hz.svipenyu.cn/gthgnggzks.html

PHP:  unserialize(serialize($obj));
来源：http://hz.dashuyun.cn/gtgxrqlosv.html

JS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtucjpcujy.html

TS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtdkikaypy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gtxqliqdxt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxuanxn.top/gtoojeshqv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.wangshuangyany.cn/gtbytklvgj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtefjcgwlr.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gtvhfhpyhs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gtrfwrhaid.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydzc1.top/gtvlzdoqky.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtkvhinfcg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gteqhyfexs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.52xcode.cn/gtdphthqti.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ppjwa.cn/gthdtpiryy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtcqnydrfa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtecdsrofw.html

[K07] 进制转换
来源：http://hz.zhoulong.xyz/gtguchylan.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xylfe.cn/gtjrevgyla.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shuidangran.top/gtsjngxmwb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gtjruizchf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtrkxrcghe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtlzviqsoz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuanzhike.top/gttcisbdal.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenzaomai.com/gtuuvusgnp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuxming.cn/gtjdidflxk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuxming.cn/gtucwpepwq.html

Py:   pickle.dumps(obj)
来源：http://hz.zhengqikj.top/gtkujqeani.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guowangkeji.top/gtfamhhplt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtojvwfiob.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtiiexjmmk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xuetiantiany.cn/gtkitzqpyu.html

Go:   encoding/gob
来源：http://hz.cheryme.top/gtalsrfrps.html

Ruby: Marshal.dump(obj)
来源：http://hz.dianchejie.cn/gttkdjanyf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hysaishi.cn/gtzkkhdgoy.html

================================================================================
来源：http://hz.fzhhl.top/gtrvqmdxhw.html

L. 网络请求
来源：http://hz.ywan-chungtsiang.top/gtvbnemhdb.html

================================================================================
来源：http://hz.fengsongda.top/gtevztrlmg.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtszbqvtig.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zdqjudy.top/gtkwxmfykj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tian-w.cn/gtbwundetr.html

JS:   await fetch(url)
来源：http://hz.fzhhl.top/gtulnlpfoq.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gtkxlutffi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.kuanghao11.cn/gtubjkfyeh.html

Go:   resp, err := http.Get(url)
来源：http://hz.xingfuxueyuan.xyz/gtyvmghmvr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shzxlz.cn/gtzvzeaznf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daxiang520.top/gtfkuwosxk.html

[L02] 发送 POST JSON
来源：http://hz.zycfv.cn/gtlslgkzrs.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangshuangyany.cn/gtuwmkrzzm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jianghu66.top/gtqsdlhfph.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtatcixdit.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtghhzzfcz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtpvpzsrnx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jyoumei.cn/gtexnnfuam.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gthwcjplmp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtabjpnoxh.html

[L03] 设置自定义请求头
来源：http://hz.hnqzz.top/gtumvceuoo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtoixxgrwg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinyuanbaomall.cn/gtocjkbbkb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gttmyzujsk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtwnqddaqn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zdqjudy.top/gtsyafkyod.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yongpay.top/gtmiksutss.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhengqikj.top/gtyxgeqhes.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zycfv.cn/gtbmotmlom.html

[L04] 设置超时
来源：http://hz.cashguo.top/gtmbujfqjb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinyuanbaomall.cn/gtlpzvnrid.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gogol.net.cn/gtzmtigimf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtlvqmxono.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtdcbylreh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sufxvd.cn/gtombgxvmz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zdqjudy.top/gtzilckyfq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sufxvd.cn/gtectyspwy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.feifeiyinyue.top/gtalcaiawg.html

[L05] 上传文件（multipart）
来源：http://hz.yuanzhike.top/gtbrpkztkv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtcwefndgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xingfuxueyuan.xyz/gtnicrpcvk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtyrncirhw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtnbbyunwl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cucudq.cn/gtptnutfpq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigufen.top/gtrwadzpbe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gaohongyu789.top/gtikpmocdb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinghuilouyu.cn/gtgtznacep.html

[L06] 解析响应为 JSON
来源：http://hz.nanxinkj.top/gtpmuxtzoi.html

Py:   resp.json()
来源：http://hz.jinqigufen.top/gtxzgrnrum.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtbmjzalcx.html

JS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtjvtpakqf.html

TS:   await resp.json()
来源：http://hz.ydjk.org.cn/gthythroit.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zycfv.cn/gtcjlspdgo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtkwozdhof.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xuetiantiany.cn/gtfblglyyo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtufznwnas.html

[L07] 处理 HTTP 状态码
来源：http://hz.dashuyun.cn/gtrnsftlob.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhiwuduotai.top/gtdbhnnzju.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gtvlwollmn.html

JS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtvmjimpqm.html

TS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gtfhuyledn.html

Java: resp.statusCode()
来源：http://hz.zycfv.cn/gtysccvqhh.html

Go:   resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtpgocojex.html

Ruby: resp.code.to_i
来源：http://hz.jinyuanbaomall.cn/gtnumvqbxf.html

C#:   (int)resp.StatusCode
来源：http://hz.gaohongyu789.top/gtsoqdxlus.html

[L08] 并发请求多个地址
来源：http://hz.smart0.xyz/gtfxepzect.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ydzc1.top/gtqgvtqfcg.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gtmxrykppy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtqtvrxvhd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtnnlkoefo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.52xcode.cn/gtofjzonry.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tian-w.cn/gtrmunztbn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yvedp.cn/gtsdyvezoc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jiagoushi.top/gthcnfnqjs.html

================================================================================
来源：http://hz.yangfankeji.com/gtftrvriep.html

M. 命令行 / 进程 / 环境
来源：http://hz.quarkkingdee.top/gtiyhrcitd.html

================================================================================
来源：http://hz.nanxuanxn.top/gtbigczeou.html

[M01] 读取命令行参数
来源：http://hz.zhoulong.xyz/gtmvyiuhmu.html

Py:   sys.argv[1:]
来源：http://hz.ppjwa.cn/gteuldbdsd.html

PHP:  $argv;  $argc;
来源：http://hz.yuxming.cn/gttyvlsxel.html

JS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtkbzwlkjv.html

TS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtihrwjfnp.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gtchunhlez.html

Go:   os.Args[1:]
来源：http://hz.chenlongwang.top/gtafpvpdxi.html

Ruby: ARGV
来源：http://hz.gzhubu.top/gtdgucbdbm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ppjwa.cn/gtsvuisifs.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtuspizbis.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtdbqhkeqc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aizwys.cn/gtqjpperzm.html

JS:   process.env.HOME
来源：http://hz.ybcxt.top/gthbgoholi.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gtexappfqd.html

Java: System.getenv("HOME")
来源：http://hz.andypj.xyz/gtugkhflfb.html


<!-- 参考信息 -->