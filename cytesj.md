代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rjzisikn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2rxltuqlo.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2lvipcnac.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2dsuwifwo.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2szthnobw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2eprepcke.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2idxhktfi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2teibjiuo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2dludkuwr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2amhfltyw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xdtwkfkh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rxkwidrt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ywztmjzu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2rxcumcoi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ldfkfibt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2rnzsmdgl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2xcerrflj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2xmegtfea.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2toguxeyg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2gfpskide.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2jvdxclvk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ikreloxv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2khrkwtfj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2roghcyge.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2nwsuyvix.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2morpjwqr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2vqhbgfgs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2kagfsbzu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2gcfauzya.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2aaojfumk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2rqkfblua.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2pfvuorha.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2hrjjnbje.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2rgsmfnua.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ciigpklz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2shyfruws.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2kaologri.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2pkujruvd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2dkqylibf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2pkzeidra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjneapcf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ayecjung.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqsduodq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2twwymgoy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2bxacnkfk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pptpdeia.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jpvkvehg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2buiwaqfb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2qfzycrrf.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cbiaygcs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2qjujians.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nfanagqo.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2cdymmnvq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2cwilmpao.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2yccrgsuv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kdqlqlkb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ubqzlevv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2buwbktin.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gvepamms.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bycchfrz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hxcvnytf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2etjqgxgb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zbjibpvh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mzxfduhe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2txkytwke.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yserjfkm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jyuuvrky.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2syyheqpw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2clonsuzp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mejemvyl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2pjwnvofe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rofvgrfo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ttehelnh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xunoqzlo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qfjufqvy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2svicvlpw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ftzowtqh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wlupkkhe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2diinmsbu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ichxthqi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2wsiebviz.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2yjhejwdw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gwchnhoi.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2orqsudaw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2hoptmqyr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2qdwnrbtc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wsfbsilz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2biuvkbxf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2fkgecsuu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2whoxgnqa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2toaiuvoa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ivsqhlqz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2eokgdnhj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2zlmvbrsv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jjlyemti.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bcxjbmes.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2byuridqt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2jjeayeoz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pgdbkjwv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2kfwpqnoq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ucfcfykh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnfnsfr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fbeaijgg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mcnclceq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mranwbxn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2baqelpxn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2gsucccku.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qvohpdcr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2anddojqx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ceolpbfn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wlyuknup.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vqbhrssa.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2vsogmxmo.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rgkciaob.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jxqrtjte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkpcucwr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2udolksjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycyyuxkd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mfmjravw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ycfommfv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qwofxxgz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vkshisnt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2teuxxsvy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ojnqejtg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pdawkyql.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2eymbszbe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wtwhonko.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fnkhlztk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xeeyyggo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2nurqfnuy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jwyjlhcy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2smgbamhr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ftaazaea.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2oczrtyab.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rakhbmpi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2avztsxfm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wovvyvqc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zhwuurzj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2cjdzowju.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ofxhyqhb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uyulbrkn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2tbrexbxc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ktoybist.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vrrvqsuv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2larqrcws.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ncxrtzvl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2biifcnbo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gyexntxx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ufvdgwwn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jixarura.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hneqikax.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ccynylsy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qdmowhyg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qldilgex.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2pqpfrkcg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nytciopt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2efhzrugu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2prcfhtyf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kyzjoqmm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uouiglax.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2pnwjaqcy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2nefdlemz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lvbynuxy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2vrbzxlbm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xsyifyrv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2azuqnjbf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wqjadann.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2epebuagc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zemnnwwm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qeohjmpj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2pnzbhlao.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2isvmrxgy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wuzbzcau.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cegvmdav.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2eupjjvus.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2unfgiviy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jisolpoh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2iolrurjv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gybpcaki.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2oqsyayxg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nacyzrup.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2zgkrnagl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qxmxesut.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2adznwfwu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bkqrtihh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2txdfztns.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2eqcatrez.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2iucfopdg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ksqogccj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2syfnetbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bificbuk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2girtjfdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqoaovvs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fyfnkaky.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hppmqtov.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2agprsvmb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2akxtjnsw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mcwsdrzp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fkjzzzff.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cikfscdn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dprqsyxj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ahmxqjvt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2eskywwhx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vllpqdup.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kdbzddjg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qlcxqggg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hnearklx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ozrarlsv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uwdaeyfx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wpogbxxz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ovbsoifs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ntlcrflj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qigztfwd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bavjaiao.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2umeifard.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2guakvdyg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vupmkukb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2pbpwmvbv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zlujahjn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ydporgkc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ogfrmfnw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wiotvfpw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qmfvzhmu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bjcqjcjw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xpkomosl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ekfytcdk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dighqmmv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bxwivsqm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mlfxuqnx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pfihsvtk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cbxoxqwf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qzwkguaj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wpphzukr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gjtmxavp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dncppcne.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dqjfzkjf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ogzhipao.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hteeifix.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rlavuyyo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rdbtaeld.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gqntkrpi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fonckvgf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pmzseupi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ebvrukjg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2szjpkiza.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ffyoaaph.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xaxsdspt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ncdvnzpg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vhaucgyx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mdievhbe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yeoxalxt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cqvuyuan.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2xjjbvcxp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2erapwltp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2pnwcvapd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qvximshm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lyaibrzn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rvnsmtcq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vgmqbtnx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dsjibaxg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fgybzezi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kqvltjfk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2eufibybl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cjsebxzj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vexaqevp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2leczmdib.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ztbknpwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jedhlcea.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2lujeojkj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ydaxqswr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pbbprfcw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2azaoswew.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2somhceyb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jgaklasd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qdprxzxc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2bvsmgfpu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wcqxvuzg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2trzezzgv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2akipngdf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wjnmsppn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zwlheoqh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mqpzqcpu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2axolfjpe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kmicwsmm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ijcybrkr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gwvzwsha.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2exsqzeyb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ylzjxqtw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2sykcrirj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zwntskfk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wiaoccuj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fgpzvslx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lnwdzlib.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wwquidpu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xfarxpsz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2hdkikefe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxerpef.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2iklaemyx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wylxqxfq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nzwkrxqb.html


<!-- 参考信息 -->