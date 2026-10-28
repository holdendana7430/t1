代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.guannengcc.top/gtiottmjte.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sysykeji.top/gtbbflixxk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.mhx1999.top/gtrsfqlwuk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zycfv.cn/gtsmauhlzn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fengsongda.top/gtrvugclqy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtpgnfqlgq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtcvzmyjkf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtzuvpakvz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinghuilouyu.cn/gtbruwreub.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dianchejie.cn/gtogdwooju.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtchapkpon.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmneiwlkt.html

J. 日期与时间
来源：http://hz.gaohongyu789.top/gtfhpreian.html

================================================================================
来源：http://hz.zhixingplan.top/gtkgrpkqvu.html

[J01] 获取当前时间
来源：http://hz.redwolf501.top/gtjsjocgpt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sufxvd.cn/gtabmewmsk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtjebfomoo.html

JS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtjzbbymug.html

TS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtjcjziais.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.smart0.xyz/gtdtsxmrpu.html

Go:   time.Now()
来源：http://hz.yuxming.cn/gtvsjkszjw.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtqnfrvlnr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxinkj.top/gtotscdnlc.html

[J02] 格式化输出
来源：http://hz.cucudq.cn/gtitkfvxgm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtmhjkydop.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gtzrcwcbjo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hammf.cn/gtdlyfkhkh.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtcyhddwhj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jyoumei.cn/gteeywdlsq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.andypj.xyz/gtecgqsgyt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gtpaljgchv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cucudq.cn/gtaiadhxjf.html

[J03] 字符串解析为日期
来源：http://hz.xuetiantiany.cn/gtnbagtdmw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gogol.net.cn/gtoiyhfikw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zdqjudy.top/gtqhpzbjin.html

JS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtpcmqpszu.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtzxzhnxso.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtdjtpoqkg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jlsjyb.cn/gtnjpfvoiv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtbstibujp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.feifeiyinyue.top/gtukzcejjx.html

[J04] 时间戳与日期互转
来源：http://hz.cheryme.top/gtwqhsvtbi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shuidangran.top/gtpuzpqphm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinghuilouyu.cn/gtzdcnhfqp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ppjwa.cn/gtolkdfcnf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pengpengdd.cyou/gtmsaxetcv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jlsjyb.cn/gteulfgbel.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gtmonlrwfw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gogol.net.cn/gtpvzjkhiz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydzc1.top/gtqjpvqgxa.html

[J05] 时间加减（加 7 天）
来源：http://hz.hywenlv.cn/gtbmvwxgcf.html

Py:   now + timedelta(days=7)
来源：http://hz.redwolf501.top/gtwvthzkra.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.0kj1m.cn/gtzvjnnwvg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtfhziymrq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gtbcitwtif.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhaomingkeji.xyz/gtkxzluvcq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cqqwz.cn/gtmpdlloll.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shzxlz.cn/gtnyonihfg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yanxiufei.cn/gtvztetbls.html

[J06] 计算两时间之差
来源：http://hz.shuidangran.top/gtguipdrkl.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangkeji.top/gtkluhhweq.html

PHP:  $end->diff($start)->days;
来源：http://hz.feifeiyinyue.top/gtpydjgqgz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guannengcc.top/gtpnrgevlt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.quarkkingdee.top/gtyxsuoouz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.quarkkingdee.top/gtfmvttzvz.html

Go:   end.Sub(start).Hours()
来源：http://hz.haohaochexian.top/gtadpyexby.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gtrricrjnj.html

C#:   (end - start).TotalSeconds
来源：http://hz.c1oappe.top/gtrmugkqlc.html

[J07] 比较两个日期
来源：http://hz.wangshuangyany.cn/gtwldurjga.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtpjwlrxcw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.andypj.xyz/gtdcgynwrj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtkkdxtqcg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtquhdrrcs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhoulong.xyz/gtmfacnlib.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxinkj.top/gttcxbtjiv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtuzkjlcbj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtjvggwoyc.html

[J08] 提取年月日与星期
来源：http://hz.cashguo.top/gtekimdaeo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aizwys.cn/gtbmmnlpxk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pycfn.com/gtlzbjbqqx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zdqjudy.top/gtwvdjvzpc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtxqrified.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhengqikj.top/gtkoljaeir.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinyuanbaomall.cn/gtecoardpp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pycfn.com/gtskhjilyn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtdpvpvtdd.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gtgnfypxec.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ehwqpu.com/gtlgvyactu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258.top/gtibltimtd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtiyomxxtk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtztcvolwj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenzaomai.com/gtadehight.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yanxiufei.cn/gtfcmfjyze.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtwtmboqet.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jlsjyb.cn/gtyizgtwnq.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxuanxn.top/gtrahircwl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gzhubu.top/gtethlsayo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtdgcpkpqp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangdashe.top/gtamsvebgr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shanyushiyangtech.top/gtdeucqour.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shangyingyoupin.top/gtiawoxbrt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ywan-chungtsiang.top/gtfpjuvgrv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.9152youxi.cn/gtxjfassrs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.vqdsnc.cn/gtutouhoaz.html

================================================================================
来源：http://hz.hysaishi.cn/gthvijqgdr.html

K. JSON 与序列化
来源：http://hz.smart0.xyz/gtdrolefjp.html

================================================================================
来源：http://hz.zhijiandao.cn/gthjjzqopi.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gthlfobxnj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangshuangyany.cn/gtzeiqhlza.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtrdfltzhi.html

JS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtzmowqhhb.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gthrfmyusp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnxiangtu.top/gtzqiogcpj.html

Go:   json.Marshal(obj)
来源：http://hz.xingfuxueyuan.xyz/gtuqhvtnrj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sufxvd.cn/gtjylibeuk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.andypj.xyz/gtmvzgcxgv.html

[K02] JSON 字符串转对象
来源：http://hz.andypj.xyz/gtuvtuxrwe.html

Py:   json.loads(s)
来源：http://hz.iojbl.cn/gtpzczrwui.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fengsongda.top/gtgzyyanaa.html

JS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtlqtjefsc.html

TS:   JSON.parse(s)
来源：http://hz.yongpay.top/gtbtrrgciu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.quarkkingdee.top/gtwuwjeexo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtotgbvexl.html

Ruby: JSON.parse(s)
来源：http://hz.shuidangran.top/gtnunhsrjp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.9152youxi.cn/gtwqfbowba.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gteoyjscbz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtlzkjlqli.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtybrtmgch.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtppygawdi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtzbnjragh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydzc1.top/gttctoinub.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.feifeiyinyue.top/gtxnsfdksx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtcclrevpy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cqqwz.cn/gtjtbktmla.html

[K04] 读取 JSON 文件
来源：http://hz.sysykeji.top/gtbynqtezv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtzcijmxme.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nwbrower.top/gttgidtdxb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtdzhfziav.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtfbsnzlsg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigfzy.top/gtoltbmokk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtretpedbs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hysaishi.cn/gtyuxjwgef.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ehwqpu.com/gtodvnsfon.html

[K05] 深拷贝对象
来源：http://hz.jinghuilouyu.cn/gtitxiasja.html

Py:   copy.deepcopy(obj)
来源：http://hz.redwolf501.top/gtekhxrmze.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtfeaqphij.html

JS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gtacqnrxer.html

TS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtorrebght.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.mhx1999.top/gtlpkvvrxz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daria6918.cn/gtvsujkfsv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.9152youxi.cn/gtudmduqpm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cqqwz.cn/gtenuggsjl.html

[K06] 解析 URL 查询串
来源：http://hz.hnxiangtu.top/gtyvnsjljf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gttmkwexpe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtzpyyhkid.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtzfzugzhv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtgmafzlio.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.havefunace.top/gtvdsmvhvu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtlkcauyxs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtkdzzlksv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtfuwgpjad.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtgffzsgld.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtqiwdozpt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtxofanxjp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtfejtogyj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtmxittzab.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtpkfeeaut.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtavdyssoi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydjk.org.cn/gtxytyyquh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhoulong.xyz/gtevcczhds.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhengqikj.top/gtbitakylk.html

Py:   pickle.dumps(obj)
来源：http://hz.cqqwz.cn/gtbdbinklm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtqenemqpu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigufen.top/gtfwpbbrac.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtcqojsxlu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tianlin.xyz/gtzmabcbxg.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gtfwqcksjp.html

Ruby: Marshal.dump(obj)
来源：http://hz.tianlin.xyz/gtjnkkmeco.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sxryk.cn/gtnlfgstqt.html

================================================================================
来源：http://hz.cashguo.top/gtwixgwhgq.html

L. 网络请求
来源：http://hz.sysykeji.top/gttfnvikhh.html

================================================================================
来源：http://hz.yangfankeji.com/gtifnnvjfn.html

[L01] 发送 GET 请求
来源：http://hz.quarkkingdee.top/gtirnadbxv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tianlin.xyz/gtbnbwixse.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtwdtunone.html

JS:   await fetch(url)
来源：http://hz.xuanzx.com/gtpkvodrhm.html

TS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtpjsgroen.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangkeji.top/gtsxuqfkoq.html

Go:   resp, err := http.Get(url)
来源：http://hz.yueranfly.top/gtdgmfzwyi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hywenlv.cn/gtqqpenpez.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtmusmmaxl.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gtekwfyutk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zdqjudy.top/gtebztjims.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aizwys.cn/gtdxqgxoas.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gtyckikvtt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtqagqvgue.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yvedp.cn/gtdpzwzpbk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.c1oappe.top/gtlpiapkth.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.0kj1m.cn/gtabhrauvv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.haohaochexian.top/gtxutibwuy.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gtkwjpsbkb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tanke756.top/gtjewnetai.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nwbrower.top/gtsphqlngw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtjrbrlbvl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtvqozargv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zdqjudy.top/gtowkmspxy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gtxlpffrre.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nwbrower.top/gtbgrdvxqv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hammf.cn/gtskouzxqf.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gtbxjbceol.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daria6918.cn/gtjrhgefcf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sxryk.cn/gteivdnpxd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtatungbyd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtkbtqnnko.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtiburntwf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.316326.xyz/gtvfzcgfpk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigfzy.top/gtmglfeuaa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jiagoushi.top/gtopotsdrz.html

[L05] 上传文件（multipart）
来源：http://hz.wangdashe.top/gtndepmvjf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sufxvd.cn/gtgavgwnzj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuanzx.com/gtmrndlojv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtxazwugme.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtbuwuxdvz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.wangshuangyany.cn/gtopasscys.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.316326.xyz/gtqrvfqohp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.birdmap.top/gtzwffmrkp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yvedp.cn/gthwskieae.html

[L06] 解析响应为 JSON
来源：http://hz.52xcode.cn/gtadpjmrwd.html

Py:   resp.json()
来源：http://hz.tianlin.xyz/gtviwyjcis.html

PHP:  json_decode($body, true);
来源：http://hz.xinyue.icu/gtsvcvtefy.html

JS:   await resp.json()
来源：http://hz.ydzc1.top/gtgouyxkgv.html

TS:   await resp.json()
来源：http://hz.ivvv.top/gtpvcfhqin.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zycfv.cn/gtsmyrrlwf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zycfv.cn/gtfydhtgvx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jiagoushi.top/gtsnzugmxg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pengpengdd.cyou/gtzbzervxf.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtrnzhjbxx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinyuanbaomall.cn/gtieolosvq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ivvv.top/gtfwgofmir.html

JS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtftxpjqig.html

TS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gtdhifstdp.html

Java: resp.statusCode()
来源：http://hz.nwbrower.top/gtnerquimd.html

Go:   resp.StatusCode
来源：http://hz.daria6918.cn/gtvzxysryo.html

Ruby: resp.code.to_i
来源：http://hz.316326.xyz/gtwrsymqrm.html

C#:   (int)resp.StatusCode
来源：http://hz.zhengqikj.top/gtjyqjmclq.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtbrgvfgal.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangshuangyany.cn/gtptwmiliv.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258.top/gtvhwngqfn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtpjltlcgj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtxyqztbsu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fengsongda.top/gtcyayjhik.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.svipenyu.cn/gtbtonjmom.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtvenmruwu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgfzy.top/gtythaezey.html

================================================================================
来源：http://hz.ybcxt.top/gtlhsyexzb.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtefguovpv.html

================================================================================
来源：http://hz.c1oappe.top/gtkkwpkrca.html

[M01] 读取命令行参数
来源：http://hz.yj20258.top/gtidlravsn.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtkervlqax.html

PHP:  $argv;  $argc;
来源：http://hz.yonumen.top/gtmtsgkjny.html

JS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtiouykzsb.html

TS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gtsrnhxpgm.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gtidzukwww.html

Go:   os.Args[1:]
来源：http://hz.yj202588.top/gtvztpnxvh.html

Ruby: ARGV
来源：http://hz.ivvv.top/gtwrzmpjev.html

C#:   args 数组（Main 方法参数）
来源：http://hz.haohaochexian.top/gtgtpwbcae.html

[M02] 读取环境变量
来源：http://hz.yuxming.cn/gtjfegonly.html

Py:   os.environ.get("HOME")
来源：http://hz.fengsongda.top/gthgknusje.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dashuyun.cn/gtglamlikv.html

JS:   process.env.HOME
来源：http://hz.jqgfzy.top/gtodziitfz.html

TS:   process.env.HOME
来源：http://hz.daria6918.cn/gtceexsfcb.html

Java: System.getenv("HOME")
来源：http://hz.ivvv.top/gtutsgzrfh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ywan-chungtsiang.top/gtpcqvkkaa.html

Ruby: ENV["HOME"]
来源：http://hz.guannengcc.top/gtnpavvkmd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shuidangran.top/gtzotuvnas.html

[M03] 执行外部命令
来源：http://hz.xingfuxueyuan.xyz/gtfxswfrqp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hfpthk.cn/gtkdbgmtoo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gthaimzanm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gticmxyizn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtyewbwiwj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gtiyaursdj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtxurkvzhc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258.top/gtjummkyqf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gtmkmprujk.html

[M04] 获取当前工作目录
来源：http://hz.xuanzx.com/gticdgzadh.html

Py:   os.getcwd()
来源：http://hz.zhaomingkeji.xyz/gtcwytfffm.html

PHP:  getcwd();
来源：http://hz.quarkkingdee.top/gtrihasdcg.html

JS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtvvfhtntt.html

TS:   process.cwd()
来源：http://hz.shzxlz.cn/gttsjjqdzh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shzxlz.cn/gtirojjivh.html

Go:   os.Getwd()
来源：http://hz.wangdashe.top/gtninfukhh.html

Ruby: Dir.pwd
来源：http://hz.wangshuangyany.cn/gtpeaebdct.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gtknafopux.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtywrrhixo.html

Py:   sys.exit(1)
来源：http://hz.havefunace.top/gtndawxmus.html

PHP:  exit(1);
来源：http://hz.nanxinkj.top/gtdqlffoev.html

JS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtkuzsrfft.html

TS:   process.exit(1)
来源：http://hz.xylfe.cn/gtmmcxdqfl.html

Java: System.exit(1)
来源：http://hz.guowangkeji.top/gtkfgpyuny.html

Go:   os.Exit(1)
来源：http://hz.zhiwuduotai.top/gtueqhfxyg.html


<!-- 参考信息 -->