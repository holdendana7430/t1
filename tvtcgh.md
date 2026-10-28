代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.shangyingyoupin.top/gtgxpniraw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.52xcode.cn/gtszrpddty.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ivvv.top/gtmxspqgez.html

JS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtpzhibgqg.html

TS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gtjlxfpdqn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtdkenvdpc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.fzhhl.top/gtehtcvcyr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtfnmydqfn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sufxvd.cn/gtuxewrfum.html

[J04] 时间戳与日期互转
来源：http://hz.redwolf501.top/gttdconqit.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhixingplan.top/gtjanlthmo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhongyouzk.top/gtihxlrszf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gttbnhdvqx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhijiandao.cn/gtdvmotelj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuanzhike.top/gtszgoebwt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shuidangran.top/gtcdygnfcr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gtfuwmbckw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.smart0.xyz/gthsqijhta.html

[J05] 时间加减（加 7 天）
来源：http://hz.tian-w.cn/gtdvnymipf.html

Py:   now + timedelta(days=7)
来源：http://hz.zhiwuduotai.top/gtjappllqf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zycfv.cn/gtiiizdeaz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtmjcwczkt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258.top/gtwwvmlmkf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yvedp.cn/gtmzhxrtbb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cdnleiting.top/gtrsijdakg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gogol.net.cn/gtjjyuuzbj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.haohaochexian.top/gtxqoaqrkd.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtlwybuctr.html

Py:   (end - start).total_seconds()
来源：http://hz.0kj1m.cn/gtzrjlalbs.html

PHP:  $end->diff($start)->days;
来源：http://hz.meibo888.top/gtuxmundxq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jlsjyb.cn/gtqvwatjdi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigfzy.top/gthoaxdtqv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxinkj.top/gtjkfaddzt.html

Go:   end.Sub(start).Hours()
来源：http://hz.pycfn.com/gtqtbknidu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnxiangtu.top/gtzaraltcs.html

C#:   (end - start).TotalSeconds
来源：http://hz.mhx1999.top/gtzbbnspkt.html

[J07] 比较两个日期
来源：http://hz.zhengqikj.top/gtbtfmycmd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtufhexdos.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgufenzy.top/gtldrpgpuz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtznpzwiaa.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtaptbyjfy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gtugsdihyt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shuidangran.top/gtlwfuubkf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtlkgaspbu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtksqvzjag.html

[J08] 提取年月日与星期
来源：http://hz.yj20258.top/gtzuleunkj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtfadfpybt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sysykeji.top/gtdryqxzgq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj20258888.top/gtuyciwfiu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.havefunace.top/gtdcjvpbcs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtlbfqlkee.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gtltimmhpp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.316326.xyz/gthypvetxy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.haohaochexian.top/gtjtylpsic.html

[J09] 时区处理
来源：http://hz.jinyuanbaomall.cn/gtatcjlvra.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gttmkoaigz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tanke756.top/gtkrzqtufm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aizwys.cn/gtlburvpyb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtwaaayeqk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jlsjyb.cn/gthafgjhgy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zycfv.cn/gtsabgqitd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gtkchmhqvi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.feifeiyinyue.top/gtasoptjyu.html

[J10] 取今天 / 本月第一天
来源：http://hz.ivvv.top/gtdfucqqff.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ybcxt.top/gtlrxydpfu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gthgwxmfzl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangtech.top/gtmdewyreh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhongyouzk.top/gtnqpxjdmj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangshuangyany.cn/gtcwxtqiwf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.vqdsnc.cn/gtopezpugb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.0kj1m.cn/gtrexecmvh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ywan-chungtsiang.top/gtknfznkga.html

================================================================================
来源：http://hz.ivvv.top/gtbcuufbig.html

K. JSON 与序列化
来源：http://hz.nanxinkj.top/gtfiiavgcf.html

================================================================================
来源：http://hz.yj202588.top/gtniumzrsn.html

[K01] 对象转 JSON 字符串
来源：http://hz.yanxiufei.cn/gtlyezrpve.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtmpudzipr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtljrbvhzx.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtvzobhxzt.html

TS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtvphitrfs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhixingplan.top/gtcydrqfpv.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtuddpistq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guannengcc.top/gtqxzngazq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ywan-chungtsiang.top/gtgmnjrege.html

[K02] JSON 字符串转对象
来源：http://hz.tianlin.xyz/gthmkuacib.html

Py:   json.loads(s)
来源：http://hz.ppjwa.cn/gtmomkwxvt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gtsvztczsv.html

JS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtmrhupeij.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtpguucpns.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fengsongda.top/gtoglyxaxz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtypqcvnlk.html

Ruby: JSON.parse(s)
来源：http://hz.meibo888.top/gtwhuirksc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zycfv.cn/gtehadzwik.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.svipenyu.cn/gthhefcdzy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtjvjmwnyw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtygqkvgdw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtshkbunis.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtaazbomgv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtnzxtpahh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cashguo.top/gtivqsibee.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.guannengcc.top/gthbcuwlwz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cdnleiting.top/gtbrdmcopp.html

[K04] 读取 JSON 文件
来源：http://hz.meibo888.top/gtzvdblvzp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xingfuxueyuan.xyz/gtqrrirkzi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.andypj.xyz/gtdokeoxej.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtugcggcti.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtjpervlob.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gtbxxtzsne.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtgbnxjfkx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtjgcweqxl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangshuangyany.cn/gttwkxairm.html

[K05] 深拷贝对象
来源：http://hz.cashguo.top/gtzvguswxo.html

Py:   copy.deepcopy(obj)
来源：http://hz.feifeiyinyue.top/gtxaxzopwg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guannengcc.top/gtgqgeomeg.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gttakdtgbd.html

TS:   structuredClone(obj)
来源：http://hz.redwolf501.top/gtcdkyyqth.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtdfvcnhof.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jiagoushi.top/gtpuivondf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhijiandao.cn/gtttgfnbsy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aibaodan.cn/gtlmlkxfaa.html

[K06] 解析 URL 查询串
来源：http://hz.guowangkeji.top/gtasovkicy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtscdkuonz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtripgnsup.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtgulvktiw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtjrsotcfk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zycfv.cn/gtmdownigm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ybcxt.top/gtrpncipsp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daxiang520.top/gttmgmrpgx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtbeefirwp.html

[K07] 进制转换
来源：http://hz.zhoulong.xyz/gtzfuuyqgu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yueranfly.top/gtzpoltqko.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shzxlz.cn/gtasasbxtf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gttkykesot.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtmuxrawnc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cashguo.top/gtkjmtndas.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtrzwgbxnw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtlvidndiy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtgfetcmfv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangdashe.top/gtqvdqellr.html

Py:   pickle.dumps(obj)
来源：http://hz.hnxiangtu.top/gtnopwwdja.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jyoumei.cn/gtwtvxwoah.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gtgzkacqau.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtpkcmjyan.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ehwqpu.com/gtqnupwvvs.html

Go:   encoding/gob
来源：http://hz.jqgfzy.top/gtlcqhiqxj.html

Ruby: Marshal.dump(obj)
来源：http://hz.daxiang520.top/gtkmkhrxvi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gotoacloud.top/gtaebunwis.html

================================================================================
来源：http://hz.havefunace.top/gtwyatojlp.html

L. 网络请求
来源：http://hz.daria6918.cn/gtnrgbrmqz.html

================================================================================
来源：http://hz.chenlongwang.top/gtnrznzglh.html

[L01] 发送 GET 请求
来源：http://hz.gogol.net.cn/gtzzbgvdnf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cqqwz.cn/gtybnavyei.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangkeji.top/gtkgtuztkr.html

JS:   await fetch(url)
来源：http://hz.daxiang520.top/gtcrnrizuy.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtwfyzabxh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.dianchejie.cn/gtmucqsstc.html

Go:   resp, err := http.Get(url)
来源：http://hz.guowangkeji.top/gtoopcdscm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gaohongyu789.top/gtgplfzrnw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.guowangkeji.top/gtrenztfyp.html

[L02] 发送 POST JSON
来源：http://hz.52xcode.cn/gtpyurtvuw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cashguo.top/gtjbcwyqns.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.316326.xyz/gtgupopqzc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtcmyljkei.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtmubzsosi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ppjwa.cn/gtkloemrft.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daxiang520.top/gteedhcstp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhaomingkeji.xyz/gtjmhoozwi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shangyingyoupin.top/gtqkkueeuu.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gtkixkflnh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenjidiqi.icu/gtugwdjbsl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.daxiang520.top/gtlnfsbafv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtuomaaijy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtcfgmqxya.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuxming.cn/gtwqdgzgdr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtetmqjsti.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yonumen.top/gtwlllwufe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtznbvkrmk.html

[L04] 设置超时
来源：http://hz.xingfuxueyuan.xyz/gtgbnleqxk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gogol.net.cn/gtoybkzleo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gtbrxsfioc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtzdwtvpbx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cqqwz.cn/gtehwrhunq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.iojbl.cn/gteedlbukc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gtepbbkede.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhengqikj.top/gtbmqrwwiy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgfzy.top/gtbdhrvhad.html

[L05] 上传文件（multipart）
来源：http://hz.shzxlz.cn/gtroyaivyj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gtmmftgugt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.havefunace.top/gtdpacrkay.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtzqxqvufw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtxsomnsaz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shuidangran.top/gthctmaxbi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tian-w.cn/gthtyvliln.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xuetiantiany.cn/gtkayukdqg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgfzy.top/gtpnnfrayk.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtmngpylmc.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtyatoauew.html

PHP:  json_decode($body, true);
来源：http://hz.pengpengdd.cyou/gtnauofhlj.html

JS:   await resp.json()
来源：http://hz.yj202588.top/gteezmymxf.html

TS:   await resp.json()
来源：http://hz.birdmap.top/gtuekdezwq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhoulong.xyz/gtcgwsqcah.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shangyingyoupin.top/gtgvbsvalk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aibaodan.cn/gtdnjpxstz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhongyouzk.top/gtgpyjsekb.html

[L07] 处理 HTTP 状态码
来源：http://hz.c1oappe.top/gtetqcwxuu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.havefunace.top/gtaxejltrs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shuidangran.top/gtinlpuomq.html

JS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtpkvufcog.html

TS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtahuqzobj.html

Java: resp.statusCode()
来源：http://hz.dianchejie.cn/gtvzrlyogr.html

Go:   resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtaiuziuob.html

Ruby: resp.code.to_i
来源：http://hz.kuanghao11.cn/gtcymofcgf.html

C#:   (int)resp.StatusCode
来源：http://hz.xylfe.cn/gtkqyhoomm.html

[L08] 并发请求多个地址
来源：http://hz.aibaodan.cn/gtepeswjcr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gzhubu.top/gtgehcljmq.html

PHP:  curl_multi_init() 系列
来源：http://hz.andypj.xyz/gtlfxtmbot.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtamdejjoi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtduejxnan.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangdashe.top/gtbrtjmdzz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ydzc1.top/gtsdiiydme.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigufen.top/gtgbanmmro.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yvedp.cn/gtoetxwvar.html

================================================================================
来源：http://hz.sxryk.cn/gtcrlgzumt.html

M. 命令行 / 进程 / 环境
来源：http://hz.xingfuxueyuan.xyz/gtxkemqpsx.html

================================================================================
来源：http://hz.hnxiangtu.top/gtbdtnjkhy.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtjndllkum.html

Py:   sys.argv[1:]
来源：http://hz.zhoulong.xyz/gtjlybppwm.html

PHP:  $argv;  $argc;
来源：http://hz.daxiang520.top/gtlhosxbjj.html

JS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtbrbjnyyf.html

TS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gteuoqgcyv.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtxwxanrgy.html

Go:   os.Args[1:]
来源：http://hz.nanxuanxn.top/gtzscpbzkb.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtyfsewnth.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shangyingyoupin.top/gthdcutgeb.html

[M02] 读取环境变量
来源：http://hz.xylfe.cn/gtsuapotns.html

Py:   os.environ.get("HOME")
来源：http://hz.tian-w.cn/gtuhlrznnv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.0kj1m.cn/gtqlhfftea.html

JS:   process.env.HOME
来源：http://hz.yuanzhike.top/gtapgyochw.html

TS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtlkcrncmi.html

Java: System.getenv("HOME")
来源：http://hz.meibo888.top/gtyquyyqbz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtjyzbtdrv.html

Ruby: ENV["HOME"]
来源：http://hz.zhixingplan.top/gttfgkyzqd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtbmxnyrtq.html

[M03] 执行外部命令
来源：http://hz.kuanghao11.cn/gtcxhufcop.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtbqdfkpes.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gteadkvarc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtxawpengg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtukvgjuhs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daxiang520.top/gtpepyrvro.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yangfankeji.com/gtjvcmxhyn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj202588.top/gtbylymcij.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxuanxn.top/gtrgyflrdw.html

[M04] 获取当前工作目录
来源：http://hz.ydzc1.top/gtyrjtammc.html

Py:   os.getcwd()
来源：http://hz.yj20258888.top/gtmjbnfitz.html

PHP:  getcwd();
来源：http://hz.52xcode.cn/gtlpoxskvh.html

JS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtldskqbzy.html

TS:   process.cwd()
来源：http://hz.ydzc1.top/gtseirgugo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuxming.cn/gtkimtivpp.html

Go:   os.Getwd()
来源：http://hz.jianghu66.top/gtuhyteanf.html

Ruby: Dir.pwd
来源：http://hz.guowangkeji.top/gtdfmqfvfm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daxiang520.top/gtbpvcyqyl.html

[M05] 设置退出码
来源：http://hz.zdqjudy.top/gtkuijbdhy.html

Py:   sys.exit(1)
来源：http://hz.jianghu66.top/gtbjaigwuw.html

PHP:  exit(1);
来源：http://hz.hywenlv.cn/gtfuowviol.html

JS:   process.exit(1)
来源：http://hz.iojbl.cn/gtklaqdqoh.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtdwyijace.html

Java: System.exit(1)
来源：http://hz.tianlin.xyz/gtdqxhdked.html

Go:   os.Exit(1)
来源：http://hz.9152youxi.cn/gtuosyfwpq.html

Ruby: exit 1
来源：http://hz.tianlin.xyz/gtavjltdsy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pycfn.com/gtzlyisviq.html

[M06] 向标准错误输出
来源：http://hz.yangfankeji.com/gtipkmrjmp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtarcvikem.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yvedp.cn/gtfnocpvfs.html

JS:   console.error("err")
来源：http://hz.yangfankeji.com/gtsihgrnex.html

TS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtwqcskhvu.html

Java: System.err.println("err")
来源：http://hz.aizwys.cn/gtavyujltb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuanzx.com/gtvrkhtmoy.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gteiihvbpr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zdqjudy.top/gtgvaorgwv.html

[M07] 判断是否为主入口
来源：http://hz.feifeiyinyue.top/gtdbbbclih.html

Py:   if __name__ == "__main__":
来源：http://hz.chenjidiqi.icu/gtmoomkdio.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxinkj.top/gtvjjbkwlo.html

JS:   require.main === module
来源：http://hz.fengsongda.top/gtlsjoilhr.html

TS:   require.main === module
来源：http://hz.mhx1999.top/gtknfvmlij.html

Java: public static void main(String[] args)
来源：http://hz.nanxinkj.top/gtgjttytol.html

Go:   func main()
来源：http://hz.xinyue.icu/gtqbcoekdn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.redwolf501.top/gtnxehgjyp.html

C#:   static void Main(string[] args)
来源：http://hz.zhixingplan.top/gtpszcugvw.html

[M08] 获取系统与运行时信息
来源：http://hz.birdmap.top/gthqkxooxb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhongyouzk.top/gtdlamxplx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yanxiufei.cn/gtgigeknvu.html

JS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtsllwlzfx.html

TS:   process.platform;  process.version
来源：http://hz.ivvv.top/gtonqlrfji.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuxming.cn/gtqfyrdlma.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cqqwz.cn/gtmpffidjr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gtaxsulrup.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jianghu66.top/gtwuwsdyzf.html

================================================================================
来源：http://hz.yvedp.cn/gtdshzriiu.html

N. 数据结构与算法
来源：http://hz.zhiwuduotai.top/gtwnyfmoxo.html

================================================================================
来源：http://hz.meibo888.top/gtatiapqyj.html


<!-- 参考信息 -->