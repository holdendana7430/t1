代发 wailian999

J. 日期与时间
来源：http://hz.cqqwz.cn/gtdsjdtgmm.html

================================================================================
来源：http://hz.shuidangran.top/gtdfsixngd.html

[J01] 获取当前时间
来源：http://hz.cdnleiting.top/gtoqusamrs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cheryme.top/gtlnoybpft.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtfowizasb.html

JS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtqbvylzse.html

TS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gtodypnfha.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yanxiufei.cn/gttuwuptxo.html

Go:   time.Now()
来源：http://hz.pengpengdd.cyou/gtdorbzssr.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gtvomcayzq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.316326.xyz/gtggirlaau.html

[J02] 格式化输出
来源：http://hz.dianchejie.cn/gtxfrrimvm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtpnllzuax.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtropzjatx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.9152youxi.cn/gthglnjyow.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gtdkqildoh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dashuyun.cn/gtauzcdidp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yueranfly.top/gtgxesfbao.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtrwjsxgyv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pengpengdd.cyou/gtwgjxrkkw.html

[J03] 字符串解析为日期
来源：http://hz.chenzaomai.com/gtuuqwppuf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gtunsofhos.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.haohaochexian.top/gtelejpuwa.html

JS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtigmsinft.html

TS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtwijamtos.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtsipfvigf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gttpcvbkrc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtnnbuwjyg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxinkj.top/gtspemkevu.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtiyxjwcpb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnqzz.top/gteurnwhgf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xziqi.cn/gteeuzufcf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinghuilouyu.cn/gtpapuqkdf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.svipenyu.cn/gtqmqpabbl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.vqdsnc.cn/gtnmjyzxac.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gtsfdfytrb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xingfuxueyuan.xyz/gtnmszaayw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yueranfly.top/gthjzeynag.html

[J05] 时间加减（加 7 天）
来源：http://hz.cucudq.cn/gtocfsuhpc.html

Py:   now + timedelta(days=7)
来源：http://hz.xuanzx.com/gtxgkkqekb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhengqikj.top/gtwsjeucfc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtfnyvapmh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtakhpevkx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cheryme.top/gtxidmzfis.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj20258.top/gtqsbxzyza.html

Ruby: Time.now + 7 * 86400
来源：http://hz.9152youxi.cn/gtpmuwiwzi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ywan-chungtsiang.top/gtntglytwc.html

[J06] 计算两时间之差
来源：http://hz.gzhubu.top/gtmqqwymnn.html

Py:   (end - start).total_seconds()
来源：http://hz.zhijiandao.cn/gtvhjtwrtr.html

PHP:  $end->diff($start)->days;
来源：http://hz.snrcjt.cn/gtaipqdkpl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuetiantiany.cn/gtoaijpupm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.snrcjt.cn/gtntyvlcef.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtawadjgwp.html

Go:   end.Sub(start).Hours()
来源：http://hz.yangfankeji.com/gtxzoxigds.html

Ruby: end - start                 # 返回秒数
来源：http://hz.9152youxi.cn/gtarexepzs.html

C#:   (end - start).TotalSeconds
来源：http://hz.yvedp.cn/gtxmfwjyei.html

[J07] 比较两个日期
来源：http://hz.jianghu66.top/gtlejnjlfq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtwqcytyds.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.316326.xyz/gtdvsyeccj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtxoodnpda.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtqeapabyq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ywan-chungtsiang.top/gtuuftjfaw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhoulong.xyz/gteizlynlk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtgggfsmzo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtfqgvsunb.html

[J08] 提取年月日与星期
来源：http://hz.jianghu66.top/gtzxkrbseg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yangfankeji.com/gtmmuhxfaj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtngbenyty.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangdashe.top/gtutpcujqw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guannengcc.top/gtjrdwnxja.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cheryme.top/gtpljatkki.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ydjk.org.cn/gtwdmwnrkz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigufen.top/gttwrkgtwq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangkeji.top/gtbqaonfzr.html

[J09] 时区处理
来源：http://hz.yonumen.top/gtlrgphqvz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtmdphkpzb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yangfankeji.com/gtsjppyzsy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgfzy.top/gtyxffwhwf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.smart0.xyz/gtreihomcq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.snrcjt.cn/gtemabcewf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxuanxn.top/gtwglujvfl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hongshengwenyu.top/gtzrtxxhjs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.9152youxi.cn/gtczreuekd.html

[J10] 取今天 / 本月第一天
来源：http://hz.zycfv.cn/gtrkxwfxhz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhoulong.xyz/gtoagbrkrb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtlrbncxwk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxinkj.top/gtoefuiaus.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtfijiujao.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gtfvsmcxnu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258.top/gtmoesfich.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigufen.top/gtxathponr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydzc1.top/gthclrszwk.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkoywqplw.html

K. JSON 与序列化
来源：http://hz.ppjwa.cn/gthlktoiki.html

================================================================================
来源：http://hz.meibo888.top/gtdcxhwhth.html

[K01] 对象转 JSON 字符串
来源：http://hz.shzxlz.cn/gtbfonxmqd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gtfdefucka.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtnhzwzyje.html

JS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtdtxgddnw.html

TS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtrboxxsfy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.0kj1m.cn/gtwomjfghv.html

Go:   json.Marshal(obj)
来源：http://hz.mhx1999.top/gtepgzzifg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.birdmap.top/gtlvqaoikw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhiwuduotai.top/gtwdtitdyd.html

[K02] JSON 字符串转对象
来源：http://hz.yangfankeji.com/gtsispjkja.html

Py:   json.loads(s)
来源：http://hz.redwolf501.top/gtydflpcou.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fengsongda.top/gtrsxdehoy.html

JS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtypuuizjy.html

TS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtdktstabx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhixingplan.top/gtgwyzsugy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtgxfeknay.html

Ruby: JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtwqowqveg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhengqikj.top/gtcstkjzou.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhoulong.xyz/gtdzkqtdwm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cheryme.top/gtajchhlgg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtwgzvhclo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gtxspiycxu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.vqdsnc.cn/gtdnzvbzcf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xingfuxueyuan.xyz/gtdkvduxop.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dianchejie.cn/gtbytpkvmn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenzaomai.com/gtjacftxlf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gtfuciavus.html

[K04] 读取 JSON 文件
来源：http://hz.jiagoushi.top/gtfynnutcg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.316326.xyz/gtlqimjreo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ehwqpu.com/gtabhgzpvo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtnsxsrzru.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtsgqjxzer.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cheryme.top/gtosxrbxgd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtelgdctwc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gttftvreip.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yonumen.top/gtzuvmrkye.html

[K05] 深拷贝对象
来源：http://hz.yj202588.top/gtrqdmrigs.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinyuanbaomall.cn/gtwnpysqlf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtvxiyfsxc.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gtlftltjmp.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtnviyrufk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gtgbugtwph.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gtbeaxpsil.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtxykwoksn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtooklepaq.html

[K06] 解析 URL 查询串
来源：http://hz.jqgufenzy.top/gtscpsbwoj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.birdmap.top/gtcpzgkktz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangtech.top/gtbieutnuj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtgqwlmndn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtwusblwir.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sxryk.cn/gtvemlouuc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtgcllymko.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuanzx.com/gtowqhquov.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuanzx.com/gtjjfejxyq.html

[K07] 进制转换
来源：http://hz.jinqigfzy.top/gtpwdashqd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cqqwz.cn/gtcfknttvb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenlongwang.top/gtodcdqcft.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtefgyomzj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtfylqnbgn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtorzfsovb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gtfaqejctz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj202588.top/gtnbviihnq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ydzc1.top/gtzbmqnmfu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.haohaochexian.top/gtgjbunhfv.html

Py:   pickle.dumps(obj)
来源：http://hz.yongpay.top/gthllijrmp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.haohaochexian.top/gtjlvjeewz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtzxebwryq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtnrpsmygs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.meibo888.top/gtyrczoncw.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gttdamwdyj.html

Ruby: Marshal.dump(obj)
来源：http://hz.9152youxi.cn/gtjmsqecgv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinghuilouyu.cn/gtbizrsmfa.html

================================================================================
来源：http://hz.jianghu66.top/gttcjhwibm.html

L. 网络请求
来源：http://hz.yj20258.top/gthsdraevo.html

================================================================================
来源：http://hz.fzhhl.top/gtqksrhffv.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangkeji.top/gtudygwmuf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.havefunace.top/gtowkuetfr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hysaishi.cn/gtnloiiubr.html

JS:   await fetch(url)
来源：http://hz.tianlin.xyz/gtjwkrejah.html

TS:   await fetch(url)
来源：http://hz.fzhhl.top/gtfqcanyur.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sufxvd.cn/gtoxqviqkw.html

Go:   resp, err := http.Get(url)
来源：http://hz.smart0.xyz/gtwdkotlyu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnxiangtu.top/gtndebrice.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.havefunace.top/gtpvaxksar.html

[L02] 发送 POST JSON
来源：http://hz.sweek.top/gtzjxsrcyn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xylfe.cn/gtlbgrasti.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xylfe.cn/gtcfwrddyf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gthkvmtmsl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gttuogcmsy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangtech.top/gtzgepetcr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zdqjudy.top/gthclrvjio.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtksphqbmi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.redwolf501.top/gtvgzxaaqd.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtrhsebhcr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gtyfxxmwtg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yangfankeji.com/gtxkqlxvit.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtndvrykgw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtyindmnsc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.birdmap.top/gtfncvtxpj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangtech.top/gtvksvbfai.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gtlanjvaza.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtnqwtohwi.html

[L04] 设置超时
来源：http://hz.zycfv.cn/gtafyqoobh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.52xcode.cn/gtxszltsoq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gotoacloud.top/gtzoeghsnd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtsnbnbtlp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xingfuxueyuan.xyz/gtmqnbqxlb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shzxlz.cn/gttumylipg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xylfe.cn/gtbckyzdpx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhoulong.xyz/gtipgxbfvp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gthndpwdhb.html

[L05] 上传文件（multipart）
来源：http://hz.nanxuanxn.top/gtxkucpjqz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gthxkijznq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhoulong.xyz/gtbnoqkvju.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtcbtbenbd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtixabbsjm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cucudq.cn/gthjqthfjp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhengqikj.top/gtmzjizvpn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhijiandao.cn/gtomoxtqtf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.mhx1999.top/gtgkqfoovk.html

[L06] 解析响应为 JSON
来源：http://hz.cqqwz.cn/gtivtbbyqx.html

Py:   resp.json()
来源：http://hz.52xcode.cn/gteizgsgqk.html

PHP:  json_decode($body, true);
来源：http://hz.dianchejie.cn/gtqgvedyhy.html

JS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtenrvqvod.html

TS:   await resp.json()
来源：http://hz.pycfn.com/gteohhcpns.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gtisdgzdnr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pengpengdd.cyou/gtjongxojq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtfakrulyv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtgefpokhc.html

[L07] 处理 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtpqpsldmh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jlsjyb.cn/gtrvyqorgc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pycfn.com/gtvlhvgkux.html

JS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gthiyysarz.html

TS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gthyeibryb.html

Java: resp.statusCode()
来源：http://hz.gogol.net.cn/gthkmplaxy.html

Go:   resp.StatusCode
来源：http://hz.shanyushiyangtech.top/gtkwkvsgej.html

Ruby: resp.code.to_i
来源：http://hz.cashguo.top/gtfpujykdn.html

C#:   (int)resp.StatusCode
来源：http://hz.chenlongwang.top/gtojyldvpc.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gtznddnupa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gthgpaxsaz.html

PHP:  curl_multi_init() 系列
来源：http://hz.hysaishi.cn/gtfztgijvl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtchjktbsc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtorjgtlgd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ywan-chungtsiang.top/gtddmblkoe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sxryk.cn/gtzbzseldj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cashguo.top/gtoraencxe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xinyue.icu/gtnrnyosnv.html

================================================================================
来源：http://hz.zhixingplan.top/gttzsbasdd.html

M. 命令行 / 进程 / 环境
来源：http://hz.daria6918.cn/gthzsgjats.html

================================================================================
来源：http://hz.hywenlv.cn/gtfmelgqje.html

[M01] 读取命令行参数
来源：http://hz.jinqigufen.top/gtrnygceqf.html

Py:   sys.argv[1:]
来源：http://hz.cqqwz.cn/gtsrxaatlw.html

PHP:  $argv;  $argc;
来源：http://hz.yongpay.top/gtwbqncmwo.html

JS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtlnalaajl.html

TS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtrwdflmwz.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtjxxvqgpp.html

Go:   os.Args[1:]
来源：http://hz.meibo888.top/gtwrfwmbkx.html

Ruby: ARGV
来源：http://hz.yvedp.cn/gtszallcbc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.andypj.xyz/gtuugahrfj.html

[M02] 读取环境变量
来源：http://hz.jinqigfzy.top/gtmbiielrd.html

Py:   os.environ.get("HOME")
来源：http://hz.yueranfly.top/gtonarzzji.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtjqmxqrsq.html

JS:   process.env.HOME
来源：http://hz.9152youxi.cn/gtydozpodf.html

TS:   process.env.HOME
来源：http://hz.yuanzhike.top/gtdfefyakc.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gttaerexkl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.feifeiyinyue.top/gtztdrqitb.html

Ruby: ENV["HOME"]
来源：http://hz.0kj1m.cn/gtwjeoglgg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gotoacloud.top/gtkyywipgd.html

[M03] 执行外部命令
来源：http://hz.tianlin.xyz/gtudemqioh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.vqdsnc.cn/gtwwzsbosn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.birdmap.top/gtihzlrgvg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtmlbecnie.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtgdmxdltx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cashguo.top/gtkpttkyfa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shanyushiyangkeji.top/gtpmkbaace.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtarfgzjvw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daria6918.cn/gtnugqagca.html

[M04] 获取当前工作目录
来源：http://hz.vqdsnc.cn/gtpdstqrgc.html

Py:   os.getcwd()
来源：http://hz.jiagoushi.top/gtlbskgiwm.html

PHP:  getcwd();
来源：http://hz.wangshuangyany.cn/gttykyaeel.html

JS:   process.cwd()
来源：http://hz.daria6918.cn/gtkvacbopk.html

TS:   process.cwd()
来源：http://hz.sysykeji.top/gtsdldpjcf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj202588.top/gtntepdhjy.html

Go:   os.Getwd()
来源：http://hz.sweek.top/gtmisvbhny.html

Ruby: Dir.pwd
来源：http://hz.ppjwa.cn/gtqatweitl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xylfe.cn/gteylxvcbf.html

[M05] 设置退出码
来源：http://hz.0kj1m.cn/gtespuuoxc.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gtqnvzwris.html

PHP:  exit(1);
来源：http://hz.yangfankeji.com/gtgqzvilbf.html

JS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtxamruceg.html

TS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtrclxwcwl.html

Java: System.exit(1)
来源：http://hz.yuxming.cn/gtlsnkmkye.html

Go:   os.Exit(1)
来源：http://hz.zhaomingkeji.xyz/gtnnvbahzt.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtuworduyp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangkeji.top/gtftqfvopa.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gtdcerizag.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yangfankeji.com/gtjlzmlgwa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhijiandao.cn/gtgbhhnpba.html

JS:   console.error("err")
来源：http://hz.havefunace.top/gtvrhphcbt.html

TS:   console.error("err")
来源：http://hz.jiagoushi.top/gtwkauoodr.html

Java: System.err.println("err")
来源：http://hz.jqgfzy.top/gtfpgvbwzm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxuanxn.top/gtvhpbbhgd.html

Ruby: warn "err"
来源：http://hz.xziqi.cn/gtfgtjjuqa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.52xcode.cn/gtxlxvyuvv.html

[M07] 判断是否为主入口
来源：http://hz.jinqigfzy.top/gtamrtjotm.html


<!-- 参考信息 -->