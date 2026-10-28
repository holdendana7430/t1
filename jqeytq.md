代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhiwuduotai.top/gtwkpgjmtn.html

TS:   /error/gim
来源：http://hz.iojbl.cn/gtiwcyjgys.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yanxiufei.cn/gtdegscnuu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.haohaochexian.top/gtvtzsrbxi.html

Ruby: s.scan(/error/i)
来源：http://hz.xuanzx.com/gtdthjewrf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtecmbejxy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigufen.top/gtpnehnpqi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.iojbl.cn/gtskmklmey.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tian-w.cn/gtuypzoivc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtjnmdqlcn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhongyouzk.top/gtmgfzdajw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xylfe.cn/gtdnsjivvo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenlongwang.top/gtuhrgsfsu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtpdwyasly.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtezshldds.html

================================================================================
来源：http://hz.meibo888.top/gtmypjeerd.html

J. 日期与时间
来源：http://hz.nanxinkj.top/gtkyrajxho.html

================================================================================
来源：http://hz.aizwys.cn/gteekwfdhv.html

[J01] 获取当前时间
来源：http://hz.gogol.net.cn/gtemegxcue.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zycfv.cn/gtejjqwfjl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtwwxmyqpx.html

JS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtozoxpuic.html

TS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtxmoivqqt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtgogyykyq.html

Go:   time.Now()
来源：http://hz.xylfe.cn/gtueytkdwe.html

Ruby: Time.now
来源：http://hz.wangshuangyany.cn/gtdlhxesxz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnqzz.top/gtexafmpoh.html

[J02] 格式化输出
来源：http://hz.hywenlv.cn/gtdzbuipen.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pycfn.com/gtafbqmyag.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtfyesgfmp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shangyingyoupin.top/gtzeiuabas.html

TS:   d.toISOString()
来源：http://hz.daria6918.cn/gtpxljhwtp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jianghu66.top/gtlojdgiim.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gtkdupakyq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtkjblwaaq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sxryk.cn/gtgqjxjwwc.html

[J03] 字符串解析为日期
来源：http://hz.fzhhl.top/gtpsygvscp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yueranfly.top/gtoscgwyde.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxuanxn.top/gteoizdeoj.html

JS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtitfgggwi.html

TS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtkcydmvnj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtmknlzial.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guowangkeji.top/gtjftfkupf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cashguo.top/gtbcudnhtc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.meibo888.top/gtppwrmflu.html

[J04] 时间戳与日期互转
来源：http://hz.nanxuanxn.top/gtpabvwxit.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.quarkkingdee.top/gtxnvdhagp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sufxvd.cn/gtflykngyh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gtvdujnvnq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.daxiang520.top/gtbampmjys.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj202588.top/gtlswwflom.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hywenlv.cn/gtsebnhqmn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sysykeji.top/gtgwyafpts.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenzaomai.com/gthzothyiw.html

[J05] 时间加减（加 7 天）
来源：http://hz.feifeiyinyue.top/gtmwvacsnp.html

Py:   now + timedelta(days=7)
来源：http://hz.ywan-chungtsiang.top/gtkfvvsnuh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtfxiuhuks.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtzocaqmfu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtqgrmvieo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhijiandao.cn/gtqpdlenoa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yongpay.top/gtnbutolka.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shanyushiyangkeji.top/gtgelygvlu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tianlin.xyz/gtpfhqpvkg.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtpczklrty.html

Py:   (end - start).total_seconds()
来源：http://hz.xuetiantiany.cn/gtviaopgof.html

PHP:  $end->diff($start)->days;
来源：http://hz.ybcxt.top/gtdfvlnhmo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtabpqzzkq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhijiandao.cn/gtogroseey.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigufen.top/gtmqwoqhqf.html

Go:   end.Sub(start).Hours()
来源：http://hz.cheryme.top/gtfwnyavyd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.bjfxy.top/gtijgydftl.html

C#:   (end - start).TotalSeconds
来源：http://hz.shangyingyoupin.top/gtqvmwisok.html

[J07] 比较两个日期
来源：http://hz.guowangkeji.top/gttmkslhxx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtqtnvvuss.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yanxiufei.cn/gtdlsprytz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtvlrtyhjx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtvcodpjzs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtkyrcoint.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zdqjudy.top/gtiwgezrdi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtlinjbets.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtiaebvarm.html

[J08] 提取年月日与星期
来源：http://hz.ppjwa.cn/gtchdgvivu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gtsbexnsrq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangtech.top/gttmewbsda.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aizwys.cn/gtvqghktzc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhoulong.xyz/gtnnygpchb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.c1oappe.top/gthuhpizjg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aibaodan.cn/gtqpaiuasm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sysykeji.top/gtroxgtmsz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sufxvd.cn/gtrfvfgmjv.html

[J09] 时区处理
来源：http://hz.yueranfly.top/gtysnzzegz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gtcoiblghl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guannengcc.top/gtrsziyhhx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtwpwojtnw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtdmsvmgjo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangshuangyany.cn/gtpcvucaoz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ywan-chungtsiang.top/gtphhmjzaw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cashguo.top/gtdzohofsi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigfzy.top/gtidomxgic.html

[J10] 取今天 / 本月第一天
来源：http://hz.aizwys.cn/gtesohtrcx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yangfankeji.com/gtgouxfofz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuanzhike.top/gtfaverpqs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgfzy.top/gtxgnpoycb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuanzx.com/gteigttvte.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tianlin.xyz/gtmjuqqfvu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.iojbl.cn/gtxsrnxlhj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daxiang520.top/gtgdneukbd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtpqhdzvvw.html

================================================================================
来源：http://hz.aibaodan.cn/gtnltzytzo.html

K. JSON 与序列化
来源：http://hz.cqqwz.cn/gtojnubjsh.html

================================================================================
来源：http://hz.52xcode.cn/gtqnufiysu.html

[K01] 对象转 JSON 字符串
来源：http://hz.9152youxi.cn/gtyrqhsbha.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtfuupmhgv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gttrvggbaz.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtzngeqngg.html

TS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtoauwwnlj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cdnleiting.top/gtrgsbncgm.html

Go:   json.Marshal(obj)
来源：http://hz.cucudq.cn/gtzvznwnuh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gtgafoscbh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dianchejie.cn/gtsawmqlia.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtwurhcgkb.html

Py:   json.loads(s)
来源：http://hz.snrcjt.cn/gtbmipqcwg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtamqodtml.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtzlbuodga.html

TS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtixjopanv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.iojbl.cn/gtmroyvzqe.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtcptahvuv.html

Ruby: JSON.parse(s)
来源：http://hz.chenzaomai.com/gtyyhqmejf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aibaodan.cn/gtbnousdvr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtjdqzcjhv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtxwszttez.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtqtndwvag.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtilrrgrqm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtjfxfbmqz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxuanxn.top/gtfvgmygpm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydzc1.top/gtsxolnwrd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yongpay.top/gtvdslramf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhixingplan.top/gtewadufgb.html

[K04] 读取 JSON 文件
来源：http://hz.nwbrower.top/gtxbelnkpe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigufen.top/gtxmdbjplg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxinkj.top/gtdpquhesl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtnandlwxw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtitsdggio.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtwukimhbo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtmriucysy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jianghu66.top/gtkwzrzfki.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cheryme.top/gtxuanegdo.html

[K05] 深拷贝对象
来源：http://hz.yj20258888.top/gtlxtggtwj.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtqtcwhiwn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gtammxsbwj.html

JS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtsbnburtj.html

TS:   structuredClone(obj)
来源：http://hz.yj20258888.top/gtiypvagop.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.9152youxi.cn/gtgqgjazkl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtyafamwaf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.mhx1999.top/gtqijsxtpk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jlsjyb.cn/gthtiapakp.html

[K06] 解析 URL 查询串
来源：http://hz.zhengqikj.top/gtrkedydxa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gtkyvqgvsc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ywan-chungtsiang.top/gtyoknvgqv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtlcxhcatt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtryacunli.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenjidiqi.icu/gtpmznzsny.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtjzbqrjle.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtrlsrvipm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuanzx.com/gtjbgaktfy.html

[K07] 进制转换
来源：http://hz.iojbl.cn/gtmfojtvco.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtdxelpjhv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dashuyun.cn/gtrgsthvrv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtwbtcjpqf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtojttxkop.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtojxsriqg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dashuyun.cn/gttgzegxia.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gaohongyu789.top/gtimyawtgz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ivvv.top/gtctdghqrb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hfpthk.cn/gtodmwohbl.html

Py:   pickle.dumps(obj)
来源：http://hz.nanxinkj.top/gtyksxydit.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.andypj.xyz/gtiwlzfzgi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtituvsvkc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gtvfbmqcmr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zycfv.cn/gtrmilpnts.html

Go:   encoding/gob
来源：http://hz.wangshuangyany.cn/gtlkyfrfdu.html

Ruby: Marshal.dump(obj)
来源：http://hz.hfpthk.cn/gtpucxrwhe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtxoavfzqt.html

================================================================================
来源：http://hz.daxiang520.top/gtmsbdacng.html

L. 网络请求
来源：http://hz.feifeiyinyue.top/gtfeczpmkx.html

================================================================================
来源：http://hz.kuanghao11.cn/gtparqdbso.html

[L01] 发送 GET 请求
来源：http://hz.havefunace.top/gtuogmpynj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gtqowhycrp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tianlin.xyz/gtsbfftpsf.html

JS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtsqkyawvp.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtcxrpclnk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yvedp.cn/gtooyqomie.html

Go:   resp, err := http.Get(url)
来源：http://hz.shangyingyoupin.top/gtiltpotyf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gaohongyu789.top/gtzovgrwjw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.c1oappe.top/gtmtheaylz.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gtphbjohxh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.bjfxy.top/gtebfzldxl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tianlin.xyz/gtecmxjatn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtlvrjsnih.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtheqvsvbf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangtech.top/gttifmqiyf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hywenlv.cn/gtnxhmjpff.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xingfuxueyuan.xyz/gttqxskjom.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinyuanbaomall.cn/gtpmxocvsu.html

[L03] 设置自定义请求头
来源：http://hz.zhongyouzk.top/gtujgmrukc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.svipenyu.cn/gtconknccp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhongyouzk.top/gtymdurgpp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gtmxvqdvog.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtlojziztm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gtyxkjrpud.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gzhubu.top/gtailxwhau.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zycfv.cn/gtmoclvdwl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gteykuyljl.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtnmcwqnjm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xingfuxueyuan.xyz/gtyjycoxqx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yueranfly.top/gtwrgdxlyx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gtthlgxggf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtxfmqnquz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fzhhl.top/gtvpmbsyml.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxuanxn.top/gttjznyyuv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtlyesgjzn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgfzy.top/gtwxksyqaa.html

[L05] 上传文件（multipart）
来源：http://hz.gotoacloud.top/gtoedhgyya.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ivvv.top/gtnhnmsyhc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yanxiufei.cn/gtiftmdyaj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtbgzaezng.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtrqrvccgj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydzc1.top/gtajmishkx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinghuilouyu.cn/gtgoeakxua.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.meibo888.top/gtazapssct.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.svipenyu.cn/gtpgekeiib.html

[L06] 解析响应为 JSON
来源：http://hz.tianlin.xyz/gtkmzlivdj.html

Py:   resp.json()
来源：http://hz.shuidangran.top/gtgazexzqw.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigufen.top/gtrzokgknu.html

JS:   await resp.json()
来源：http://hz.bjfxy.top/gttuciqtwx.html

TS:   await resp.json()
来源：http://hz.yj202588.top/gtpnomdugy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gzhubu.top/gtueckpybg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinghuilouyu.cn/gtrphxdsqs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nanxinkj.top/gtozjqpkbk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yanxiufei.cn/gtwukpsqvs.html

[L07] 处理 HTTP 状态码
来源：http://hz.yanxiufei.cn/gtcjccgiiy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tanke756.top/gtrbdzgfmh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gtjykjcmdd.html

JS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtzoiqdbpj.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtniigewoy.html

Java: resp.statusCode()
来源：http://hz.gotoacloud.top/gtqgvdrifz.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtvkrsdwte.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtsnxtblkk.html

C#:   (int)resp.StatusCode
来源：http://hz.sweek.top/gtgydvurus.html

[L08] 并发请求多个地址
来源：http://hz.pengpengdd.cyou/gtxjucahki.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.meibo888.top/gtdxoyimms.html

PHP:  curl_multi_init() 系列
来源：http://hz.9152youxi.cn/gtdcxxyndq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtouysviqv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtuvvddlwg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gtlluhjqla.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guannengcc.top/gtmddkvypm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgfzy.top/gtemrirmak.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yueranfly.top/gtklgblqmt.html

================================================================================
来源：http://hz.jinqigfzy.top/gtrahrmtxu.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuetiantiany.cn/gttvwzyksh.html

================================================================================
来源：http://hz.ydzc1.top/gtmjvoujuc.html

[M01] 读取命令行参数
来源：http://hz.jiagoushi.top/gtbeiztaii.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangtech.top/gtwqnhqeae.html

PHP:  $argv;  $argc;
来源：http://hz.yanxiufei.cn/gthfbojpiz.html

JS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gtjoukaigg.html

TS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtjvoityes.html

Java: args 数组（main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtxsvqibwz.html

Go:   os.Args[1:]
来源：http://hz.hywenlv.cn/gtzyfibqmd.html

Ruby: ARGV
来源：http://hz.yuxming.cn/gtychxvmpd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hywenlv.cn/gtvzcpqaag.html

[M02] 读取环境变量
来源：http://hz.quarkkingdee.top/gtbagsdwmg.html

Py:   os.environ.get("HOME")
来源：http://hz.tian-w.cn/gtqomtzhvy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtznwaxsxs.html

JS:   process.env.HOME
来源：http://hz.birdmap.top/gtdrzqqapc.html

TS:   process.env.HOME
来源：http://hz.xuanzx.com/gtgkwehceu.html

Java: System.getenv("HOME")
来源：http://hz.nwbrower.top/gtzwizroda.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuanzx.com/gtwjhiylyn.html

Ruby: ENV["HOME"]
来源：http://hz.kuanghao11.cn/gtdtaxvrkf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.kuanghao11.cn/gtnztmvcau.html

[M03] 执行外部命令
来源：http://hz.zhoulong.xyz/gtwkkslbrx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pengpengdd.cyou/gtuukmbzdh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gtmltsjdba.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtheaorccv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gtwaqvzdfa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gtpnkyjlof.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fzhhl.top/gtciarsdwe.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gotoacloud.top/gtumdifxmu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nwbrower.top/gtzwoqactl.html

[M04] 获取当前工作目录
来源：http://hz.yj20258888.top/gtlzmptqhv.html

Py:   os.getcwd()
来源：http://hz.feifeiyinyue.top/gtqniezlmv.html

PHP:  getcwd();
来源：http://hz.nanxuanxn.top/gtwexlgfrz.html

JS:   process.cwd()
来源：http://hz.sxryk.cn/gtspgjzwmg.html

TS:   process.cwd()
来源：http://hz.aibaodan.cn/gtknzqyzjc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.snrcjt.cn/gtxgihoele.html

Go:   os.Getwd()
来源：http://hz.yvedp.cn/gtwevayjzv.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtvalyvjgs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sufxvd.cn/gtkgpbvakj.html

[M05] 设置退出码
来源：http://hz.xuetiantiany.cn/gtxbultind.html

Py:   sys.exit(1)
来源：http://hz.pengpengdd.cyou/gtanhjgwfu.html

PHP:  exit(1);
来源：http://hz.jlsjyb.cn/gtlhwzibeu.html


<!-- 参考信息 -->