代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3jsmmawzj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3cszixahq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3biipkszw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rsyacpqd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nblwzivc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3udfobwse.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3inhksgad.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qcwqrhfz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3cyfjsbft.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3dfzppovl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nhhokdrp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3gcdodagx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3swugeyvd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3lzwbpgcn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3phcuntva.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vomqborw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3qxseuuqz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wyslxnqp.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3yetzphuh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3wzkyieip.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3ziwbtzul.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3agjttvln.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hzxbuoib.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3bdgihblf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tbtghjcy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3eirxtgus.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3kwrrsujq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3uprpshal.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3akgbhltn.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3qfatithz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3knjctmhm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3fpupytln.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3lnkfbpzi.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3fsnzqhif.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3nsayberb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3znbvldyr.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3bswyxnqo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mwuqyont.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3iftyqrau.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fthpumqs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3outdyzof.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjvgehhn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3gexasedo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3chdrquaf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3eefpiyjf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3znwyulnb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3bdjhocxn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zcfsqlhj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3zolsvlws.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3wtcspcdt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3uhnczwht.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3qlmecogg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3tiauvkmt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ppaaznaq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3nukkfyjl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3bgzfomyx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3jezlrxei.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ttotlerx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3oykinssa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3jbhgdmib.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3syofglmm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ecudwosz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3hhhlzixb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3phownief.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qkvbvank.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3buyfcady.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3agoowmdz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ovneicwd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ilwpzjte.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3igovazru.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3esblvtzc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3hevnkzqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsumkplu.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3rxerzjjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqiffkcy.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3hqodqtnm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gketmwcj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ummguuuz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3psalnwwc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nabnjeuc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3uunlvxzd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3nbommocx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3kenqcjee.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3udsksvfp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3evgksmsz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxavsbdd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3iqbolwie.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3babppwtz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ckelnosd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ihafpktw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zumasvpa.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cekbjdtm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxigwljl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3thjrkfii.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3txlxfpdv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ffxnmubh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvejmxdm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fsuhqepg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3zvlouyba.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3vmxstnkn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxgfqwg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3osfrefgs.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rfaqfzgi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iylzquvt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3wgusqctu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vmqfgsev.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ldywgwmr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mdnjaqak.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3pawlbadm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3phpowvua.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kslvuamq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3gskzrfrs.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3iiyuyxkr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nuvpdotz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oyxsfysk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yudijmnn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3zixjqvti.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ifyhlogc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3axykeqiy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3mzgueimc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xvevssri.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3srhrbzcp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ectiyqxk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qjszbmwj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3alobfofz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3voymnhqv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3aljripae.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nltqumcl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3flvgkdjb.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hlxklpmt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tfcllisu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3hefvgovw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rsapxcho.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dzoehtdy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rjjvtavz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wwxdqqdq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3yuytfxpy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nvbggdmy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3niabwmwg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3jytehorh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3zmuilqga.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3avvqyeod.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3clhqsjyj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3nxwhdxej.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3cvhcyqhj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3pykjesbw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jrdqqinl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwxrsjgk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3gsomojbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmyxqyaf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ezqgyxty.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xnpxspag.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3oqecxlto.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ecuafpcp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3njyqgtkx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3dtarlgru.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3urhtbtyd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vuhjpycf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3overdgjt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vmqlibdx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3urdiezze.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3geeiqtca.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3igisajbb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3foqjnpws.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3xzhcdqqt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3agdjvvtd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3pijhvzrk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gzpzaveg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rzfqdgwx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3haymncxi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nyokwmis.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3epulsple.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3epqizpzs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3fmxqeqcv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jwzrpfex.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3omwvzdzd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3amvrnpjf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gpiqqoaa.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zxofnhyo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ltvhzymi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fbmuzatx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hmsdfheh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3linhkelp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3rosmbjgi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3dtdklols.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tyucptun.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nwjbrvti.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zfotjqrf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3clgrlvid.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jehqsgdz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hozesvoc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3iuxvvdel.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3lctdxgcv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3dcbbirnm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jmbmetxo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gvfclnvq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3crqwirot.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bmakbbhx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tizzgaqs.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rnntjpnr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ylcjyitx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bleldlyw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ujkbalwv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fzzxswzz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3axfimvns.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3khgulzis.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ynkkzfsa.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fkhikhln.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3aafdzain.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tfxaqhwj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3terkdzpy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dafjjvab.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sgopvlqc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rpoeijuq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3dzsahbya.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3iqogactv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cayfiqlv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hbozcpsp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bshxtqtv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vrcblrdk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dsyttlej.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3uoslwfoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uopucqdc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3wreyuxuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abtcjvcu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sixykhzo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gcswdupd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3dtpqmhof.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3byocwfay.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulurqsey.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yuimxfuw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3erbyzycr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3abtulkbn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xryttjmn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rbxkwhti.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zwkfwcls.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bxezfnlt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rkldylev.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wcidxbng.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mekegjhn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ftssfana.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xiumligz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uieguncv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fdilduyz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yftwirdp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fecamful.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3atzyjhoe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xmrhjepv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zubyvtxc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3smcypbng.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3msbwfnfj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tbklowcy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cyeqakpz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3cumgcyyp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3glkaqgex.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hlauqldw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hhosmixj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ruurafpt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3acsiecxf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3orhjqzfd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3arpwusmo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wkyytryy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3isfhsfuw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3saxgtbjd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzneaakf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcdkmktp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qeevgztn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lahxbirb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3biffjyfv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3iaosarrm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3covhzzwd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kqunbqpp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ljpdkmnc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nheysblv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wucvybyu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oawwrvfk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xudfdnwi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3giuywasg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hpmptkeo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ohvxcdiu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mfamtyxw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ooziepvc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kntjuwxr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3miaqyzje.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qvuzrzcw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3esdgldxj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lfqmypii.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ggpdwath.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jiumoage.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dxuuwtys.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3spjhfkrk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3frbxicvk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hqpeqeou.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ywooftth.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3bbrsznhx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3eousfyhz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3tdgslfmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byqeloxh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xrnpqqdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iliagizl.html


<!-- 参考信息 -->