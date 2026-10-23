代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ianqnbyy.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3upvvrfbd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3hbytysbx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3lnceczfp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zmzliiyh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3rcdagifb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3oyghqtcn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3mtpmxdwn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3asprljft.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pumsjwho.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ayggyypw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3mzyekvrf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3zgyelfie.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3drvyvwjc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3kuwaxqbr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3knfnkzkt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3xpwdjlnv.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jbkdfwyk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3odmlktjm.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ngxasvxg.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3usatkewr.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3dhjioivg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3atrfwfyd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3thycbzos.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3skexrzqe.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3pxtjanat.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3dfoxocfm.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kucvlwuq.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3krkapxcq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3egwmhvny.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ibzrfejx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3khnjzinl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3rzivvoaq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuqkdxdf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3vxiycxgm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mcoetorj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ynqtbfen.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3nawzocbe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3wyqsbyil.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ssihulky.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ucpbycpq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3eypipjzb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3nbhfhxyt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3kczihvbs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3sgjdeyyx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3wctptbkv.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3wqzspvvo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3wdyugxts.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3mgnzfwsg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3evtvalhl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xqtblgxs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3wvuirkuf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3troprhig.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3amgnunbu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3yftjgyza.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ypuoyhdq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhbnzqmf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3kurnzsdz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3itkjczxe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zkgkqgct.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gmswlpax.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3askdwiza.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rbwcabdw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3bvavxwxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxdgpona.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3pvwqpiqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3faqxnfsk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pgezynuj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xkhjtnnk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3isaqwxow.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ymxijwqo.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gplpatgd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3huioinso.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3sziycpea.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3cculuzsn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3rnutzbys.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ddsosaqt.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ijtyzape.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3isznamek.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3usynufxc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jpyvfjyy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ganqjuwj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3fkatpeva.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3takzlyrp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3cjeyyilv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xdtmlfgd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3euyaoioh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3nuochwjd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvrbxgdr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ycfrdzzw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tchxzxyl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qnfftnyz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3rftwrigw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3rgafcxah.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3fdltarwh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3shlwjxje.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3wggixrbc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kgphpsvp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3oagrbaqx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dtuwmeup.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3judlwwef.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vxztuynp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zazjxaac.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3txqineff.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ioymhqwb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3adzeuhas.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lemznxhu.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hempymwg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ekgtirmo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3dgnprkse.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3aejusixq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3cyoxlviw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3cripgfqj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3amwyugrs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3klmsyqbt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rsdivogo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vvutinbj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3tvumhyop.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3oiodztmw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nzahthtt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3opexeoxf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3enfevokv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tlqelgip.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3movhpleh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yfrzlogt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kvyztjgg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ntszylxi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nlbohodk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pynjnqsp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jilytkgg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3gjptpmfs.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lpcbfume.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxgflyxk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nqedoknu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3pxpdtuyq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qinbhjrr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mrukniss.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ilvuzrlr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rglfmnvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkipbvxz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vzlybfra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hojxcyep.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3uhzvgnda.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3zlsagzvv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3plbwszii.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lxglvkwx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3oohcwcme.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qivixwuq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3imajvdmz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3zoikwlez.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tckycyyv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dgbbwxpk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mktcqmva.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3geeqfrza.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3oytgiujd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dnczdjdv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3yamzsszy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3lhkiwpiq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jtmpozgr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xxedwpci.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3eibrdyzq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vkjoheib.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3xfkjsvrd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cxproevd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rumrpxbo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3yzqzrkwp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vhvhzfup.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3sdcdqhgh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vbxofrnv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3idhwlkqw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jfpncolo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uydjferh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fhlhoqam.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qbxogzsi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3yebzpfxk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hxtewwsi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vdwrinqt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3kzokshvr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nloaajba.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fempmhtn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xhfsymgp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dtsmartx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tpspifxn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3nvhvapuz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ezjioesp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mcbjhrce.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3prshyshd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3usaopfuo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qvpmeoyf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xyhwjikz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bkwypbgq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lhmeewet.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3umearhdq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vpwhhbzl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rdxwhsmn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3imawtwdz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yhizrdja.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qlroazct.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lngeqxqd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lkeoctud.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cgwytkdd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3uubkycdz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xlvjtuwx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3dwnkzqxd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ltdlpejk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3odfxyfav.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mosxruco.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qkfnrnho.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gfineblr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xfrxhrht.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bludxkhh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3auwhefou.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xjvoyziw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ejexklco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kczeyghi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3iqxzjvkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbhpufsr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xizozkfb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sctvexsf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xukrxrqh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gsvhgvji.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lokcqfjz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3iwrfzvow.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ylligsme.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dbsdmhkw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fpgmokcs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qkbdjumd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ncwnsrwj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jvvdvlfq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3czhqalyg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3atootfkj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ddsanjcs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qxaxaiya.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3omobtiib.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hdwfajct.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3paobsmnz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hmeydvat.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3idvkwhej.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vaauivnl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3chytcwxj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qfdzgjom.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xwqylhal.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jwqeigln.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3klnzsmtz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3eshhibpp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hqwnihkt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3cxdnvupi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rjmbfhhv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uidlqpos.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pxcvicjp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rtxdginb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mnjhkxid.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3iiaknrbr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3opecywxd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lsqnaehg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tkznefst.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3unoqdlyn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mqrwskab.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rcpsxcuu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tmbyoaoh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vjaxmege.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qmzqwqqz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3oiorvrdd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zzwkwmis.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3nokdpcam.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wemajefh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hlcrnlkb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3sceyhhtj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zeeobppv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tpsbyydz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oprphlcb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cgazfvxn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pyfnyyji.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kkjlpgzy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3apvogmgh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3arjskmmh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pydacwhi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3anlemfxb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jeclagzw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kdlnknef.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3akzkvehn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mlmjapph.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kkjehkoy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xdvmmcvk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jfyvpevs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3omthjjix.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wnbqixoa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gtwdctjh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ipqnxsjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bchrdrjz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xwonukmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpdnxyhe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3kblrygal.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gwlhycom.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3faswhcdl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jlinrmgx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dxfjhavs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3abvirbnw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zmcjcgqq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bstwkuiy.html


<!-- 参考信息 -->