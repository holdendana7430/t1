代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3qdmivozj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3zsdojipd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vbsxwxop.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3cvdosuhb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zwejbkiz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3yxmrerbs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bschbogv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3fildfxlv.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3auvkvxhu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3tyyoodqy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3jrsgxkqn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3rocfbhdd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3hppzlajv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3lqwqkuyz.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3szcfnkai.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3bzuifcuz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3gqpnmyol.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uuapvwjo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3meusjjfa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3lxppjskn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jrsgyjzm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbshwob.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3jtajxvua.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lvedmdzo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hjqabizf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3lyccyomr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3derlmwck.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3lgnpjgrx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3xtrybkvu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3cevlhrkh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3phdtioeq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3efuosfgz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3uredxvol.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3hddjrkhj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3imzsvves.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ikupyhyj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3bjyasoca.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3olrjwaqx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3friyxhev.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3qfplzicr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3xptoaqmd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3pdjsoftm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3fpmahhhz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zwtoxlhy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwcvflsj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3igvlmuql.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3rywnqsgl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oephlkij.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzicmqdb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3lilbanzw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rwyubgkp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3wevozaok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xymqgqrr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vjuhspgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuwuaibb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ozsqbvnn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wbqphmvp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fgsjbzet.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wykmrvad.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gycsyhki.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3imecwegv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vzvvxfak.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3teptwdxn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gexbshnl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jnuteajk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwhwdrii.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3gnxzitsn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3csmebwlj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmvppsbn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lyjatwsr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3chbnkkpg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3obkvqfwe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwanvkae.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3bqlrsyjh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3rwnrugvd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gtfnwuck.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ezhxuruk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jeumeapo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3kjanzlyt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3vmifhnia.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jnlcphvj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3unzbioib.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3mnrzqvdq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahwohosx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3iuilcncd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jqusyizp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iesxzalo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dduhyqzw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kueqsezi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3uxacwosc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3glfexgkn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hoeaayog.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3uwodxxyx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nowyjlqb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bpsyuvbz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kflpwjbu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3mfktjvqb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3cmejcqml.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uoarmvcf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ccytcghj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3usowuksc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nabavmaj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qfdyveof.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3reowkxch.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jnbwyczw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hgdgmitj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gnvwzksa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qgtqsuiz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xrbqegay.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3qhrdpnci.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fjdjqkng.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3yhhcvhbk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xxofzppv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfgqzhc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3miyibdkr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3zshineqc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3gelcpqcv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gzszbgsp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3bcfghmkb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rjmfmtla.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hsgcgskf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wgghuice.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ncqnhcoy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3uqscbwwr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3lbewfluz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gvbiyzzs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3riavmpdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gedpvken.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3iddeyvfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sozugemu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3fctdzypd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xwsfibre.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3piurdwqm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ymbkdzld.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yxfmkkmk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3uvndpmvv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3kolkbcwm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3pkblijuv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3huhaupym.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3misjpudx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tevisktf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3klstiwvj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cyicyonw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gtqencau.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zyqivwvj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vnhkrcqr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3lxuwnmiv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kyruinew.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rdbtmsyy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3nbyqgloz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qflbvltt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gmzkskat.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nhfwaoql.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3uhtwnfrs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mclscled.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3obeltagh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3olkvrprr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wauygzpr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fytjlhgp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zjsedyzf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3woxsrshm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3niytyflh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zxxlnoxn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3hhktdrzf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3lkdqlazb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jdmhdbyr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3bjkdxhnc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3mxxhqhha.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3soqxdixz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3doyfwiux.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hnvhwdep.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3txexizin.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwwrruqf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xwshqpfy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nrlvrizv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xcwyelyl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tywfdtfq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3inpgyxhh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ejutragb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jtvdnlbj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3svpmnjqs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3irfmfmrp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ujylesqa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3whqgilja.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gfgbemhb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3exoeertv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uvmrlccw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3eogbxlyk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oldehush.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cpadqiky.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wcexoekw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qlsdhwaj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pfoxdnoh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nksjipja.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3njimsddw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qgfjxfeb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mdjmorru.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nakqzhah.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3lusputce.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ncmckqpp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bxtautrz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dqpatbff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcxybgxa.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qjqcvnif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etpzsexj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3imchgmho.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3rqjuorww.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rginakvg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bstktanp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jvokblyh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jcrnchkg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cotqygtf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3pyknsyte.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xijrgpst.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3regjeoqu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lywiyfmq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3frjtluvt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vrmsuhwy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3twtzqkbl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mskajvhi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qhbvdyoj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ytoeddac.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uzusqcrp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jftbvjfy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qqxjlgbi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pkvlkzgv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3alidqmze.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3njjwcipi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3sxnxnglz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qzqteemh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vuigvwef.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cmrrsuvm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3whlsawnn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ivlbndbs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3syswtnto.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ytshabmn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3apfczils.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3esodoezs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3iglnxtbk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3soxkhswz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3lsvuwojt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xbrynyvf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xzdcaqrh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dvcwjddb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhgdbvac.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvroxllu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwdkocnb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jkoztege.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ubmihuyg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3urvfdsnh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3grgnajgt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bhzdmaki.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mntxnuyg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tbbrusda.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pkhhzeqy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yxnpxryr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dnuzxqoa.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3phlzifln.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pcjvrrkn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xhrrojel.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3iaqenlfj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lvaxmhga.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ueiqywpo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3leutdxtn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nixdadpa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3whbizwvy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jlnlblse.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mwycszqq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gyutugga.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ypjmxzwq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rjgzzbls.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ppcotfox.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vsooxigl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wjwqohaa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lfbcykol.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3yleydxnr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mwqbqley.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gczxsubw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3jvggkyic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrxumsqq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vognpxcz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jkfppgeh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uhjvnqmh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3foprdpsc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xfjzuvsm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jdpxkqth.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kzpeatpf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wftkehqo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdtqopfm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bburedkr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cdtwtjmk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3rxsmcjcs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dgbztlwf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fsqoyxcd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3afzyavuu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3odoeiats.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ltwknaok.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3otfgtohi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3mdotaivr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fvfktfgd.html


<!-- 参考信息 -->