代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtnbhfknwq.html

[I07] 忽略大小写与多行模式
来源：http://hz.gotoacloud.top/gtsexlwmdl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jianghu66.top/gtglcmvznr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhiwuduotai.top/gtpnegbkic.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hywenlv.cn/gttcuqxbxf.html

TS:   /error/gim
来源：http://hz.zhixingplan.top/gtrbephztz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhijiandao.cn/gtzwbptdpq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aizwys.cn/gtkreencrg.html

Ruby: s.scan(/error/i)
来源：http://hz.gotoacloud.top/gthpgyysmb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jlsjyb.cn/gtaqsuihgs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cdnleiting.top/gtvwuwtswh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgfzy.top/gttlopzovh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zycfv.cn/gtrphhbkhv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gteanxikki.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtsukjgmfu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtyhcaqobs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tanke756.top/gtfavtraer.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtkmjovtbv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtysodgvfa.html

================================================================================
来源：http://hz.xuanzx.com/gtrmuvgkld.html

J. 日期与时间
来源：http://hz.ydjk.org.cn/gtxakvekbc.html

================================================================================
来源：http://hz.316326.xyz/gtnaxfiqsn.html

[J01] 获取当前时间
来源：http://hz.mhx1999.top/gtqwibmkfv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.haohaochexian.top/gtvctqxkda.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinghuilouyu.cn/gtegptfwnz.html

JS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtncjupqlp.html

TS:   new Date();  Date.now()
来源：http://hz.gotoacloud.top/gtoqybhivr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jlsjyb.cn/gtqayeakzd.html

Go:   time.Now()
来源：http://hz.gzhubu.top/gtdfgafbrm.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gttoxfzjpq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gtfvoarnzv.html

[J02] 格式化输出
来源：http://hz.chenjidiqi.icu/gtorgmwggu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtkkwkgnke.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gthckhxprj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuetiantiany.cn/gtiocpqicr.html

TS:   d.toISOString()
来源：http://hz.cashguo.top/gtaydultst.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jiagoushi.top/gtudflfeqz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.redwolf501.top/gthxymnbzg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtisamcplb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtjtkszirc.html

[J03] 字符串解析为日期
来源：http://hz.quarkkingdee.top/gtuwmxwiqf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtubaxzblw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangkeji.top/gtrtgdgvxz.html

JS:   new Date("2024-01-02")
来源：http://hz.hysaishi.cn/gtxxuyycxs.html

TS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtofpjrzgd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtcexmhxkg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shuidangran.top/gthsixjaho.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtmsjayktx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.andypj.xyz/gtpswnxbam.html

[J04] 时间戳与日期互转
来源：http://hz.c1oappe.top/gtupodwtms.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gaohongyu789.top/gtxryetnlj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnxiangtu.top/gtuvngsrqf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xinyue.icu/gteifrfifi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pengpengdd.cyou/gtahpuvler.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtvpjnsbjy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.dashuyun.cn/gtblqbagtp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtmevwceqe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dashuyun.cn/gtlnywjrgl.html

[J05] 时间加减（加 7 天）
来源：http://hz.xziqi.cn/gtgcitrijn.html

Py:   now + timedelta(days=7)
来源：http://hz.ydjk.org.cn/gthlxblqhn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aibaodan.cn/gtnacqtciz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gtjnsvndaf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtscwgkoqe.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sxryk.cn/gtjjosnepz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinyuanbaomall.cn/gtfhfygown.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guannengcc.top/gtcbhibmqt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtblabgopg.html

[J06] 计算两时间之差
来源：http://hz.shuidangran.top/gtkcvrbvil.html

Py:   (end - start).total_seconds()
来源：http://hz.zhaomingkeji.xyz/gtbpaffmpu.html

PHP:  $end->diff($start)->days;
来源：http://hz.sysykeji.top/gtmppwcevc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yonumen.top/gtmdmyzgbg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.quarkkingdee.top/gtaebdfzfw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ppjwa.cn/gtjwfmdudw.html

Go:   end.Sub(start).Hours()
来源：http://hz.yvedp.cn/gtmbiswdez.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtwmzncjbv.html

C#:   (end - start).TotalSeconds
来源：http://hz.shuidangran.top/gtruyfvdkr.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gtdlftnzfj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gttvwwbwpg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ehwqpu.com/gtxavmjvnt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtlpqvsgnd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtozfzeiuw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tanke756.top/gtilmhokme.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.havefunace.top/gtunbgrgib.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtqklfjzch.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtfjcjhrbj.html

[J08] 提取年月日与星期
来源：http://hz.shuidangran.top/gtqjxrslkg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.316326.xyz/gtmyojudbz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgfzy.top/gtdiqgtlpx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xziqi.cn/gtzhtzdhme.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shangyingyoupin.top/gtoukldois.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ivvv.top/gtjcbtwdbl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cheryme.top/gtvtthdwig.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuxming.cn/gtvypoiury.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yvedp.cn/gtqlspvuew.html

[J09] 时区处理
来源：http://hz.fengsongda.top/gtarsngdaq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shzxlz.cn/gtpqzarzex.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtjefdktxq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtjzqweudp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtknhsxrcu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydzc1.top/gtxdaaueud.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nwbrower.top/gtbxndjnvc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenlongwang.top/gthvjdnqyk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hammf.cn/gtkywcfuau.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gttlfzojhf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtboxokgrj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuxming.cn/gteruwifgs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangdashe.top/gttqsdkakl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenzaomai.com/gtuiwsrrfb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tianlin.xyz/gtgapfwvio.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhongyouzk.top/gtssxhjhrr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtnxxvmtqd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.kuanghao11.cn/gtzabppjlf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtgvlnixhc.html

K. JSON 与序列化
来源：http://hz.shuidangran.top/gtkoegfote.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbxmnudzu.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gtjwvoatyf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtltwwbysy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtusmyljtc.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtgwdwnfgd.html

TS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtpxfzxycd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.havefunace.top/gtufkeezlv.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtxlqrqzll.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhiwuduotai.top/gteqcfmuoh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.andypj.xyz/gtjdmadjxy.html

[K02] JSON 字符串转对象
来源：http://hz.xuetiantiany.cn/gttemxreel.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gtuaxucspc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tanke756.top/gtnnotynsj.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtfwdqwsmc.html

TS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtgucxcpog.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cashguo.top/gtdgnhwypp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtkofovxzw.html

Ruby: JSON.parse(s)
来源：http://hz.zhixingplan.top/gtaumnhynd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zdqjudy.top/gttjsyohzu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhixingplan.top/gtjajpsutw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtbyfaakld.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtrfqldemc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtjvnevvgh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtrtkrngsc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zycfv.cn/gtketybogi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gthxhelzod.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yangfankeji.com/gtxemnvwgi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sweek.top/gtnidxiaay.html

[K04] 读取 JSON 文件
来源：http://hz.nanxinkj.top/gtyyuastor.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gtfzwvocvi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.0kj1m.cn/gtvlkvyyxi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gtjolakyhr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtqrmaxfeo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtjvrzlovn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gtjeerhpli.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cucudq.cn/gtffsqadeq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtlvnbbdgc.html

[K05] 深拷贝对象
来源：http://hz.jqgfzy.top/gtrpgrmijw.html

Py:   copy.deepcopy(obj)
来源：http://hz.cqqwz.cn/gtaldvqraw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.9152youxi.cn/gtjpcobnze.html

JS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtkyawchlz.html

TS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtrdaorsjd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tian-w.cn/gtlnzclhmd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hysaishi.cn/gtsenxrzgy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.birdmap.top/gtdqupnzyj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xinyue.icu/gtiforgdjo.html

[K06] 解析 URL 查询串
来源：http://hz.svipenyu.cn/gtzwkxavyw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.havefunace.top/gtuzfzpxnp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinghuilouyu.cn/gtkdroytru.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtgkhsojqp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gtdeasaxts.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shzxlz.cn/gthkfaahqw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258888.top/gtdebsgbhi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangdashe.top/gtdzmujbws.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.snrcjt.cn/gtsxcsvgmt.html

[K07] 进制转换
来源：http://hz.yuxming.cn/gttwhmcgce.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuanzhike.top/gtbdwklllh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hysaishi.cn/gtblgpcvzk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtuxeofjjx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtqrncfays.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtmbvbsfts.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuxming.cn/gtzsvtbjvi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shzxlz.cn/gtzxudtkpn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnxiangtu.top/gtnbtjwgzc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cqqwz.cn/gtibuxhiql.html

Py:   pickle.dumps(obj)
来源：http://hz.xuetiantiany.cn/gtejcwhcht.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daxiang520.top/gtrpntalil.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtqphegmeo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gttosvfquj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtgvgsdtvc.html

Go:   encoding/gob
来源：http://hz.gogol.net.cn/gtxwjwhdzm.html

Ruby: Marshal.dump(obj)
来源：http://hz.vqdsnc.cn/gtptsslgfb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jlsjyb.cn/gtlcfjexcw.html

================================================================================
来源：http://hz.yj20258.top/gtufamkfqv.html

L. 网络请求
来源：http://hz.c1oappe.top/gtofbphdrr.html

================================================================================
来源：http://hz.fengsongda.top/gtfqtnhcdd.html

[L01] 发送 GET 请求
来源：http://hz.chenjidiqi.icu/gtjhpbeqae.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gtgchpevsp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.fzhhl.top/gtvvpbqivm.html

JS:   await fetch(url)
来源：http://hz.ydzc1.top/gtvyyzufwr.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gteuxcmpwg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtrvacyflz.html

Go:   resp, err := http.Get(url)
来源：http://hz.sysykeji.top/gtcktvjmpe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ybcxt.top/gtxzjswesj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cqqwz.cn/gtrmvwlbtz.html

[L02] 发送 POST JSON
来源：http://hz.yangfankeji.com/gtelwluxrl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gotoacloud.top/gtgixyfmpw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinghuilouyu.cn/gtsiyoxroe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gtpdfyxwlj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtdwyolqrq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtmaeiwtmw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhoulong.xyz/gtepyhmtbg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gotoacloud.top/gthqjxvjtl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ehwqpu.com/gtocrjqamc.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gtbvkyvjom.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daxiang520.top/gtzyejmeci.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jyoumei.cn/gthpoouqdz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtafydnicm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gtyltknjyz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zycfv.cn/gtulcwghcm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtscefgjtl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tianlin.xyz/gtlcdguahb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydjk.org.cn/gtasjpmntq.html

[L04] 设置超时
来源：http://hz.tianlin.xyz/gtbbuflgwr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aizwys.cn/gtjlxofywk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cqqwz.cn/gtfrletwsf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtsdzegtai.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtrrtcxogm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.svipenyu.cn/gtidcmujpo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangdashe.top/gtlwtrxmqg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ppjwa.cn/gtvwpovtip.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgufenzy.top/gtsozidfzw.html

[L05] 上传文件（multipart）
来源：http://hz.jlsjyb.cn/gtgahbzcps.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtpyfavvsz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cqqwz.cn/gtaueaexjl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtslqyflip.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtyhxwvbxa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhengqikj.top/gtsrwyetlx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yongpay.top/gtfedsuyeo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gtgbonuwrd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sufxvd.cn/gtbwqpampz.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigufen.top/gtjuawssyd.html

Py:   resp.json()
来源：http://hz.xuetiantiany.cn/gtptbxfraa.html

PHP:  json_decode($body, true);
来源：http://hz.kuanghao11.cn/gtaqnuxpja.html

JS:   await resp.json()
来源：http://hz.ybcxt.top/gtiitrkree.html

TS:   await resp.json()
来源：http://hz.52xcode.cn/gtyaefsksi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgufenzy.top/gtllowejcx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shanyushiyangkeji.top/gthtdveahp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nanxuanxn.top/gtkcpkggla.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guannengcc.top/gtmlffpxij.html

[L07] 处理 HTTP 状态码
来源：http://hz.yangfankeji.com/gtusjybevt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dianchejie.cn/gttxckatpv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yangfankeji.com/gtyrudhqyn.html

JS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtnoaprfkp.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtaxusfnwq.html

Java: resp.statusCode()
来源：http://hz.zhixingplan.top/gtvmybzuwn.html

Go:   resp.StatusCode
来源：http://hz.sweek.top/gtmgbjgxjl.html

Ruby: resp.code.to_i
来源：http://hz.chenzaomai.com/gtqkembxal.html

C#:   (int)resp.StatusCode
来源：http://hz.guannengcc.top/gtcbthxlan.html

[L08] 并发请求多个地址
来源：http://hz.jqgufenzy.top/gtdegwdavv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hammf.cn/gtasmburcr.html

PHP:  curl_multi_init() 系列
来源：http://hz.kuanghao11.cn/gtborbdkax.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtyfnuuuba.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtbqycpknn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jyoumei.cn/gthiqcdpbu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ehwqpu.com/gtivslzfeg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zdqjudy.top/gtrsefmnoi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gtnuststdm.html

================================================================================
来源：http://hz.yanxiufei.cn/gtauxrjvkv.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhixingplan.top/gtpveomzhj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtibmsgkig.html

[M01] 读取命令行参数
来源：http://hz.zycfv.cn/gtnqdhwnzw.html

Py:   sys.argv[1:]
来源：http://hz.yj202588.top/gttqouxfha.html

PHP:  $argv;  $argc;
来源：http://hz.0kj1m.cn/gtvmqjatec.html

JS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gttmtdessq.html

TS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtglmdiqds.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxuanxn.top/gtyuniywrq.html

Go:   os.Args[1:]
来源：http://hz.sufxvd.cn/gtfxhsmskp.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtlpbmnpjy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pengpengdd.cyou/gtbnmkciye.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtlmmheufo.html

Py:   os.environ.get("HOME")
来源：http://hz.ivvv.top/gtcwftneze.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigfzy.top/gtvscfflds.html

JS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtuxrnorsv.html

TS:   process.env.HOME
来源：http://hz.yangfankeji.com/gtzmqvczee.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gtibnsisja.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenjidiqi.icu/gtovcfbxlm.html

Ruby: ENV["HOME"]
来源：http://hz.hfpthk.cn/gtjszqiplg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shuidangran.top/gtttgrqxzp.html

[M03] 执行外部命令
来源：http://hz.hammf.cn/gtetajwbua.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zdqjudy.top/gtzhejllck.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shangyingyoupin.top/gtaweqjdag.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtezprwbya.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtogidxiee.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.0kj1m.cn/gtlkupmktb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cheryme.top/gtjxmraljj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daxiang520.top/gtyslwzqfo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cheryme.top/gtdsnnabzu.html

[M04] 获取当前工作目录
来源：http://hz.xuanzx.com/gtepivqjxi.html

Py:   os.getcwd()
来源：http://hz.jlsjyb.cn/gtvlwuclrc.html

PHP:  getcwd();
来源：http://hz.gogol.net.cn/gtdejuwwph.html

JS:   process.cwd()
来源：http://hz.shuidangran.top/gtpvsokbuq.html

TS:   process.cwd()
来源：http://hz.cashguo.top/gtwoqcecth.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangkeji.top/gtvcgrmbxz.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtmwifxbie.html

Ruby: Dir.pwd
来源：http://hz.hywenlv.cn/gtodrwmyod.html


<!-- 参考信息 -->