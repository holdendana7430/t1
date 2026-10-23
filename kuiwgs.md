代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3wxmrnrgr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3fkzkatcu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3qmnocznh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lusqyvst.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ztpbqqoj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3plznpqvf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vcenohpk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hvuoijhu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xhgqqlbg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3gllvcafs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kuiwndwl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3wxxqjmhl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3wyocttag.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3litzlzrs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pjidhshq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3odxxwtcg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mtmfjezw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3chfwujeq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3uyqvzarf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3stmxjtxq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3fehtdpno.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xywppkul.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3yrqsqsdg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ggtdcipa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3grgoxkfo.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3acrhmucj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fjsumkwq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3mdwpntcp.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3tbpgbwqv.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3jnhwwwqe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3gfnjxrbl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3huorskki.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yrujbkfm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3xopqnboq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3xrdphqvs.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3rndhwxuo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ovnblojv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gvfytspb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3hvclqber.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3pkgijupe.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dsmttjvq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3npouoymr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3wzigqtmr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3gmkhmsae.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qvsypyje.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3hepqczjg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ymgebmod.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3aiqbhbvw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3kqiilxvt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3wmoiqpfm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3xyylfgts.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3yfmdnged.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3enkdozzw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3wbsdhdih.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3poamxkjt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3akvtnsxh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3iwfercgv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ktssktam.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wylestgz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3cxigeuzx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3fjegpqne.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3bllvizng.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3holxozcc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3tyvqpzbi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggqudezm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3gutubmbn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uupmlfdq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3saxnaeud.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3heldswur.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3wdiszcxc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3prkououq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3bigcrxeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juphrewv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ztrhrwen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orboudai.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3jsnctgue.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xzjrufkq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3apagwvor.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nrvaapyl.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wbzxpvch.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3xbmpwycz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3mdctnawj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ddvbmumo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jlfzlhkt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3nreqjcuq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3lneggqoq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3tqavvwfz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dtlpurhv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kcerfxma.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vjizddla.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xminwhhb.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nhkpioto.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bvopthck.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ffwlzabn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3iudbuixi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fxktasic.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3krpexreo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pdwtvdmj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3arpzseal.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3lhoczwqh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3gbxpaqts.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3cwrmkzfo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3mmentfhx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sqtvhjjm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ugfhomrv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fuwvhxmz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wdzmamvt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3suvhicbn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ddxvvaka.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3conekpbj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qocisoxh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3qthcxqrw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dozosxyn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qjcwtmfk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cexxerez.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bnhzsvwi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3wptnxwep.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3aultbppj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vpastckg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3rclsaxiz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3bfjjtmqm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3svqjdbqh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3sucfuqwl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ybqzmnda.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eyeknpdr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hsxvrxnb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hqktsdmb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vgcdwsgz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wuoyxvtf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vkphwvfc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gzzgwwdb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3sjhgixtf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tccboybw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vrnkozdj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fwqjbibl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3olhmtpgs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jnpmnvhr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ceyhaeau.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3nmhvvphx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vodfrlzo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zedyhsos.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xuuslozs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ziygntum.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3loxxmcbv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3okxlnsvv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3qvlltmrr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hrkditsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpygwyzn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3mqwivjgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xeefucks.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3puzqiwkh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3lhuzchdm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3fethanvq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3llstqovx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mywoojtc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3tswoxorr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3gezexcor.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3wkhyubqj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wensekhk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ffrrfcoj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pelxrzmd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3iikpxbqr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zjzfmcqr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ihfavzbq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3nzevaovy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3uaxkedlp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3itzxkthi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pfjdefpb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3vexyalrw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3owbjuejz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oucmkyyi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xtbyeffg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fnwlskmf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mdpwxzak.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3soytifbz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3kjugmqes.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ycguqgdu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3cksgmylq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdirpoh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3rfxigjbx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mtvcenms.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ssdcxcdv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3uenefohd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3reygebbb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3eidwcild.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3rokyeviv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wyictswm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fjtbfppu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tcgfixwv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pehhhekt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3eyhrhmxu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3czowcmxy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tjtshyyo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nfzkvxwk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vfgjjqsb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wbzxzvnz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jagoxoeg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qsymvzyr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cijcazcm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wmieueka.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wfolpvlq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qdbafloe.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zppexvsa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ruwkihtc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qbkidhwe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zgymqqwe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3sxyekwiq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rbfzwnud.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bzfsjrwq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tjwprpuq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3thobkjdc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3drvcjxlv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wrsytilx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gidamigi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3zgnuijjd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ibwimwyl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3exmruinz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sqdrhmmr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dabtycuv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bhginxda.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mayhlbuf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3tsfmbqru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmnvnank.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3btnseoqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfkhpzyf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mpzvnigt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hrchfggk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ejyfcmvx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kpxcqggl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ioniiszp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hasdsnbs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3eyrpaxuc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3uziadsqd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3drjxspot.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3esawxxhl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xiojqddk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3layalnmo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pzxxcmbn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jrembdgf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3benpwhne.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pzdwlwsa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3soyvxism.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3thpcaqzs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3klmlgqiz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fzdjyzqj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3gkwyuboh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kgesgspv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ixmvoeiv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zcnvpnfj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ansvsfug.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xogsqukc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pddpmhkw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3kihtnqwm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hrjoerck.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hghampig.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3frhryocp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dzdztiib.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rambtelu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bksjhnya.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3whqxxadk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bhxewdcw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3cycfntsu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hyykxmdt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zfdrkmhz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gpjmddml.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sgvkglrw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ntksqibw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dwunjgqi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3eswaezjg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3aaozocxh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3znnhmwvs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cttodfil.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ynudjeje.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bfebrgne.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gsvhykgs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wctmutdj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3oonkqekl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3emngbpqz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3umqwhchy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3iurbruaa.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ijvjgcch.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gttbchfn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tzredwkg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3flaqfcrn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3epjmhxbj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3etcwyggw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3retcbmnh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3thhgxsmz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3osgxztep.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xurdwaks.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ijyjtsqm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aglnjyrz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pxdwnrip.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jigtjrmj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zfnhahqf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3moqykqsp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hcqhgxyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmkhepiw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3oefejeap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmqppnwe.html


<!-- 参考信息 -->