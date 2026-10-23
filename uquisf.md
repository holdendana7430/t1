代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vykvuppd.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3qslcsjtn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3iqyywdre.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3pdwhsmjl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3nxkyfgiu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3kespexuv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3uotadoin.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3mfmdxszp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3gflnkafi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3jfgjptze.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3dfhtancp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3jagduzdc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ilalaxcy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xzsmzqmx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vufuismv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3bcuumsub.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3lnxrourt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3rsgizotj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3wojokfem.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3gyrsxhtm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3bptepgeg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3zipikmvr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3wfpjnlrn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pepibphz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3dqbwnzsf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3shojqawy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3epwhqxnb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3uqgwovle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvwwrpml.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3fpupncqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilwohwki.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bxxfxqcq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pjaoevzp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dpzmwure.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jdtsemit.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3rhtgtbpk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3xbhfdzdn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3jxrnmllr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3efbpbhgs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wadearcv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qxwlfpbj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzxdelve.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3paejmhvc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3prqjypfq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rokaeiki.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3epiyzdsk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3apflsigg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwxonocg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3afutggvz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3uajbdhbq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3rplocoum.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xticllmu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3galvumxh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dpdpnkpu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jobpoywm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3zkufgcrj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3iuormczy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3aviwwksx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tgrewrlo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gspvckee.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3amkknqbc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wjmdjdtw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yzrfjafe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vyupujsl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3yrbeqwna.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xwmjbpsk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ctjwvmre.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3wqskeluo.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3qelsnkje.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3rfsythuw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ddfofgqa.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nfezummd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ojobeiwz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3eegsqeas.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3entjcdgn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3fnjvnfwa.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3eustzikk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rszskrcb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3bigqgflp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3atmdchqq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pqakgapg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3wcexmfwn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cswqfoqx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rbrbbdzm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gihefdvn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3qrkqarcw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wehnbkim.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3famwfdds.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3logzlaes.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ktzytytu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bjrinamz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dyfykgtf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3uklgxesz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qclqcspl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3uzrilslc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jikgpdkg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ctbvgllw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wwapbwmd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wvlhdzvi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3eefebnkk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nubzckgf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3yopkxgnx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3waircdql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umjriiue.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3gcovfhii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsjizkzk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mpbwsxwo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3smstzrdg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3iiskqwry.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dnncyrgh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lrslqpir.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mcmcixdd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3damndkne.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3sxqzmdbn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jqfqpyil.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qdmdijxn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ybhllngz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ecanxnef.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ezqjiigz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lvgdkfab.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dhrlaqqa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mczbktpe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3caawaxpo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rryuwxfn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fefaptzh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yhhstdaw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wvgdavle.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rukytrlk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3abxtpnfk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bkvpbmfw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dnzehpvz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ocakjinz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rdvxfpox.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bibwbiyp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ublnlyot.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sikikyjl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3stmfscfq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fcjztqsh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3spccyfom.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3olszsvzr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xmliwcwo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tlojzpqf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3obfbpzay.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3kzvqmcyr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3mxgqutjb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3doyvoeuh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3iidceccg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3meglqbjg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pqhuqrbz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3kbsshife.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tnrfdydi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3utnnypky.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pgbgwylk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oorpyzkq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zncmsyhd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uyyuuicp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rgntchdy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qhspsbch.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qjljobtx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3avunjyuk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ghewlljw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wyvgrjge.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3oxjgsckd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tkxuiwfy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gaxdkvbi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3rozjimkl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nedrnpyi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3rzrhqehg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jbugfrjy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3pklvjrww.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3bpummeme.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ocxxasqb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3frkzkptw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3judczxkl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3doygkylr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vehrnmdw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nqubdkok.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3powqyory.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmkfwuqz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3eqhgsjzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfvuaqoh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pslmsnyp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mgmzbeuq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mjfltppw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bepslohu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qeddfjnr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3orzrhvun.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ajeelmeh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qblcjjhx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rszgxbul.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ndsidigc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3btywsonf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tdpndfsr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yhbecldf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zmowsbod.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hsjdcqzg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nkazkqvd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wbiqwxfo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iyqdpdwi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gatypsqz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pzbjnixw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3aukwgyah.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lqmntzsv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vwabrnjo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3cnqrotry.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wlxggazt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3udrfgwfm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qnvplndg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nzrlpjxa.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3csbticdd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qrreijga.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dqreqvwa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3odspdzbw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ozjocedf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xwluvklh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3rmtptydu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3padgcbgg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rvnseqwt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twmlgpjr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rlosrrhr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygkycznc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lrvgivok.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fvibyerx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmngskm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3tpiyjtok.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vxafgoio.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tacpyjpi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yhbblwcr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3othpodjc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wdoerpmd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fukejxoj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3iiarhyrs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kqjlijkn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3pdotwytx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kizncwuo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ziptnpwn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yvzydits.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3nqcvfqkh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zbihudot.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nfydtwhv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3skcjteuc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3blhmdrry.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jldzvwdc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jqspjzee.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qeodhsko.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3racqhqcp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ysyfqtly.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gvmkijcm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3likmqkfz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jfleaucx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ticzbcku.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3eouhinfp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3tijdbuug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehqordpl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jqwhftmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vadimsdg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ihtafvvr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yqfnuofz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ydtituyg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3heyeyboj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pkxxosgc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzopmmvv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bljfrrhe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3iljcbrac.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ganjonan.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xkmdybxx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vhxhyisx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3aafxasxy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wbqubgik.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hljxnovr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tvxybagu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3syafheiu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tirepptx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wmodkizr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3tvetizoc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3lghohsfz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gcshhzgs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3izgsrhqi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yasojzjk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bhpbfefs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3tdugpzok.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dwvolsti.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ahjnsvue.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3fipbqyao.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3psqwnreq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bawipsua.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lptlonel.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3thfkwuuo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3znmtveeu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bdfewnxs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3motfqflh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cozqtvmh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vhzoddyo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jusdxkgy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlgyqarh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsfqmano.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sfgjvuon.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3jamfpboy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kldstukd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3akkeyppz.html


<!-- 参考信息 -->