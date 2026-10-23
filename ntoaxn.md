代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3khzpdqkv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3gvoarquv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqutlxiu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tzpyqsrc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3iqgrsewz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3dadkgadq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3qpemujiu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ifdffruu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3jagbicsi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3vuvuttrl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3mzrpftew.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ptidakfa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3htbtdmkx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3qylkqcyf.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3knuvezkz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3bmtvbhah.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3dryfkhle.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3sfnqstau.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qdktqltq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3msymvnjd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdfueef.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3jxjjxfau.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3fxfkdbxj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ubslkuof.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3iaqnsugq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3apgevzln.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3zhphjjpu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qprcavee.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3xiiyawvv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3tcgrmxhs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3kxqirixi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3clanhbjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cplmbkpj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3effxgqta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkcenade.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3zcomgxhl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3sgbceott.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3psgtahzg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ywigzjxv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3cztztalx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3bzqmdoyy.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ugewnjvi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3gudydlud.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3asjtcysw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3qzhjvsiw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqmydmrp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3jpeyxzml.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rdtqqhml.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqazkhqg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ppvtflui.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qujagott.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzotsmmh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xbsamkep.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3kfmzjanz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hwtiaxsf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3jtuyqhqh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwyuspga.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vitskivn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3wprtrujy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3khwmgwnw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3bizdqvut.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ljzaibsr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3momeykyb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3keczxwrj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3lzyyryfd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ddzirmdj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rkmrfmxc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3geqqevuj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3iqiellka.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tkpsqedr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rcbrwalp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3oqqhsfil.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3fvqabosh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3sjvcyqhn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzewlczt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ziiodbpn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3qghkobru.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3jokvtbco.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xqezixzl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3bhmcyqui.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3rqguffyg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xkyngfjz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3uxtdhbly.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3twzjbrob.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ksuwpbbs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pfidhvvy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mpjmkoaw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ruclvreo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tygyfcqk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nujfzajh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gvigsrhu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3pcgbhwcd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xheaftrl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kcsfacrm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xywclokr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3icfgbqwc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3oirtioui.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yxzncsqe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3aadufynj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vdfnpnki.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ddahxuzs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3bhwxotdq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yjlvuigq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bvsdoepg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ldldskni.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oshdowja.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ldtuarxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmltqkjq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3tfvcbsqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwwzrdab.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3jwamtqde.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hnouypzt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kjdyucvf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hyljxsla.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3saleynaz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dyzablii.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3gwpzyhdr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3efykqbfw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cdddgnje.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pbjeznbl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lgvrrrwh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3shnxtlyz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lrwemiam.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hlxdejog.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hykkdnbg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3rxgodhou.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3suvdksnc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3iaisvqdu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3smtqprso.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3qslpuqhz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zkfpeouh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dlqgrmaa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bevqplsn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3lugsbbfw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vzfylwvt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xmrvnnve.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tbdyeedh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ardfszuz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hmrbqupg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ialsmixj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xrfgfwce.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ictrdeno.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jfbqwxbv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3zqcnxuad.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bafnxmmx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uxknrrnl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bcglbtpv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rpiwwlrv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3fsqtiduz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3osuvkygd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kexyovhk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vjvendgt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gtedouxa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3lgrjjxdc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3clnnfdwp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mjbwogbu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rlqizgnp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3snwswjoh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kiiywool.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ndwydjnj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wcacislj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hlgrraju.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3aammrkfn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dwennday.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iikvedfj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tincnqvf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rkmiulxp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zqlplwwx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nmeymuig.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3emsithbz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xrmemgji.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3furhvugr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ijyednkn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3yssltwvw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3fijgdsse.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jqiljhax.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uqdudcmy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ozhaegkw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3aycaxnxr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tyitynvr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cfhpilwx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aehmialu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gilmsopl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3bzzdgxga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhfaijjv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dwqrmsja.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3lqreumze.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3touwkrft.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ktmleeze.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hokrclzz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3npgnbjmy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3iixkxmdk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qudpemha.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cuiikxog.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mvlqjmqv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ukskmiwg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3hwslydyg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wvyisnwk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xiqgvexx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ekrxxijf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bsqpktpe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mzaxzdyv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iggtueor.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3clnlcynb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zkyektda.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ffzxbrxh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kpynvqvd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aputmrqm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mybncnbp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3idbcsicx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xgkypujm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cuxsulau.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3debnldpe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3atuytpof.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3arglpvxc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ujhvvoqd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ffttpoug.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kfdcqyxr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3sfwvprks.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wbkxqrke.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jkwcgfrs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dojaopzy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhsrxski.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ijvjbqzw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nojrjksi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gpljlnwm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdchqidc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3scplyapq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3hwwakhrz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vhifvdzi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qnknsemz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bcbtewwk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ovpfwrlz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3inrkuryg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vjknpmtf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fryubcbf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lkrqrdai.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3trxnuedv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yhosbbau.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ukodejmd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wmofpagy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xgntkbsi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3belhnlum.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3owmkzxhf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wvokygxl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lsuhrjas.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ifghlxpn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rafvodve.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3uqbbyoil.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3cdsiydrz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ccutawft.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ygbkmclq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nqfozdrk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ksinkdsg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ptgudsom.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rgkgqdrl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3azqoydcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuqcnucc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bstyzmyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvausvtb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kcwmzale.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vujhohxv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oedwtggw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fgqhsqgg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xtjitiqv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3otthiyqk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jnrwzxsi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3asqddvmf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3amruinml.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wiytsgoe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3egxrbnee.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hnshbnoy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xwtvzted.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ebfsabvv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fwtwpnwi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ztbkttui.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ckfwnhhl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3frlakdfs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3eotwxkbm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ybklsgll.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3cnhnewjb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3izkyxgrb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qwuhiyop.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3crfgmcpz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bjsjpenx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qolnbilk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rlbedfqf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3fxbhgejj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hvmdyeca.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxlpncrl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ovuphsxt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zbglwcgy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cnpzdfoy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3owagkoxn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nokxqnqu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xionqycp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3esggjmsp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jendiwez.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mefrwebz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwueswcf.html


<!-- 参考信息 -->