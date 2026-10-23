代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3tgupldez.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3nurzalhj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3scyqgfuq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3thdktbwq.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fcobkqof.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fgbwhqir.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qtczwudf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xzoobgjw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3rtyqmhjv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3lczdegjc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3bqciklgg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3exjpebnm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ujijetvb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3myqjucii.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mwceaibw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lscglpuc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rcjmiayc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mivvbcvm.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3aklamree.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3bzigdpgt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3pnotgavx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qltwdelg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3oxztxleq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3egpjjoou.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zosuapur.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3uosflqff.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3diochrmw.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3kxrnaxsm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3gpifvkqc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ksdfbumm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3sjufpfqu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3mcbljcvg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zlcqcuft.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3eodtbqbl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3nfgelqou.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3shdcrcom.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3qtuapunx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3elznkdnv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3mrbvrism.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3njtlacya.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jrokxbfp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3eeypzumc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkgnftjj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xmfguhde.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3athlekli.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3lddrpcpi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3gubmzsdg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3lepponsy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3iqzxqatv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3sidrrdva.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3zgxgkdhr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3lequgclt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3yapudwjp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3jmgiqgrt.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3iyeqyymt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3gokpxllf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3sxgapjod.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3rxblynkj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ublkrdfe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3fkaxlcfk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3gmtyokjg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3epckqkzo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3yvouhzvw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3tkcyqhwb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3jwqrcmvl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3dpgfwprd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3cyetrgej.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nmplxwbk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3sigpcovl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3uebmbqoa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3stydgypk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3hsumalxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbloftwy.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ecdbbrbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpcfyvjy.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jkudaexr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3uajyunhp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sfmkjmem.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oaupensu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gmhuoymu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3tgvbgjhd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3dliyppfe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3clihkjws.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3tumcwcxn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3vopfkwgx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3dtdiudsv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3xftkecry.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jzjmmsry.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxpqfswq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dxwduvjg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3igdxnljt.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ovolrsfa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evcmclhm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3dqeqgwqg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qxvckgyx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ufacowht.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tqxhmwre.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qpipsdna.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3hkhblayv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3oarqndaa.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3wspzfxwy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rylxfeez.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3qdlpvtxm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gehzsftv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3khaigmey.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3udmhcmit.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3patqwzlo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3iobwrifz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3iesqrgyr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gatgvobh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ccnycbvu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3sxfvkkjn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gvjngtba.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3lvkubezl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mpzowckt.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fcoovver.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3pershshh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3showedcp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3grumplrj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3nfpgjhzg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3dmlntcsj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kpjtxkup.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3bzjkbafd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3lwcqdbxk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nmodeprs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3yupaldqw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xsleusvg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cnhpawpt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qqusvnej.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3wxnrutto.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cfrlaokr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3topxejzt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fosktkpg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3prptvqxw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sefxneqm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3gxvtdstx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rjdzusft.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ejnanzro.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ufadrnlk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xyzxcthu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fdrixjzn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ajckpbne.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sjexavge.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3tmlioisn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ixmfknzv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mhtujlbo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rrfejxrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpzcqyww.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zhgftkub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgjagdso.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ucwyzzax.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3uoktwxlg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3etoesrdn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3srdxytep.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ohjiyyga.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3jrsvbllo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3tpkcrram.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3uemekixj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yuwghjdu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mscjknrv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kcdbubav.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3rtpjrvmi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xbzzuvdw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ewguwygg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3bylyfosr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vpummztr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qoxibmxt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qalcgywy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3uuppzqop.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bmffjuwa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3klckqpch.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hqytfvgw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vjrwakfe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bducgfjb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3aomseglg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gejkzsxz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yjhzehxx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3wnvuopco.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ttztlfyc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rwvmovgb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tbdwywjm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sixwekpq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qotftfbt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ookxjpbi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3keodvdft.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zhyaxhyt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kogterpc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3eswebaxx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3dsiinycm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kvviaguy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3oaesabyg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3kdkagcfr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ajqilofn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3vyruebho.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xsfronjo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3zggftqgz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3drggbqmx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vmhywfll.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3evyvdzpo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uuimbxvp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bwubgipo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vbwreumt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3pbchyvni.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3yzltqbic.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tmsboqvf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3rtmcmuof.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hqjnweas.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uihfbapi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3syrzwbdc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ungbkvrv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xhsaivyw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3beclokxg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3frriovkl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3zjkzjmkg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3jocurvav.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pweuvlfo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sjfqcnay.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bunburiu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rmwyuerk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3jmdqktxe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dbetujoy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ebugispu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmcgrhgy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3cgosrugo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cltvmgag.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dnjokozi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vpkqkxtw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3lejnvwwx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cigjmbcd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oneictbn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gwbjhfwc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3yctairmy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zeafytdj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vpahzuva.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lddiygxr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3apodexuk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cydtwore.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ltsrlopf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3miffmhqa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jbmcixat.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3umieadeu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gnkndyjv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yqluswqp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nviwgsis.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3denfnppv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xpemminm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3imalnmol.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rbrmniqp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3oxmdraht.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qrvilgvk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dzjcnwrx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ylsqgkmr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ttejyrez.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hejwxhrg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mjsrmyob.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ephqyegs.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3whudcpar.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rpsrknrn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3liitcabq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bnbncyol.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yytfdiyl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vdqzixsw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxrlotmk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zkqoevlh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tkehcmqc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bwugvfoh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gorwrwvl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lmamuvrz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bpfjpvep.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ixycdrmg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mxxwwlps.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3oihofzqn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3edbcverh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wrlwkmmr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nyjnmneg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3sejfmjfl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lrmzhcrl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3oupiulrk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pdtjkccz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3oclnzbec.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tqznbklt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3haiypelm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nhewmiyl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3orrmwldf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pbikrfat.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3aqehrhjn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dwqtwwsy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3pvjfxeef.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wmdgybln.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jluwburq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nqkmfuii.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dngohqbk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mxprmnbf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3fogivygk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3egucmgka.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3bgnbgrmw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lccohirq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usvfbzhn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3jsjnsgql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhclhthc.html


<!-- 参考信息 -->