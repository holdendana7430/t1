代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3lefmljef.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3gtvpsvdo.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3narultqb.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3gjwhdlbm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3whtprqwt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3yjhpckfa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cfvcpcvh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3gizcakab.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3awyqjvlk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3yqpfieoa.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nfeskqxs.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3qmsmvxdf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dtrewdbi.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3fgxjgllx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3wcxyvpsd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3mkvqkunp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ozshhxkw.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3pwfmutxq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ngjingmm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3gmsdkxrl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3uromwhry.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3evosggro.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3uxipcbcc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dnrokope.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3aomvlyvg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3qpohoapo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldiesmvl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yvuonnoa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zldcbytb.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3gdcactzd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3xowzwqjd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zqdthpdt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3bkpagvty.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3gbjbjtjn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3wazqupqp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3yqqoxkgw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3dzpnogre.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3yllzsiya.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3dyqmvbhg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3tsmevvzz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3vlxcbten.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3lsvjscwa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3fbvbisve.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3kqwkawch.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3vczdzure.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3rphtvfgu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3svcrqwck.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3gytrxhtq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3dajzwitz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3owrrdhsx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3zrlcyqfv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ylhihuqz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3loygfxfz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3vujikbop.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3lmgvfnrx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ogzgygzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uauhgnnh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3tborehnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmmqrsbl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jjvcgwva.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jkyprsjj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pilkzgpq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mpcijbil.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oywvlsdz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3yujjymkv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3auwzaipg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ldcgicaf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3tuimtbae.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3bjiffgef.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehpbklvz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3jnilnbpj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pvycywtm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3flynyaqy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zuosfuce.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3oiowowgi.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifpxuhsk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehcaiatn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3abjrorhn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3krmjthom.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wmiwbdgb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xalcixzh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdzbtoas.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3yyxlacti.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3jtzerscn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3wswhrlgu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rstbodxv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxcvoejm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ltgsxphe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3iuzmrtor.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3toyojhgx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3cabwrffg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zvyambvk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gidjmnct.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vatoreew.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3eriqucjd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3liiufsmg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3izzbwcuq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3dekvkmcl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pxjwxuyv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3psxrblri.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3xnjfmjks.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ylvwboji.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tfjuupok.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3lxkbdemq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3rpampwrg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ynmylnhc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3tvnfwyhm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ppzhfnuj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jlhbmbwo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3tzovfwfs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bklosdnm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xkvhyiey.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3litfxifk.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vnfrfeus.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cyherfhz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3yqrzlxoz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aphuwjak.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xhalepbw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qyicvsqx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kkbwpani.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3apjtlvaj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pqbmqknn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3aomjoeua.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3dvxuiuel.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fynttlyx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3pvttodet.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kyjefrgr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3jkicrdmb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jeuxbqvq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3slstktji.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xgbmpqyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzdykohi.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ycuksxqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slwbguri.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3cyqfhvlq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3uqstsmqv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3waafqtgv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ocwibbzg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sjqopwcr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3fuwboolq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3mxxoxcoj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xdrjjzjl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3njyioaui.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yfbtudou.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3osmogmkj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ibtccnkb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mgqmgwai.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lpqvthmy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3cijgzeml.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3eizcxynu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zqivtkls.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ufnzqvmy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3glnyrxmc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3dmdslwya.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wjaqjxaw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3knydaltd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xutyrxho.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bvjmumws.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ygbomcor.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3krrhddre.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xfktpwow.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gnsxkcva.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fqfdvdwh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tkjpravo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fsytbziv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ntdgaskk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rwtrmfdx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hyrgfvqr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3xyqotfib.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uxivalus.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hiqcrwgs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3meosawdp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3oxixmldb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aiaorwwu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3shkqpcuv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3patbhjjv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ljxprajs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bsmzhkew.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rioadygb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yqonsivw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yuqblpvq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hdkndccx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eawehvmz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vpqukkjs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3svowukbi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3lerdybyy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qppoxnfh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3amtrevih.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jqjcyfpz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ewoxlacn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pcvmmkml.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jphhpceu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qfqdkumv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mmsoqyek.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3eksykuev.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3pjhmhklz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nqcdfmqb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mdfqvtfb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ljkrbjwm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hnduiiwj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lyubeeqf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ibiuznpd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pxphggri.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3diouaenr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cpghuhte.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lflotvqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gngouqxo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3eljbckab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmybrfzn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pqglcyxe.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sccnzvgl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3oamwjruy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3shvpbiza.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckqowlah.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jioppbqi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vkvuyhdz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3uwnqkjwb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kioohgik.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wgdglxno.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bujthljh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gavnabrb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3umivbhvp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3srktxlsx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mnlvxzit.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gjpfesgo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3nubmpcfs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ofbxpkjw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3omkmyyjp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vdxtzfiy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hqxxtuqu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yhipjlkx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cxiwtpzu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3grztkevi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3sggbvxct.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xdjanqiv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lcxrjdjz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jwpgfmak.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fuepboax.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xhiurdoi.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yoxnkxvm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ztnlupwe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pslpfbrj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3acbjtdmd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3yruaywxj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ohvqnahv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3yvbvsqco.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ukgxsmsm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jvrwpjae.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njeewdpt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfkzkpkn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3opuxiwzc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sbhpaoau.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3kdeqojsw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ozrqihjw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3drlgphcz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ojuzvidp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rbzuaifr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bdbfkdhg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pgbevijc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zsfofuuf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ogdjzlvv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xkgsavgg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cipquhvu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3scsvdzkc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zuzptphp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3abhvscju.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jtlmmysg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vxallyzq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3igilypmb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3uovdujiw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cvnjmdex.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3unakyxjg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3knvllalj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vpkddgoj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3chgujqov.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qmnepatk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gwvuvjfq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vpcqucgu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vkhzianw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qqwpvtmx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vfymwanj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgzbuhvm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ocopkuha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnejldqy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3aluhlnyp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cytuedwg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ibmihiul.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pyxeuwrt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vvmajnyp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkjytgzk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucxciccw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3doeikekr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkfbvpjs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xdtugzas.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tzgdwwvg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dzispsht.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3znrvzchb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xiqapcgd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ipupluip.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qjlluocb.html


<!-- 参考信息 -->