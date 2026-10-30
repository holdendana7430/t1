代发 wailian999

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gqxborgwt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gcdzczfjw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/gcfnbmwdl.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/grqejeeqk.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gjiktcedv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gglwkwzua.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gwxajcaho.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gacslfidq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gfwiefayq.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gjqzicvya.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gmmcpbhzp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/gjxvnnfjc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gmkgmmkbz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gdltfanik.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/ghdwcuozg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gxihiovnj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/gqxzwetjc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gzlcbcgft.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/gwcnypxip.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gwwnjnnhh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gsyvumpbk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gphwhxvzp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gzcgaqcqq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gbtnzltkr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gbpviwjum.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.zdbjq.cn/Article/details/gwhhfubjv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/guzmokptx.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gnnjacbwt.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gjurarcpe.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gkjxwfgvm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/gfqwtpdvq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/gfdlagjbw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gaagzgfpx.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gkixmfnsj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gnwbzehmg.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/ghsdaheeo.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gujkfdwph.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gygrseshk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gcucxzsos.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gimqkxyuc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gonogndcr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gwgomnyhp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gtctykyhp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gmyrwerxe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gjebafrcw.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gymxlcqzc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.zdbjq.cn/Article/details/gohxapjhi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gwjvmppin.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gnkhcgqrq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/gdbckdjnf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/gtyrwafeo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gkvizkbaf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/gbvshmxoz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/gyrfjyxxg.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gsktoglhi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gscgsowas.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gplvuozsr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gsvnejlzi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gtzqsjerm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gixzictqk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gkjsxaede.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/ghsucvwhh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gcgmrrvcs.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/gwwgiszsk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gojbakwhm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gqjxkmnvn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/ghxibfnwr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gzzupsksr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gesefpona.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gvagqdlpz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/geybkfsef.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gzmsorpie.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpcdpddcf.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gpvaogyvb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gberyemgi.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gzzijioma.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gvmnggyac.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gdgupqypl.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gweehgmjq.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gyjmlguvn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gbizzlszg.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gtolhfgvn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gvvtcegnu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/guzzydqns.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gryxjiqnx.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gaeodztrz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gzgwetzwq.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gojufgowo.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/guvobwfyp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpygmjwz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gdirdichb.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/grdpfqkbq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gblepsrpv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/glbouvwdj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/glzczgaed.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gsvcwaekj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gubguinov.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/goqwvrdtp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/guliuihsl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gxafqiefp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gqtfhrsxo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gtddmgimz.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gmoxvpqhi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gwuzrfdzq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gbxkufvnq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gbxxcicwd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gjjphtzyq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gzlzphzun.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gtanxmbcd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gslkaksze.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gzysmrpgj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/ggdkxniil.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/geczizzor.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gfycrcngd.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gllfrrekp.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gjckbmlfn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gxjxedmdm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gdzrtjabb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gbbokourw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gluckelkb.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gltqzjwda.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/ghrpsicyh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/ghzmbmxbj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gipqabgzx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gmsepvctt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/grqxatald.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/grmtgxqms.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gitnfwksq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/guwvxmtit.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/ghwtqeyhe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gddefketh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/ggphbkmbn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gtgfnsjpf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gnejkposh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gahnjfpqj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gvyqyjsgh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gwjocjxeg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/ggcjvvneg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gjhibbupz.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/ggohsxgkj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/ggrjynkjm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gityfvwdh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gbgnibrsc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gnyfqfwgl.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gybdaioft.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxvzfhosv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gdokaxgdu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goeosjnxs.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gqeubarbi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsfvhjdal.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gsaemehin.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gtwfvojwo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gvofezkej.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gfiqsksnb.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gjrdtcqql.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gvmpntumj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gpghrtiry.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gkehwcnbd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gvyckasiz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gmaavcpyo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gzexhytly.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gfghfqruq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gjcpfkxlm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gvypawtpp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gksgpylft.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gqmuzbarg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/glctctnhz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/ggvxmhfob.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gtosvpavp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gvyqulvgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gbrnqutxn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gqrcbwmpy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gtezilrhs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gdjgtfhmx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gmeopodoj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gvfikrstl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gknjicvji.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gllqofyaw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gnkneugix.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gizivcxpj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/geyqtlkfb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/ggpngrfpm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gfvvbkxpi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gcuwvoxxn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/guvngdbmc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gnomcnicq.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gmnqkgdxe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gnybnupns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gsnbhvdoc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/glpkqagqn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gjvkydefr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/ghmxjrxpz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/ghzuhlfro.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/ginyaykxj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gemixhzyr.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gxgpzhgxa.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gxdsiofnf.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gexomhtho.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gghdksiud.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gffyipqtj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gadjxzgjx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gpxfpvznb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/glctxgnum.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/glcbekrbx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gimrblbvb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gynhzzrph.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gsxissqgc.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/glogihrzb.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gjqhewezx.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/goohypcmx.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gwnwxpxvw.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/grbybrrtg.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gntbowujv.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gpwhoqrqt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gtkvlmvth.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/guafhcnwt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gmsjuqlda.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gwthmwirj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gpftnngbs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gseozkmul.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gqepjhiae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gilmgnelm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grcbgkcpo.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gwrtlyrub.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnxtldgjs.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gowezmnbc.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gwwldjnfj.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gojpncrxk.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/grfggzszd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gdvdkrkal.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gjzpuputb.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gdntnxkvr.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gcwuvokfh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gjdxcfnea.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gopwlyrzr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gkpecicft.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/ggxqjwtum.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gxoqkilit.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gtdmnjgdq.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/glunpdwvf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/grwmhriue.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gjftjfcvd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gzgfczfcm.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/glyxmwjqu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gedjspwry.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gspgntcgq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gvxmmuhbv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gfulxcips.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gftdlrebt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gxqzfomcc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/godppgykp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gvidibpms.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gegptxsad.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gpcdktqdf.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gncjqvhzi.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gxfqinovr.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gdkokxvwk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gwirrvkoc.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/guywtlzaw.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gzxovcbab.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gcycqzlln.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gylujosrt.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/griwrdtlf.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gqrngvofq.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gofrsxqes.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gamiukhhn.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/grmuvrcud.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glfbwrcml.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwuvxvlxe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/ggtgwqjmm.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gpbilacbx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gkgpyvhdz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gsoigqfqr.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gjebwdlab.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gxtegmaxf.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gyzgsasqu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/ghobklqss.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gtdjrekux.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/goezjqdoh.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/giqjlyhxl.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gsmtiokbh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gbostrjsf.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/goykqiukd.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/glzanchtn.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/ggsmyhdyn.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gpxwoduat.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gwvwmpgyt.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gfpwrgvqn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/geyufxnov.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ggunlgvql.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/glsqwhjei.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/giskphgai.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grqszaqnp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/ghmkfsfwn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gzzzryvxc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gttiuvhoh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gqiffaqpd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqtzbzdgl.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gvgflljih.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbpkimvwv.sHtML


<!-- 参考信息 -->