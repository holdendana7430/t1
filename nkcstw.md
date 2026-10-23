代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lslltxyo.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3qpgkxsiq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3iodgchny.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3rchzctqa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3fsnwznrn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3tkhiupxa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3dpfhyzma.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3zdwbljbs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3aydaioek.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3vkkgsrdv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3uzqfprnm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3niycyvgw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3lntitbou.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wqarbgvk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3birilcsi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3zchyjjin.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3esncljhl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3zpunuqui.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3qecxkpzu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3kqmygcee.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmswufrs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3zhskbuix.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3uoeycsod.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fhuwlnnd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3iapkbvlc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3tldxvlwh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ppqbxhtt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3nygfjttg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhoweodd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3qmliqnje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crgjqozl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pghfoxqk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3yuichiio.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hvhfnqss.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bjjxeffm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vwhbfdqs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3qjpyurxb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lgtfqqak.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3wxsdegkv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3iwodvpov.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3fbjgocfl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3torfygvu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3zidyjpiq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uuyetdvq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rkpunlfx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3eywulqyj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bmxcrqdp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttuabzhd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqaubika.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3orbqzpxs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3esmrkjeb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bekyagwv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3mocdugat.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uaeorklz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3pqihzhpg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3cfucctwg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ungtxoap.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3vtsgjwoy.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rrajajgv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lrqtweuy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3vwwxrgcv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hadxrdlp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3srtwogez.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fdkfnztp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3yoqyeuyg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xhriczjd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wrrkmxsd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3mnreluuk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uynpbokm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ffprumkl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mgfuxrcn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aqtzujqp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ytagchxa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xsngetmx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3trvgwdex.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3fowrxmyf.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3qwkolpuu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jgyiommd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3reepsbdh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xhjujkop.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nqimjiei.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kaoaafnm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hzffndzj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uqrvebmz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kzgylgzx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3pkvbbjik.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3adwrcsvo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fwowxmpu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nswttnld.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3agalywan.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mxayiizb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gkasxhvz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xjsuqjax.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fpfmkmwh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3slyxfxbk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3evhxzlib.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bbbetoxv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fsfmrfie.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mkjtwbjg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3hspgqtdf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3hbyoxwus.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hygadnkt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gberqfgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulxlhhax.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3eommjhex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvtgfnxa.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fsassnzk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xpnrqkwq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3asljcqsj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3opjqqetl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qunbaeos.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3cclnhedv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3eildftly.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xciaqlxd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ezvqluel.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vhkuglgo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pkizssmu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3jvmxegcz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qhdpoxrr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nrcuazbp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3byywhwbv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3kuetczgh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3knspypha.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3eewgjfpe.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fxxxczxv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3gxtgfkda.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3tjddjilm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3eiugkvls.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kynrruso.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ebqfviuf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pftmfvsv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jofsnfet.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ltpktshd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3wnywqbyc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jqboluam.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ccqsqhtc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3euslstoq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hjrqlcyk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mcfxevwe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3wsxmtkoi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3nhkuknwk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3urdmcbef.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gfwwrslg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3urlbmuuj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ckscydgr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tbdlwndj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jdoitxdd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vwjwgymp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3oethmkmp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3vmbcjpwi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onwlvwjg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3uotwczgq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sraivcbc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zoytpzaa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mglpipdr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3myqjdsbx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nhqrigac.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xgzoavck.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qpkovcis.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3hmjogckj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rlnmppta.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qvpcppea.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nxssjzfn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uwvpxgym.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bxhhzmmi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vonhtksa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mllfukgv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3lgpyakrt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3spuomdhe.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hbxpfxji.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3jcqsnnpx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ywtiqxfv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rkpmdmzs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3exubcgjj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nwtdlxvz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bekmkssk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vplfelqh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wgbdwzcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opnmdttt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3tetmhepz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pplxbfnh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sibumtld.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hatzpbly.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3guffucck.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ffzgjgzs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3udokmgip.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ymtsugay.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jfryswcn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3hyburkvw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3osvfetfs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3afengglr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pjotziiv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xhynfpnw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mcphshfi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nfthxstq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mnzzgwni.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qqnstnap.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3imsrnaqa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zxuampez.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dwgrvkpb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3grzgrjma.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zmwkhdrm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yrkcygoh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uscqvjvp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rbjwwzim.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ewosdsii.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vzmjqcsv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wjhdihju.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mkaxxnfg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rltvuisi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qclwaaur.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vwswwxyl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pqvcentj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3nwtabefo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mnsuauof.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wzhsdxht.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3lfogqrya.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tpgcwskw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3utwvlzho.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gsqmlwrl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hepovsxt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mtzzstul.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwpfdked.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvdkxfdb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3rqxeggzl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3izklvgse.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3uolqqgwk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bgbzvutg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pjpnroha.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ahjpdnnb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tbxfwcps.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3upimehnl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cwvmulrb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lprjtmbb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3kkaahfnx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tfmtftkx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yztmbzns.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hqgjdtss.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yucbkzau.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zcdvcioa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jylnndqw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xxmkzoxp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3vwaucytq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cilznyyf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3azokcrnt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hkhmszbo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pkvaxggn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xcazpavi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tcgayonm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gixihhxj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3agkcrapx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3bvilsdnj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3uuawknvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfwvkdmv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kywbgmtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cphritzg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cnbqnkbu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhotbrpp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qrrhycec.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gijheqxj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pwurllrs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3crswrbbj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3icxzxals.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gvaotjdt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcwcwwtr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nzoygziy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ceueksgn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bvvvfuuo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ycdvmrbl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jgzumwvg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3krgthzoe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3aouuboow.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bbqjjlvv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zxrgqiix.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3sxmrmdqv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wxjpxxtz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bnehyoyo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gnmnzgel.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bornphzq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3plzxzoom.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ilpgnmai.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fjwtnizs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ajrhditq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gsjbstif.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmcaagge.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kihjowbb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3crtklvst.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zzavetby.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfnmtjyl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3iekqixml.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uaplsbql.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xtocoepa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ugpbpztk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lmonlbjd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xmeltonr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3loyreyuz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fazadvve.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3eylywvib.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qiygfnrm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rcqjhxia.html


<!-- 参考信息 -->