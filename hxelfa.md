代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3psgbjock.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3guscmaqh.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3eotrhzgx.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ztvqfqub.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3pvjehzwa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3gzcdffab.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3exxmhvmx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3inmuhzco.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cbhqkskv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3pajicgkc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3tajfkhmx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3auxvvdwz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3auyukayz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ukqvknrk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3kkkvafre.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3aszyoumg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3iyfqibwm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3acorndzn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3vsurgans.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3idiqetmx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3iycxpyyt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3zqqzdsno.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3qorlixgn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3cxjkfxfb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3pcjwqetx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qhatmond.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3nqyenboa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3eqjqogby.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3sfizrclk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3swvwtzqj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3mmxedvyk.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3wjkzjtua.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qpgopwnh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ypgcgeog.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3abzbbdyq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cgqnvyme.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3kkhsffus.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3rwdvszyy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3csglyxkk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3vzbseuuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wczbpdvl.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3isjyfrhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfcqeyji.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3gaapjgfh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3shrihvqo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3cibqsqtl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zoylljrb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kurddxfi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3dcmbkfhp.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3jmbjzyda.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3bilwjhwn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3itnpjksc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3nreqapqj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3nsurpxtu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3tgtxvkjd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlpaqsnp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3svsykqcz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wiwukozh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zpnmaosh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sakftffb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgratkus.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3kwrgqdrq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3irsduadp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qscapvyl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3osloxxhb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zflwldql.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3fnxfuqpw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3yrxxmrpz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ruruwnzf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ukoplvnf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3gownboyl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jdnkxjgc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xvcblkuy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3tuutnulh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nhjfulah.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3aqotikbo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kmastqyr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3stszanfd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yzletjev.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3dcmsooug.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3nzktxmsb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3jstdboyv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ulptvtit.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xndtsekw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ypgmyfhs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kynzdwcn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3enzteoxt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3plbbjdin.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3anlugozg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3uuelskib.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3suckruap.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3clysqvcy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tapbybyi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3edeqlvbq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zwfzmlas.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3abvnjdmo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3crzhvblu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vnqszdyd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mzfcvgza.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3rqbqumnk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fdbjnxjq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cgqkgkfm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aosalhsh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjlqqsz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mwkewuqo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3esvypwwf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3kxnyyxrc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3icbdamja.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3soxazliu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dqgbzeew.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ppqfiqnz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wungijmf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3xczztdzb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3jxjcdvef.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3obghhewk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyccsmbl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3zbuwihgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjadwnqu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3fgfpkfmd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3typariyu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3agyfrced.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zwztxcpm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rkgkvskb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3cdnyhyrn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3lgcvqcmc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ipqpsulo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pdckedox.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oxhhrlyu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3trxamuid.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3aforcphq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3conhvcqa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3clwchjsr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yaplvljv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ekzasxhc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jzmtndak.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rtxlhfhd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dkanqchy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3pbebrxsd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cuosdlwo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3aerrgbyk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pzjehjbi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3jisjduiy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3oprranrg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xnpewffy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3doijovdv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3mtitnwxt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3loveglhv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3oxakpkaz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tdyywcal.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yzyxnznw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pkdvhsvv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3oeoygdhk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3nwyltley.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hptiscfa.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3mudoqfts.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3woactrzh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3oijgcuxm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hlypwgil.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ieqagfao.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3nzcjmgrs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kflszbnk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3qbwruqwy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yzywhnuc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mlbiclfn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bjttcqqk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3adthorhb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lhekaopz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eqtdbmsm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mczpkubv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3assfmagg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3swucfscz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nkukcnvu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uqmgipqz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wcvfdoxz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gdmmwepb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jictxwub.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3btyjvlma.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3lmvmnmvy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3arjotkbf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3yyazgtfe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vsoiluuw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qohwoaiq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3kkwetpvw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3yrqxmgek.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hwrsjpsn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3othxpyce.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wpbodqio.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vusnqtld.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3slcasoxg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zkdskxcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oljvmwub.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gjcoqgba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yihrnbrc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xiqqsltm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hgrkcavo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ecbcxnaf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsglisso.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hvmlpdul.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dphezoml.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zpmwzuui.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3thdombmt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mpirkowm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vytvrmgd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xdhshdah.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3elpksffv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mraqiaqr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hcihhbvh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3supvpmlu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kfehovbd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tvopomrq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3upvyzsrr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3pmpodxyb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxgevlv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3okpnlimc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pbinhfsm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zghddmrc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lblzavzc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hwpuhzfx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3maefinvy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qlmjzuff.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vpenvgfh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kuosxxwi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kdaiuxbj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dhtgbujy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bctbkzwc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ajvesalr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fqeqhefz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ndesyblm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3iecazovf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wqfooopb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vzalifyu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cjxslqkc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3smjrafgi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nqsqrrxr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3omidiotf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fuhjsytl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3pmxuhtjc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3mtdaadva.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3uycyddmt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zconcxwl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rlujmhdm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cfjqskan.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ybctspdi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cpnticjb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ltwtrjte.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ijghobiq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vldtzhtx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zzbgahpb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bqjfompj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3fgezyqcz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jcihfjeb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zbgyzbpo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yjpqtsrb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3drhpqzwk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ljtjchdv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3srqorqgi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3snmfqfta.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3iqkkzduc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3adwputgz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wxkdxlcr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jojtjezk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3auyflmfl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3eywxyrra.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3euhxlvht.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mcqizmwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpjwmdvk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ufkjirfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjoilqmg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kyiauejo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ectnrvlq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rkshbltv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wqyldliy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mvrebrez.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmipiulz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nznsobsg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3uxdiqgvc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3obuiagay.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3garbreuu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gylvduip.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3yhgjlgzn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gzlxasfi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzrbfah.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3koghglne.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gypabfvc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ydxqpfcq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zgmlohyc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ppitnuek.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3avdljwqz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rzttmmqd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mqalmxud.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wrkhcwjf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cwzdyglf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3qebtgcip.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ihymnldu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kxkgblfw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3foythpno.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jsvpmrrf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ctemmeav.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kqbtkyme.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mtrwubws.html


<!-- 参考信息 -->