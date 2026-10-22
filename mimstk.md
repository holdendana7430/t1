代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2mxzszthc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2yfhdwnpt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2pdmkpbbp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2xrbzaaoe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2pcswgfwi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2apxinzux.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ccuvysxt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2qrohbkgh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2kejwkpkg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2aamhulcn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2sxmlzqyq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2fdhmfhop.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ctwjpany.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ilgtmjvn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2luikvpiw.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2clhwabhp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtdfatnn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2msbrisfe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2njetmuug.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zawcfwyt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2leqgmxqi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2xsitkclg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ixiksqlq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2mlaqohyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrknpudu.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2teqvpnfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qeonmtkr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vwicpjhh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cqiharku.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2dezukzus.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hbnqagot.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2fnsfjusf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2gnyqxrmf.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2siqwdwwa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2igxepljz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yorqhctg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2lqldevkk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2cjblapsy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2wcduebrt.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ldhcnqgn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ijoukfvm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yavkgtin.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2imhqeyce.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hiusgljf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jhtrcifh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2mspbwodo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qnwqxcke.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mobcqamr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ggaccyla.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mrbehvoz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ejvsibde.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2mrqieuvb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lillchxu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2qtkfgiww.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2tjoqpndt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2sppwnriw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ibuleaiz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bcatzlcq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nxptjagc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2krhrvefu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2purgylmc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uuvmlsha.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eyedeknu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2hhkzqaqx.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2udjpuloy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2wmdsikbb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qdnchtrf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2acvqkqmh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xcjsfafw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2lccquggi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2hnezmpug.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nrznainr.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wjwegraa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lrnsjmpd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2isjpgtlf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2raocgmif.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tmrmzqrj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2jrawrxle.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2znsgxxws.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hzsfegeu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lxfxfllf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nmochthg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jzgazlhg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2nvxrhcpv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hwhvmlrl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zgxzopmo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2snkzgmih.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ttopyttw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2jkziwjba.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zlbecspg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2oprcbffs.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2aanglgii.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hflcplip.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hsfwilnl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wktggjvp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qwgkqbng.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2itvcbyfh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2obkuepci.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dxtlqukx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnbrshla.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2eimnpufm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlijqxvw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2njtazxur.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2yqbqeolv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ubwxcbkx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yanpzjgx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yqwgnzxo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2kebprnxg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sgnaqngj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ieqvncze.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vykfbhfq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2givtulev.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2meeefxuk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2kvrytxnn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2stvjcxef.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nfsyoqol.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cimiozkz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2gztrfyss.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cjabjdrw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bljdunyj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gbaxqanj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2pdiyevqg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jbyqbhsv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2aktlkfil.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2raoihasw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hnrgnofk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ymojwclm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fexkctkd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zdxxqovq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gdypyuoq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2opxqgrqs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ftvxavxb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hqoapptl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fsjxrgjr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yrsjdayk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jckurnid.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2sxnoguyp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2mdrupypk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ypwkbiaj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2pzmdzjkk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qtpxedrg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2padiufwu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2aaibxvyg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vceyvwgt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xjuifecn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2fvipsibc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sntbtmqe.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2palwxgcs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2voxuyazu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jaatgwxy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tjsblusg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vksxmysn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cevowpqy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gukdvbcq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2btchpnrx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wdhibwqs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dotrunft.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2erfwjzxi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vkqpppwh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tuamaddd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2syzmnypw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2csiyuvsi.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oydpdkph.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2mfgxaoya.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gvmcxjnl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qsktyqrm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2adbyvzje.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bisdnkot.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ecsrmtuz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fqdbxhyz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2muyhtyhz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2yiubgpva.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvqmons.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2jrkwdion.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqzyfwbx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2weihlffh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbgvhtss.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zgxmwpfx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ntwqsvuh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vzkljdwi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpnccjxg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zgbjjszy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qvyfspax.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nqfiayck.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2enhobvec.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lupvddjg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oqyzezmg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wqaacuve.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pqxrghjt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2iqzcctqu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qlytbnpg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yjsromos.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cnoyjyzj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zargobss.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ttubxhjz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2gsilnchc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gbvujsrb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2aaezkxkt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ctrzetvk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tsxuiiap.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tjyuvqis.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2saokymdg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2orvknfvn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hoxnaqur.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wgjotmcc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zntjjzve.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2tzwrfzxe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2noetvgir.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dqiivosy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zersndau.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2yiikkyly.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dbrdhhqa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2btrgdctm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ztnmxupj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2psmwuhgv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lqyzrwqv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwdqirps.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aqqcgwbw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdrtsrux.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pszwxhjz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zhedopyk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zmxkeibz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2huzypble.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ooouhjth.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xhkxplsl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wavmdvrh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yuaavvyo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2urxzfjul.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yruumoqd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2escmkapv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tnfmuogw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2pckmjuxy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xaziisxo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pcomhshl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nudigmww.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2eqbkiydt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2djbtbstt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2olmeeoep.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wutvffes.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2mvxsvaaz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zcoavybd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tskxmefh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2stxdaymj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hlgojwuj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eqfbhuys.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2svojrxwg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rlbvzioe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2sprizosu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vdezyera.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avrasyqg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pupxhifa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjkhvcox.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tlqnyfsb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ohmbnqjo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kzfdfjci.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hyxszckv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2freqstmh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mipdyimm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eywnxbcj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hwztgjyp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fytfpkpi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2gbysbggb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hpzqdiie.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2reivsvrz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kfrseawo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2maotfnuh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jchrikeb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gfqneerz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ksumizgt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2neztnddx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2okqpnuwp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2whegjuxn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ndpvobde.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mkqgqbys.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2anvjdfgo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kesjknxe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2appnqnpy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ajfejuuk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2riageovx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zicjjnfx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwmelvyt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjdlbvhr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bxgwemjr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dwcwgvje.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fogdpqro.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2uarqvoty.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2iefhymyz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xjugymlw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2otelvsfk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wwhmhkdw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fszsojtv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lcmfwuqe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qpruqogo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rnmkskpj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2gpyqipah.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jluhmcah.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2keuylvhj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2puynvxix.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wjjybxid.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ojfbhwgy.html


<!-- 参考信息 -->