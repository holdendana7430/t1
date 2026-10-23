代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rzyxsoot.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3njvyusmq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jdldoagc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3sfxyjnpa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3tjrtrpey.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3mhhhqngh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3qfnbzuml.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3qnpcteiq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3agaaaluw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3yshontwy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3fpjtugcf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3coijfsag.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bbyktbab.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3aesxjqsf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tlcdxlab.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3lfljctxp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3gzoayyfm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ldaygltg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ekaqaplf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ethgifdb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ztphjgwb.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3dxwxcvaz.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3qwdegvkz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ttckieqg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3xdgplpbq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xrssulcv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3iimnehsa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ahlmeybl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3pkoiaprn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkdbvlyy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3qfamurda.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qnctrfvo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ooqvdpov.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ikidscuy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ptolfdsu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3vkocrvji.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3urbcqzkz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3pgmlwgtz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3nbeptfbh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ztigisck.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3wvjwvlnq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rjnvxkqv.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3xwywfqkw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3afrqhael.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3awqoltbx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3cyvubjwd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qcpdzyhs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qugvgnij.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3assanlmm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3qpmyvbrp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3yxjvfqoc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3eolmxwkh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3vigmgreq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3lxtcldqr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkyrkqo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mbdrfsef.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3xmhnuukb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3emvetrzx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3mhambayh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tggrrqan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siczvnpy.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3zfpcdkji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmlkaixl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3saxuxjnq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ssgyugdb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yfpvwndv.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vptgtaqj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xeftguto.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3khkvvxcd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3htyibsiy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3vrrajjam.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hypruayk.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3jhpeeero.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3dthvywgr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3sieaquuv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vjvhxzqu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbdeinys.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gseatthl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3grmgfggw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncjnbznk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3nmgfcuvm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3bleyayfs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vbarerpc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jgdkqdim.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3usnijffu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qfcebxhm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3myycbkiy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3pkcvvsyc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3cztsnjgm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ukegvpfg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3nkrmpgls.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3qmhasvuq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3pmqysweh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rjtdswyw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ynvnobzu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zecfepwj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3efgxlnuu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hnvkgucn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3npipytcg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xaujvbrf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gfbidlot.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ceyhflzt.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gfbjnmuy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lxopazke.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3fykfnouj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3cmcuntwk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vctvfwrm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3whetkenn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3czipjpky.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ousrjyll.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3oasgnwxr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3uyxanjnu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ziyyfmet.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3adqpgfgl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lqeuizqa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fgxssfez.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bovfrskj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3qtfzbcew.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mdalbwit.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3cwjqruzw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ifjuwgoc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpqcpya.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zmkyuodc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3tarnvumk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hrlqdooz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rfulxlla.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3dfzsqtsq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bnqylfsy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3odamfwel.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dvgskamj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mdgcydrf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ojwpunso.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3zkvpaqwu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3hrgsemij.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rqrhsiuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bolwlhss.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3glhvwwit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jffecoop.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3sqdmwxyo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vmojjlez.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3drmstgxc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jkgqruio.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ukfywckn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3txrcxbmo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3bninbbgl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3meiqubrq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ojtnwhll.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gqngbpxo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vwdjdpfh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bnuadqfg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3croaoqhy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tjwpfzvm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cubujwca.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3zgdszmbz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ftrhhejc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dwmnygzq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tljzmupz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ogdpkobo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3mhkdfzqk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3exrnfvvp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3stvekpwe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zdhkwuwo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kimdarkz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ropsxxgm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3btqatxij.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3iabvylav.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pseohmcj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3afgufhde.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3usfgpwys.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qipclbvd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wiqrixhz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3onipdccc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vyzneyuu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ugiuifee.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qovdykeb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ioskjgjx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3btptnqev.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wzyxyqxx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yjxnwbwp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fydizosl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kaiwtvlr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3cowggfye.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mevidnsi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nrchylva.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3emxdjbpy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3aahcboyo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lduoxicg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qrdmnmux.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gvvsvbhu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vrefzeit.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wlgkkkgz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3yikaptbd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ljeyqviv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hgzaqxic.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vvucqzjr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fsjhvaua.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zusfohtb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vwxmreow.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3leqlhxnk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ducdvvar.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bxddcarb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hvdnlpeu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3uwyvmlvg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3vucsllqe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qarfkrlt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lwoheozk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vysgctss.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3fypgoujy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rscgljlv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3tprywoxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssjtzvjl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jfsndclf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsiylgoo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3arvdxmmd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tbhhkykz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vyvihuqh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmcglztm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlrcwcob.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ynqjhhrw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qyurniqe.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3hnmczjvx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qixzjpca.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ljcncrrh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fsnfocsl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yejqdzlx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cbjdpujg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3glrtukif.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ifdgdqjb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sthxoqvw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3lvzhtiif.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3coecdubi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vfaimncj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3zircjwqe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xjweqtxs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uyulsriu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jlvleguk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qrdanngj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3emheiapp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3yhaklqnw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qpejcwji.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3tohdkpmx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gfhooede.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3labgjqgj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3plvzrfzk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qlmnjrkm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3dfnjqxdu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kcopgtrx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3acwtburz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pwgjxrgr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3forbkhmk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhrxzgxr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jjqxlojq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uyzewcip.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3igrchxal.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hqlfqkjx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqgomqvl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hdkrlspx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rmnpcwcu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lrbulamy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jddmrbse.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3dpqfojuw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sbvtuhhk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bynizsrd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wjdhrabt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ecczxvxa.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hacsofuy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3namkbxlu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ievpfujv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nwoppovc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jxzfojhq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xeudfypt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qoiwrphl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3bcczwtyt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xdvgdper.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qbndudpv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tivcvxfe.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ihgcrqrf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3blkbyqew.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3saovtiiq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dcsktmyc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wjxfmukx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gjfjjiux.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3pwlbibhb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3antaktjk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mecmygkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvckttfd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ttvqrgoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwgrffmm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lohgbomf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ctwkokqs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3maguossr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wlkqnppf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nxxmwpic.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ynhbsaqk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xouryszt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ikinnnad.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ecyurjeb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3smeeaxqe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lcbmwaqw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zhuzbges.html


<!-- 参考信息 -->