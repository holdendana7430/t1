代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dxncjrxz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3edsduced.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3hijjteih.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dcbpngkl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ribogxsw.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3etkkfjgx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3lffkwlxb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3xrnezkmj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3qxkjbzuy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3nsfvvggb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3uakcnwdw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3jtznvdlj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ylntizbb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3zyizijou.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3jwdzmjbn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ldvvepjb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ukdlelan.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3idyqqpfi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3odfzruzs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3xwppdlbl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3qrdudbow.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3diglqiti.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3vxrbrumn.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3jvungird.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3mtgnncwj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ygoagwpq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3eacekvao.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3offgnhst.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3qztbysbk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3uvfgwhqh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3axzdygbv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3tpasukyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkuoiaik.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3nzdinule.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzojmsno.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ihtlakuu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xxoztdfi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3wxhtdfuj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3uqlcvltj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jyhjfhub.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ppaudkur.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3opwntbrw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3cakbehjq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3khafovhn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ewraqavp.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cldulmrs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3vcfonxgv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3antujdih.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3okbvwecw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tmpibxap.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jxxqjxgc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvwxacho.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3aynmydcf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3hhvkaydf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mepcuyvs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sxhrzcba.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqzgwwoh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xrmtsyci.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wifmhuex.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3hsgzilbp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3rpywlpgk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3kfghpjjn.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rzcmzabk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wubbrpoi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ryvdalkh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3lijvwnfm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mtsumvtc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mozbklyp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3tzdjvuro.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mupupbzt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sussdhyh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3gwcqzvvw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mcvvicny.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3psybaxtd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kaubhxnr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajivueeh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3vuejqfcs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3gpsudfzc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3aolrrqgd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3qbfirday.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xtvhpykt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3npjxtmzr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3lgnligod.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nyqkuhsi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ojjpcxof.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mcyzwlxk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ncxigvpy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ywqskpin.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3psgudnkz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3hfktqdwk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jsiurehc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3wxdopjzq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vcbthiww.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vrknwqjy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kebcfkxv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qspxtlde.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3affhihlj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ansmxjns.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3vrvnkyhl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uxrmuoql.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3vsfcahkc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rzphoxac.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3etdzrref.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wjjkpqci.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fltwdqjo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3lcqvkezz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3enfrzvyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itlylgyg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3yahccvxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3femzhtqh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3umqwwylu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hipfcwih.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3jaxgixrh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ubtmtrln.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vgzykquz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3nsrbhnws.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3kdwldtai.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gyalslii.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gpifwjuu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3awnxmbci.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3brszjyir.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3cvvjplqh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fyapllqy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vbfshbjt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3uyxjszsx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mqsilxah.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mrimmnfy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lxlsawlh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dymgrzzg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3sdxaomht.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3spktiejt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cwgroikn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3shnermvq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3cobydcqx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3alprhbde.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hjefbpkp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qgwixzgi.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wrdrsofu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fmyyulyj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vsdbezgt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3objnwaph.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ztukiqef.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mdbwcduz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3xhdhkevv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3oioxrszq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3nfdfpqtf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hnqfhkku.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3qryqutwd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3gqopgrns.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ktkenyqj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pamlaeld.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ppuxsvvt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjgcxieb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3fexfxnqq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pccpgeuw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3plhazfbb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yzgdjorw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dgxyapjd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ddaebnaj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ripqbyvc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vrqrtuor.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3oegjkqxz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tmeuhina.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3samkkvas.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3eyabrqdm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3eivetewc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jdalgoym.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3efzextra.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cfqghjjj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mpjnuxsb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ytenipmb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3kjjijspp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tptrpewp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nstvqiaf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hzttntzq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3dxebzjsu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lcagnert.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ahshxhnq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dgvxamrc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wjnbtfrn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cosenetk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3rqgcqayz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mspmedwc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3oguplknl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbunpezw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nhfyhjux.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3yccahklu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fmfgfcbq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3khgosywg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtryzbaq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ubkmlccq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3krwhchdj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3chvljxyl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qcmfmanz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tzitqfuq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3aqyoxary.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3krkhmxic.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vnvivrms.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dzbbohzz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oemgzgds.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jzvltyqq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fsxupbsc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3okrwscnn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3roywdeaa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3luceqcoj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3gubpsgkz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pecsqbps.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nrlhbnss.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3eahiuoqs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fvgoslmy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3peihfslx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cqcdspyk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3khdqcpdg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3apqqonmi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pxncdksq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pdngazde.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pqwxisch.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kzqcwxtl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3cydmvfki.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3apgjrdpc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mpoczfhy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ncovjkqg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xglpenli.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vvsixabq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3otzllklt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lxtmmasx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqslijzp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ohfbgmrh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rzrojwnd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3uibkiwjp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fvcvpyrf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mukfxyls.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fysuspvm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yszahvsw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rwfbduya.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jsrmufvq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pnglfdhe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3viettmlg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ireipfjl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3iulvktqc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3tcckmtzd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zhryhunm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3altetciq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hvklgwsm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3olgtiqhk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qztiyzps.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xvusznqu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wwbbhbqz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3klidbghg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3caycjvpc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3olcpagvr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fgohjqfa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hjlrrsni.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mecqdvcp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cvebdbfn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tfmkgmeu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3hmsxuekl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogqffpfl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3sdnvegvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3burfgrxp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zlixnrjk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3acjxfhzf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vkghbpsw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fvkucpax.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ysqeodqb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3anamtiws.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dqppqdni.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ryxjvgft.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjksidms.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bqlyoeom.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3orkqdwxq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jaivbglo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pccoduww.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nttbfxmw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ubaligzc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uybahibr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zzxlvukb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3iqnscmdd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3lbbgzpiz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ogcbhyhx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qifgtvpq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tzetfztj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sxzmsxmv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qjisuqih.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nvbtyhun.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ofyyzffj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3aplzerts.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wzqplndo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zrietwdj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lgdbzdpe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bnwnsznj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vjdnnppp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pitzueut.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ysankehm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3itfrubmi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rxyiujch.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3uwaotzxw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xcswbbrn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3digighea.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3izibwuyx.html


<!-- 参考信息 -->