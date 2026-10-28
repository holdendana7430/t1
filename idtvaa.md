代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtaqiikadt.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtraayhhih.html

TS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gtsrjmwzzd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxinkj.top/gtmrvksinp.html

Go:   time.Now()
来源：http://hz.nanxuanxn.top/gtechnntyw.html

Ruby: Time.now
来源：http://hz.redwolf501.top/gtvzveprgb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pycfn.com/gtiyrucyip.html

[J02] 格式化输出
来源：http://hz.yangfankeji.com/gtcdwwkidp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtsjmctpbp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gthniidsqt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhongyouzk.top/gtkqmydlxb.html

TS:   d.toISOString()
来源：http://hz.hnxiangtu.top/gtsvgvlazf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhongyouzk.top/gtevermdar.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.haohaochexian.top/gtmxfwfegh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gthstsgxao.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cucudq.cn/gtdqduwjzr.html

[J03] 字符串解析为日期
来源：http://hz.xinyue.icu/gttzprduub.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nwbrower.top/gtxyqjajfy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.0kj1m.cn/gtmdldmcmc.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gttxputijn.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gttwfffhrq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtdkevdess.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtylsejdfb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtmtpaweij.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gtmqnbcsls.html

[J04] 时间戳与日期互转
来源：http://hz.jinyuanbaomall.cn/gtlwudvhjb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgufenzy.top/gtywjucmjx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shangyingyoupin.top/gtruzozvtp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinghuilouyu.cn/gteshjqkjp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtqupkwxkg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yangfankeji.com/gtrjsnwwsh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hysaishi.cn/gtciuaghtq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtkralkuri.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgfzy.top/gtjzktlsnq.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangkeji.top/gtsbciihkr.html

Py:   now + timedelta(days=7)
来源：http://hz.feifeiyinyue.top/gtzqrmnrxf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ybcxt.top/gtshvoulxj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ybcxt.top/gtgblbearc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtoeuygycj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sweek.top/gtxtmtdzlc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtgiuyaxjm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.birdmap.top/gtghgziopj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtujzjlmzl.html

[J06] 计算两时间之差
来源：http://hz.birdmap.top/gtwywkqoha.html

Py:   (end - start).total_seconds()
来源：http://hz.zhongyouzk.top/gtdqeoxyfr.html

PHP:  $end->diff($start)->days;
来源：http://hz.kuanghao11.cn/gtlkqfzhpw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.feifeiyinyue.top/gtfjxdnhat.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hammf.cn/gtffrqtpxm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.pycfn.com/gthinaxhqs.html

Go:   end.Sub(start).Hours()
来源：http://hz.cqqwz.cn/gtqjlegwph.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhongyouzk.top/gtqwtwvrxt.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtpnfpbmgx.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangtech.top/gtrjipjscy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtytrjloft.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gthaykwdgm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtjrbwdhus.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtsnswniya.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dianchejie.cn/gtgiodzwcx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangdashe.top/gtpmiyzgsq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtxrddinra.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtdoyxqpga.html

[J08] 提取年月日与星期
来源：http://hz.sysykeji.top/gtwvkxffql.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.bjfxy.top/gtpsdpkrjo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.birdmap.top/gtzvkuogvu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxinkj.top/gttdwociqo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.havefunace.top/gtxscefktg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ywan-chungtsiang.top/gtmqllcxik.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gzhubu.top/gtudelfnua.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jianghu66.top/gtxsvmnrli.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pycfn.com/gtlnkkchfg.html

[J09] 时区处理
来源：http://hz.yj202588.top/gtxozmuqnz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xingfuxueyuan.xyz/gtwqalxsqf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.bjfxy.top/gtuwwpxcvl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shangyingyoupin.top/gtweulzgqh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtsebbrfdm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhiwuduotai.top/gtloxxaqot.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuanzx.com/gtraodjpgx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhijiandao.cn/gtrggwekku.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jyoumei.cn/gtmxkxitpn.html

[J10] 取今天 / 本月第一天
来源：http://hz.gotoacloud.top/gtonyeupti.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.haohaochexian.top/gtmesyjrku.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dashuyun.cn/gtpgnxhnpv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.iojbl.cn/gtjdrznsbk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hfpthk.cn/gtwfftjslq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gttsvgxddy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhongyouzk.top/gtwqvhldsj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuanzhike.top/gtufzkrzxv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gogol.net.cn/gtjyzffcvw.html

================================================================================
来源：http://hz.9152youxi.cn/gtjvhximib.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtddtvuupp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwfquxcoz.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtapxcofbj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtahsgkyhj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtldmfsjvn.html

JS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtaqrhbqoq.html

TS:   JSON.stringify(obj)
来源：http://hz.xylfe.cn/gtlsaypniy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtowjdqvjd.html

Go:   json.Marshal(obj)
来源：http://hz.fzhhl.top/gtlljrljjo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hysaishi.cn/gtyhdpelun.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aibaodan.cn/gtmhciqgiy.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtfplqckqu.html

Py:   json.loads(s)
来源：http://hz.jqgfzy.top/gtipnvewcg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhiwuduotai.top/gtgqbjkeii.html

JS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtickexelr.html

TS:   JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gthyjqlsnj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.52xcode.cn/gtwimfimcu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gttemvvmsw.html

Ruby: JSON.parse(s)
来源：http://hz.xuanzx.com/gtcrfmnldd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tianlin.xyz/gtbfypczdh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigufen.top/gtaddyadtf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtmpsbscey.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gtmdkyqfgy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtvlcbugok.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gotoacloud.top/gtfvevxyfj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ywan-chungtsiang.top/gthraoivsd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ppjwa.cn/gtfrelqpzz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xingfuxueyuan.xyz/gtxkocmdkg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gzhubu.top/gtzceeuwzf.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gthfsdcrnn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtuobhialt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.52xcode.cn/gtocqdrobt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtrwdcfxbb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtqxlhwzcv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tian-w.cn/gtmefbubis.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtvaomzmmk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj202588.top/gthjjjgxym.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gaohongyu789.top/gtphzqnupg.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtskvarzul.html

Py:   copy.deepcopy(obj)
来源：http://hz.xinyue.icu/gtitvlnawu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtnsszrype.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtizttlymk.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtyvawqixr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sxryk.cn/gtokvagtwg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhengqikj.top/gtpbzterbe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jlsjyb.cn/gtfmewpahh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hfpthk.cn/gtcrrczzid.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtqwhtommr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtiltqiuic.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.0kj1m.cn/gtvtyqspaa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtmubvtofs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtjlcupgzr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shzxlz.cn/gtmzqmlgxl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gtbesmuerw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhengqikj.top/gtfcinmspx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sweek.top/gtdtmehkyt.html

[K07] 进制转换
来源：http://hz.smart0.xyz/gtjkojrxin.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cqqwz.cn/gtenfwlfwz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hammf.cn/gtmyrphatc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtcguwpcsi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtqndcuocs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtdpqusxpn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hammf.cn/gtvutkoocp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtvofskxlo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gtejvyfsca.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gtyksyticq.html

Py:   pickle.dumps(obj)
来源：http://hz.zhixingplan.top/gtyudsppae.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj202588.top/gtiaxvjbvj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtezflpexl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtrfqxshsd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.haohaochexian.top/gtzzuylwec.html

Go:   encoding/gob
来源：http://hz.yj20258.top/gttkxexusc.html

Ruby: Marshal.dump(obj)
来源：http://hz.jiagoushi.top/gtjhveyoye.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jianghu66.top/gtbldgxvjt.html

================================================================================
来源：http://hz.birdmap.top/gtvukwppgv.html

L. 网络请求
来源：http://hz.sxryk.cn/gtajvuqnol.html

================================================================================
来源：http://hz.9152youxi.cn/gtzrtpldju.html

[L01] 发送 GET 请求
来源：http://hz.fengsongda.top/gtnobcpqgr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gtbmjvrply.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtnvuljkhz.html

JS:   await fetch(url)
来源：http://hz.nwbrower.top/gttcboysob.html

TS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtojcjlpfm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aizwys.cn/gtbsxtftdc.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtkdbdizwm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yvedp.cn/gtkbgbcgus.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.svipenyu.cn/gtrrpdqghw.html

[L02] 发送 POST JSON
来源：http://hz.xylfe.cn/gtqfaibphd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtfdcqzvzs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.quarkkingdee.top/gtuaxhpwbb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtrtlvbddw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtysmjahxu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtrrtqzddb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tian-w.cn/gtknxkurhb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cucudq.cn/gtkcnexvbs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxinkj.top/gtviodfzcu.html

[L03] 设置自定义请求头
来源：http://hz.cucudq.cn/gtvpvskbxu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gtklyrmnrz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258.top/gtddmcuzpr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtvgwkvuih.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtntswusii.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cdnleiting.top/gtmzqnufhj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ybcxt.top/gtvwddwvjs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tian-w.cn/gtnnsxgoou.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtsuwtnbxo.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtxrjjqybc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.guowangkeji.top/gtoyczlppo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hnqzz.top/gtakcdmscm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtavrezyxn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gterfhxlza.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aizwys.cn/gtrowqtfwh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sxryk.cn/gtupndnmcz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gogol.net.cn/gtmaljdbar.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gtxpufwqba.html

[L05] 上传文件（multipart）
来源：http://hz.xziqi.cn/gtiamjuyvs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.birdmap.top/gtycedjbqr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.haohaochexian.top/gtebrrsagn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtcbxqsvbb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtxvfuehnx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj202588.top/gtmbjlubwi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj20258888.top/gtzzvksazz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.c1oappe.top/gtwegytjuf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinghuilouyu.cn/gtlbxlwigv.html

[L06] 解析响应为 JSON
来源：http://hz.zhijiandao.cn/gtufxbjdnk.html

Py:   resp.json()
来源：http://hz.chenjidiqi.icu/gtgykjryuz.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtljxnxizh.html

JS:   await resp.json()
来源：http://hz.jiagoushi.top/gtpzuzkkdc.html

TS:   await resp.json()
来源：http://hz.yonumen.top/gtmlntgjlb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtcqxqislq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daxiang520.top/gtuzvmymio.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgfzy.top/gtojymcxri.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dianchejie.cn/gtehtjkpud.html

[L07] 处理 HTTP 状态码
来源：http://hz.yangfankeji.com/gtmgcyxztp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.mhx1999.top/gtojybwzsq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hammf.cn/gtpngppcwa.html

JS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtpofwohhe.html

TS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtfypizhku.html

Java: resp.statusCode()
来源：http://hz.nwbrower.top/gtaifvvpsf.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtaqbpjeen.html

Ruby: resp.code.to_i
来源：http://hz.c1oappe.top/gtojleprxc.html

C#:   (int)resp.StatusCode
来源：http://hz.guowangkeji.top/gtbwihjvsj.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gtxvjnssju.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtydijdjzn.html

PHP:  curl_multi_init() 系列
来源：http://hz.zdqjudy.top/gtdplqxnsx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtmdxcxwuu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtjiyscnry.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tanke756.top/gtkydevrdc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.dashuyun.cn/gtnwmxclkl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxinkj.top/gtbdycpjqc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gtbftwjfjq.html

================================================================================
来源：http://hz.cheryme.top/gtjifglnkg.html

M. 命令行 / 进程 / 环境
来源：http://hz.jyoumei.cn/gtllkntoim.html

================================================================================
来源：http://hz.gogol.net.cn/gtkesotvlh.html

[M01] 读取命令行参数
来源：http://hz.xziqi.cn/gtuxllsiwv.html

Py:   sys.argv[1:]
来源：http://hz.chenzaomai.com/gtezbkzrix.html

PHP:  $argv;  $argc;
来源：http://hz.yvedp.cn/gthwtiqzam.html

JS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gthsvellzw.html

TS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtvoifcygk.html

Java: args 数组（main 方法参数）
来源：http://hz.vqdsnc.cn/gtoyogginl.html

Go:   os.Args[1:]
来源：http://hz.316326.xyz/gtpwydqmzg.html

Ruby: ARGV
来源：http://hz.iojbl.cn/gtnkqtqmse.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenlongwang.top/gtdbvvcqmx.html

[M02] 读取环境变量
来源：http://hz.jianghu66.top/gtmrglppjc.html

Py:   os.environ.get("HOME")
来源：http://hz.hnqzz.top/gteldzrpxw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.vqdsnc.cn/gtnigitwfo.html

JS:   process.env.HOME
来源：http://hz.cucudq.cn/gtwarwqohc.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtdmehrqda.html

Java: System.getenv("HOME")
来源：http://hz.quarkkingdee.top/gtnneikgbn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aizwys.cn/gtsvjiogfl.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtslwcoyrf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xinyue.icu/gtsklxnsfr.html

[M03] 执行外部命令
来源：http://hz.cashguo.top/gtabqjgdpk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.feifeiyinyue.top/gtzagaucxp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangdashe.top/gtbxsxqwmi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zycfv.cn/gthuxjgzra.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtkvpigprs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jlsjyb.cn/gtcdmycafq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xinyue.icu/gtlhyzieat.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxuanxn.top/gtmivwmmzo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gthlmnobiv.html

[M04] 获取当前工作目录
来源：http://hz.jianghu66.top/gttuuktito.html

Py:   os.getcwd()
来源：http://hz.xuanzx.com/gtgwtyzfvk.html

PHP:  getcwd();
来源：http://hz.shangyingyoupin.top/gtdahtcggw.html

JS:   process.cwd()
来源：http://hz.daxiang520.top/gtjqspmtmw.html

TS:   process.cwd()
来源：http://hz.yj20258888.top/gtfwavnkbr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258888.top/gthocskghc.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtkebkvhvn.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtviubdbqh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ybcxt.top/gtqtmrlkqk.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gttzrfknjr.html

Py:   sys.exit(1)
来源：http://hz.bjfxy.top/gtsgwlojnj.html

PHP:  exit(1);
来源：http://hz.nwbrower.top/gtvbghoiod.html

JS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtklcmqkpd.html

TS:   process.exit(1)
来源：http://hz.hnqzz.top/gtrsayksah.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gtsrpiludb.html

Go:   os.Exit(1)
来源：http://hz.xinyue.icu/gttucseqfv.html

Ruby: exit 1
来源：http://hz.tian-w.cn/gtbdutbcxn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtczskewfl.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtdlqsqyjz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fengsongda.top/gtdwxofxwl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtbycbswvx.html

JS:   console.error("err")
来源：http://hz.zhengqikj.top/gtzloeyndf.html

TS:   console.error("err")
来源：http://hz.zhixingplan.top/gtbvlejypz.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gtzagvbing.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jyoumei.cn/gtlphmasgb.html

Ruby: warn "err"
来源：http://hz.jinghuilouyu.cn/gtlxahxetd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cheryme.top/gtqnxnagwd.html

[M07] 判断是否为主入口
来源：http://hz.hywenlv.cn/gtlbenlbvd.html

Py:   if __name__ == "__main__":
来源：http://hz.xuanzx.com/gtpfvoglew.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guowangkeji.top/gtwfyjzbdl.html

JS:   require.main === module
来源：http://hz.daria6918.cn/gthohzyabw.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtuvrxtxqx.html


<!-- 参考信息 -->