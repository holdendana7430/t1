代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3rtewqeyq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3aoqahrge.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3hoivmegy.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aiivntpx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zyvdgsjf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3coumuayo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cpuzzzod.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xuxyxnjr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3kfozwprc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3taxuwcvr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3umksotja.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3qbazygdy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lszrnabg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3yybaoabe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3hjgggqjk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xshxlyqf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3svibwglz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3oorthhae.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ogqnlxcq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3czzkkyam.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3oxwruztt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3gurwhkae.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3tqlxicdt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3wyytlnyo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqeqmsg.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3nyjyunoo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3tbaoiddb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3wdvtrlvp.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3gvdxqxvc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3aczukwfy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3asmuvnik.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3nymjyuhi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3wglvtpih.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3bochnamj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3qvdzcxin.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3rwopnnxe.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3tcqxfnvo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xkqrimrp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3caezuteq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cyybbxso.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3iupboyaw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3dbldzumk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3rdmtdnbe.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3uuficqye.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vuezbzcu.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3pziqgsia.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3hpqxzjrh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3wvggptwj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3jgnpjfak.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3kdwekepj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3qbnzbqtw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3fiaqphnf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3htrhhhqi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ysimsedj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3hipltsjc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3fipzqksn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ckqizyxd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3dcagqbzb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yfszrfpr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3osixwobg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3odlbxajs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3mikyxzdi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3rjwaduba.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3dwpsjlde.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wraxjbuw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3czuerzdu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ybeozldk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rklngndx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fventpfi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3hglllkjs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3iaksjmgm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3zbxmneib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgjmzrrc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ljuuxcbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aikuiknd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hccwssay.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pktffpkg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qbbeskpc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vpbjohwb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3uaipcfms.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3emtogwkj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vnhfccpn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3msrggtsy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3wybmntch.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ngcydejf.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owuygdpe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3gscichfj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hnooufah.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qyqaistu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xrrqcojj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dfalrmsk.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mdplzzhl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3muyrlmdc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3hgjljnxc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3rqbkujtz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3swegzsiz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jajdambu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3epqkhrtv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3rknjdwge.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3inihjvwb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3sypsmfrn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3pbpclggx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3jhcggcsh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ameexqqe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3zuflsmpb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3cmyimzuh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fayloecc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yzefdrgl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wfwoksch.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3eoachngj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qlbnxobx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3vyyxzypo.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3nneklzou.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3udyqfvwb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bpoalucj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xatrlirs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3vodtnoiz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3moqslvly.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3skrbcphs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ixnbqhat.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3klwuunom.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3huxvlgzy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3wvlcqbnv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kxtstdue.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3oxvuktzu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xumgnwiv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pwgynzux.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pzzlvevy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zxcvebze.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vyoobhgh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mbfrobzb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pzpitonr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qanvheta.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3afjkzzup.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3huolaeyu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3crcokwve.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3toqjkaob.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ayvsfbke.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3mahvkgae.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3lzrwhygz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bebzjila.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ecqntthh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vyzbzqnz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3nlyvmkyx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xssvxpmr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3yihbimcs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mmkshhjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hczjnbxa.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3kvbnlyhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlporrzl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ipaleuhz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3khtejnrm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3vlacojhb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yjxkotcm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3eppssnvt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lpkvfsru.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pxvdtaqf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fcecfjml.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3yebkkiyq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pobdxnfq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3splfflog.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3abczlink.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nvqyjtzy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xyeuuktg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yevxolce.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ekjgzywy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wdymqjmy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ojhplqjn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ggedmadc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3nlmmhsqs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bjapzunk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3atpztnob.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vbgwsbma.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xlfkfrrr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cbhdadwd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3mxjmtmam.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mztptgdh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3clbtcmuz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3plrjpiek.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3grulygre.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3okxohudx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3blrvvfpn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3fferbeni.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3kvdcemid.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gvibesge.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3odyzozoh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ljoizvys.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bzyestjh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xpnprihp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ucirgiso.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3muonumos.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ogobrcag.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3viezhsyb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3twrbccvs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oqxabnkr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qicbkizx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tiketemq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3clauonwe.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pberaojk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3etmrnmug.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qbeuceyv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gyjjqcfc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lqxqtftx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3veapywmd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eduagami.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3euurgqwh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ndreprhd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eiajouqj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tgvxiuua.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3msndzmaz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3prwiggyw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3maiamjue.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ghvosrwt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3azxkobty.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3weusvxgc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3izcblfke.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tzebrkiv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3unupshmb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fnpxndol.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bwcnwbpk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vufugkys.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jzqpnccp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxuaovrz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3livpjgxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enihzuux.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nxsvvopr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jsxvwewb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3afthdviz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kuwsixrt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfrhzuin.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xfbtfwtk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3maumzpjh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qrsdwzhx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mzdupyxn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3optualxm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cowmppce.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dmirnurv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ybqpuluz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nizyuzhr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pzuqiijl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dzoyhcqd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3kcblildq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dqzzcynh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ufpxozpp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qzlszdhs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3yrtrowff.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ctbnlnuw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iupieqlo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3sqxzpczg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3smeoelyf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ufzoatkd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3liyjelcq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rxbupxgy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xihszehq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ybtusmgt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3boorjnqa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tgyimkvz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rzjjxrco.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dovntdyw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3irqpfgip.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3sahevnza.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hrephdzd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wuzggnmm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3erfbkdzz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pzcwnice.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqnxtnqz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yxafgrpp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afwdkmne.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hjincnyl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qenjhvto.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pqcodrmt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ulniyfrq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lxwbzqku.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3beodgwyp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iglumgea.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3kijmiyyq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xbkqxjgj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3whjhqvyw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xftbcteq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3yafsbeqg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kwwqvmzr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gjrotdtb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hygkargy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3usssdvlc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rxyztbdq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3aljsvwch.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3tjusvgae.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3swhffpoj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dbwujdhn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fttwntwg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3qodjakwt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lclghnhl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3phnthriy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lglutzci.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lqebpfjw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3txiscasc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3akjtgfwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmgskjcv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rlnlnhen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtannull.html


<!-- 参考信息 -->