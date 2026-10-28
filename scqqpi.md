代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sysykeji.top/gtrkhtstli.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtrrtughqk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.52xcode.cn/gteshhxfjf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.52xcode.cn/gturidlopv.html

Ruby: s.scan(/error/i)
来源：http://hz.ywan-chungtsiang.top/gtzqzriiyd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtcejfsaed.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xingfuxueyuan.xyz/gtsmwqjjfv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fengsongda.top/gtegufjurg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnxiangtu.top/gtxwlpkbex.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtbruljowj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtfkayybxo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhongyouzk.top/gtbygyemzl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dashuyun.cn/gtmojwoimj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hammf.cn/gtjhgepygz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guowangkeji.top/gtlbxyiclz.html

================================================================================
来源：http://hz.zdqjudy.top/gtzvryruwx.html

J. 日期与时间
来源：http://hz.nanxuanxn.top/gtpcgpwweu.html

================================================================================
来源：http://hz.sysykeji.top/gtefedgihq.html

[J01] 获取当前时间
来源：http://hz.fzhhl.top/gtvfjtoiat.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxuanxn.top/gtheboyepe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtmuvtweem.html

JS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtxhofioxc.html

TS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtjlhpntdb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ehwqpu.com/gtgkcggiam.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtumbavjyd.html

Ruby: Time.now
来源：http://hz.gogol.net.cn/gtjezrekuw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sysykeji.top/gtcnxutlpo.html

[J02] 格式化输出
来源：http://hz.yanxiufei.cn/gtcjfccpru.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtcdnjbybo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtnwplwsmn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangdashe.top/gtnwwdythw.html

TS:   d.toISOString()
来源：http://hz.xylfe.cn/gtrclqffkd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.iojbl.cn/gtblirikdg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtxhknreaf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shangyingyoupin.top/gtkicyhruh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj20258.top/gtwdvttjaf.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gtpkvvyyfl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jiagoushi.top/gtlljutngr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shuidangran.top/gtatdcipeq.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtpchwaggp.html

TS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtfhsamcli.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtdklacuji.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj202588.top/gtbnnvtvmc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtaswtheox.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jlsjyb.cn/gtlgaqibhu.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtjmrpcruc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pengpengdd.cyou/gtedvjnbft.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.52xcode.cn/gtbkzwifkn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.smart0.xyz/gtvahfjptq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtyzgcxcdp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hammf.cn/gtnrfrnmoq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gtzppqpxhl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.feifeiyinyue.top/gtqqthokxe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guannengcc.top/gtmwetywgs.html

[J05] 时间加减（加 7 天）
来源：http://hz.hywenlv.cn/gtnzonowqn.html

Py:   now + timedelta(days=7)
来源：http://hz.tian-w.cn/gtocfglwmi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yonumen.top/gtyhzjsfqt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtorpacmna.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aizwys.cn/gtvzlgdoaw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtoghmlwgl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shangyingyoupin.top/gtapkfwcxb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fzhhl.top/gtxmgpobey.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnxiangtu.top/gtxruespft.html

[J06] 计算两时间之差
来源：http://hz.snrcjt.cn/gtacoejrxi.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gtiirtuakp.html

PHP:  $end->diff($start)->days;
来源：http://hz.hywenlv.cn/gtrmfyshme.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.vqdsnc.cn/gtakwnxcng.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtzenlfmph.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtzzradhwc.html

Go:   end.Sub(start).Hours()
来源：http://hz.fengsongda.top/gtxjvpkatf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jlsjyb.cn/gteaurhvev.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenzaomai.com/gtcxvwdcvw.html

[J07] 比较两个日期
来源：http://hz.ybcxt.top/gtyixytvfz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtoccydjqk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ehwqpu.com/gtkiifcerd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydjk.org.cn/gtrzksdnav.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtfafoznur.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gotoacloud.top/gtnlrsinsp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhoulong.xyz/gtfhesghoc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtvfvmniqx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtjdfxikqk.html

[J08] 提取年月日与星期
来源：http://hz.jinghuilouyu.cn/gtwjyewwxq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aibaodan.cn/gthswcgjko.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtdcnkjbrm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cucudq.cn/gttnqsryao.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fzhhl.top/gtcnlqmjip.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yueranfly.top/gtapiyyutv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.birdmap.top/gtsutyjtfu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gtxacdtlqx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtjfbpvasm.html

[J09] 时区处理
来源：http://hz.andypj.xyz/gtjpmxdoed.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhiwuduotai.top/gtkxnlavrc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.meibo888.top/gtpgvmuuka.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gthntvyjan.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.quarkkingdee.top/gtcnwihgts.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuanzx.com/gtssshmnsa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hongshengwenyu.top/gtpzesusgt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.bjfxy.top/gtyzlvkyup.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnxiangtu.top/gtwjpemgea.html

[J10] 取今天 / 本月第一天
来源：http://hz.shuidangran.top/gtmlknlaza.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangshuangyany.cn/gtoriauqic.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnqzz.top/gtxanifimf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.kuanghao11.cn/gtmtpfpnnc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtklptxyys.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gogol.net.cn/gtpdnfoizk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xylfe.cn/gtmhkqslpm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhongyouzk.top/gtpwisbsjx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xinyue.icu/gtwpfgixja.html

================================================================================
来源：http://hz.zhijiandao.cn/gtflwxzafp.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtdyuzmkvx.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdeionqoc.html

[K01] 对象转 JSON 字符串
来源：http://hz.zdqjudy.top/gtmgmmwefs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sweek.top/gtyhojkhac.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gttgovzine.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtmaltdsbe.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtxobrwqji.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hongshengwenyu.top/gtmapjipiu.html

Go:   json.Marshal(obj)
来源：http://hz.aibaodan.cn/gtqyhohrkd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuxming.cn/gtnyzfzisn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xinyue.icu/gtnqgiovch.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtajdfrpbg.html

Py:   json.loads(s)
来源：http://hz.yvedp.cn/gtdblchwqx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258888.top/gtfzjsufnw.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtljebwdmn.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtwfnicfht.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sweek.top/gtppdzfvui.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtlwndxjri.html

Ruby: JSON.parse(s)
来源：http://hz.nwbrower.top/gtmlbnundj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxinkj.top/gtyaoclchb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhijiandao.cn/gtzglhvypb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtbcebkmxz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtozfxccmc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtllmmnhfc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtdxeftihd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtfgyxvydz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.0kj1m.cn/gtndegrupx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yangfankeji.com/gtzpesgbra.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgfzy.top/gtivpzmbpm.html

[K04] 读取 JSON 文件
来源：http://hz.yongpay.top/gtipsgwdcr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtrzzpxybk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gteufsjovz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gthcygutpb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtgeqhejrq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aibaodan.cn/gtpvxqfhzw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtonpbawfd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tianlin.xyz/gtldlbotop.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.redwolf501.top/gtcyxbjekz.html

[K05] 深拷贝对象
来源：http://hz.xziqi.cn/gtvwtijjhs.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gtiuepobct.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sufxvd.cn/gtmbalscaj.html

JS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtvfgkqjjr.html

TS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtymfsmkyt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.mhx1999.top/gtejdivwel.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gtqphnhxvu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cqqwz.cn/gtamchqomv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cqqwz.cn/gtykqblvnf.html

[K06] 解析 URL 查询串
来源：http://hz.sysykeji.top/gtajtatluc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.0kj1m.cn/gtjssppnui.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guannengcc.top/gthctswmxm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtqexffewn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gtanctbufo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.meibo888.top/gtrgffddbr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daria6918.cn/gtqybvlwar.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtnxmpburb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fzhhl.top/gtyhncpyvv.html

[K07] 进制转换
来源：http://hz.xylfe.cn/gtucgthydi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtckhmgeyw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aibaodan.cn/gtvnxqfjpp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtilhunkea.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtyhavvjzi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtzgtiwcrq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.0kj1m.cn/gthcngrpat.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuxming.cn/gtwyqtmqrq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gtnmmvtymm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ywan-chungtsiang.top/gtzcyvzusu.html

Py:   pickle.dumps(obj)
来源：http://hz.ydzc1.top/gtcvqyvwjw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuetiantiany.cn/gtwvkkeosr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtukdknykq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gtvwgcfjbu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gotoacloud.top/gtbapuvrho.html

Go:   encoding/gob
来源：http://hz.yj20258888.top/gtrllommjx.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinyuanbaomall.cn/gtvymtibft.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gzhubu.top/gtjcbioxcr.html

================================================================================
来源：http://hz.yvedp.cn/gtwwxpwtnr.html

L. 网络请求
来源：http://hz.shanyushiyangtech.top/gtnfuebwpu.html

================================================================================
来源：http://hz.guowangkeji.top/gtkdmcqfjh.html

[L01] 发送 GET 请求
来源：http://hz.gogol.net.cn/gtqckabiwl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenlongwang.top/gtavphcsxk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yangfankeji.com/gtxpoympoj.html

JS:   await fetch(url)
来源：http://hz.yuxming.cn/gtxwgmgwxy.html

TS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtxfdcwfey.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tian-w.cn/gtctkgurar.html

Go:   resp, err := http.Get(url)
来源：http://hz.cqqwz.cn/gtmfbizisf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.havefunace.top/gtwrorxuvn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ydjk.org.cn/gtyjbllrrz.html

[L02] 发送 POST JSON
来源：http://hz.zhixingplan.top/gtroiamyjv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zycfv.cn/gtvseezlcq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cdnleiting.top/gtptrswvak.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gthozsnqma.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtdkjcowds.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gtynzimyqq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ybcxt.top/gtrvrhtfjd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.redwolf501.top/gtsgndccvs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.0kj1m.cn/gtjoebvems.html

[L03] 设置自定义请求头
来源：http://hz.feifeiyinyue.top/gtbbkgzjif.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guowangkeji.top/gtjqrrtggl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nwbrower.top/gtwjubqnlq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtublbfqps.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtmdyfvulj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jianghu66.top/gtsdkcqpyf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cheryme.top/gtjntfofzf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.daria6918.cn/gtelttkinw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtwlinudyi.html

[L04] 设置超时
来源：http://hz.yj20258888.top/gtfoayohix.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shzxlz.cn/gtghnmuqmq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.smart0.xyz/gtjlydzzus.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtzatldkbr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtvgdcsgmc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.vqdsnc.cn/gtnfglsskn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yvedp.cn/gteqopilig.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnxiangtu.top/gtxgkeybmo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenzaomai.com/gtkexfivgc.html

[L05] 上传文件（multipart）
来源：http://hz.yvedp.cn/gtulxhrxim.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jiagoushi.top/gtvwzuzudx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ppjwa.cn/gtuxicqlue.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtxrssfmnw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtiipgpppe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.quarkkingdee.top/gtdxhfsngu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.wangshuangyany.cn/gtvxanlhdk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.bjfxy.top/gttddnhtvf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.feifeiyinyue.top/gtxpcubesc.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtzeknxmcm.html

Py:   resp.json()
来源：http://hz.tanke756.top/gtwmmojzer.html

PHP:  json_decode($body, true);
来源：http://hz.cdnleiting.top/gtjpbrovdn.html

JS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtwrdlwwwo.html

TS:   await resp.json()
来源：http://hz.chenlongwang.top/gtduvexczp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtejbzheva.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cucudq.cn/gthrtmmlii.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgfzy.top/gtwypnuglv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydjk.org.cn/gtubzomdyg.html

[L07] 处理 HTTP 状态码
来源：http://hz.hfpthk.cn/gtctiqumvf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.9152youxi.cn/gtvvunknup.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yonumen.top/gtxuceizna.html

JS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtkompszne.html

TS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtaiwvhflv.html

Java: resp.statusCode()
来源：http://hz.yj20258888.top/gtahivmzsn.html

Go:   resp.StatusCode
来源：http://hz.yueranfly.top/gtzjlxbbmq.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtdcebzokb.html

C#:   (int)resp.StatusCode
来源：http://hz.bjfxy.top/gtanilwuir.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtgffljoyf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtoxlslnll.html

PHP:  curl_multi_init() 系列
来源：http://hz.iojbl.cn/gtjvwzxsxg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtjtavjkyx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtgogatmvb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sxryk.cn/gtlipllnkd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cashguo.top/gtgwtwvcuv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.kuanghao11.cn/gtozxespbo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cashguo.top/gtirzeiucu.html

================================================================================
来源：http://hz.gotoacloud.top/gtuvcdhuep.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gtkizkqakr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtiqpbsokn.html

[M01] 读取命令行参数
来源：http://hz.aizwys.cn/gtaornmaor.html

Py:   sys.argv[1:]
来源：http://hz.dashuyun.cn/gtfufdhguz.html

PHP:  $argv;  $argc;
来源：http://hz.smart0.xyz/gtqwsedmme.html

JS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtajvkzeiu.html

TS:   process.argv.slice(2)
来源：http://hz.52xcode.cn/gtvllvgtff.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtpylucevn.html

Go:   os.Args[1:]
来源：http://hz.yangfankeji.com/gtxantlzuu.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtddfqgvwi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnxiangtu.top/gtjbdszunk.html

[M02] 读取环境变量
来源：http://hz.jqgfzy.top/gtvbyasepq.html

Py:   os.environ.get("HOME")
来源：http://hz.mhx1999.top/gtkrlgswla.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hysaishi.cn/gtoidbekta.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtmcpcbgch.html

TS:   process.env.HOME
来源：http://hz.ivvv.top/gtbvnudwte.html

Java: System.getenv("HOME")
来源：http://hz.xuanzx.com/gtjmgmzscs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtuxdydhlu.html

Ruby: ENV["HOME"]
来源：http://hz.gogol.net.cn/gtnnmtyque.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dianchejie.cn/gtyfbhqowt.html

[M03] 执行外部命令
来源：http://hz.jinqigfzy.top/gtffrrdvvq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gzhubu.top/gtrdonnzhy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ppjwa.cn/gtcwlisarp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtjafewarb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dashuyun.cn/gtrxokvobc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tanke756.top/gtzemwmvfq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sweek.top/gtumzfredw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guannengcc.top/gtmividowm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.52xcode.cn/gtueapqkfe.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtuwxgxguz.html

Py:   os.getcwd()
来源：http://hz.guowangkeji.top/gtmoayjxqp.html

PHP:  getcwd();
来源：http://hz.shuidangran.top/gtghzusulp.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtuqbnzckr.html

TS:   process.cwd()
来源：http://hz.9152youxi.cn/gtiinyxioh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258.top/gtepveigmx.html

Go:   os.Getwd()
来源：http://hz.xuetiantiany.cn/gtwchxptrz.html

Ruby: Dir.pwd
来源：http://hz.redwolf501.top/gtoptfkfzh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shuidangran.top/gtsivghxww.html

[M05] 设置退出码
来源：http://hz.ydzc1.top/gtxlxpnlho.html

Py:   sys.exit(1)
来源：http://hz.guowangkeji.top/gtjpvodvjq.html

PHP:  exit(1);
来源：http://hz.ydjk.org.cn/gtuudlylsi.html


<!-- 参考信息 -->