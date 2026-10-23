代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3teouwcik.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3dddnephk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3rbqvdrgd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3zhqtboff.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3khywnxkg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3wfcweqeo.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3tzzkfspe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ayiregvy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3joksloec.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ehkswsrr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3rjdwdjbc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ycchaivg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3pnmssxcm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3inhiwgun.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3mplzdcwl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3fwuhbrea.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3yycruhaz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3uezcwzbn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrfgmlc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qwileezn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3henfvmti.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3pdyebcjb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3zsawbopc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kvnilmrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuhohjqw.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3nmsjlhpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnuwbvqg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3banhomwe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tlqskkbd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3laxgaazu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wuhmaxvt.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ciuysahz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3fibsqtbx.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ljtvpgns.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3gvzdysgm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3borogftm.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3qbofugpi.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3vmirjyvx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3jfbjxzlc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3omvlrhnv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qybjozka.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xohausyw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3asvgleuf.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dyhtgmph.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fqizawud.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3zyovcvst.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3diinigcd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jeiybmic.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qcdpakpl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ylynpuda.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ujqilzhr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3exnaerox.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwbtxyh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3cpbwisjv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3scqfoioh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vbhlyhav.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3cbfykoxq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fkjwgtwt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pvfrlvfb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3friilvls.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lokxsfxi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3bfqheulu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3klleavej.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3vxeagvyp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pkhqiwty.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3vrluqwbf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rrdtiwby.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rleoblso.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3gdfwasbs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kewabhzt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3gjeushzm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3robithym.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3byshgwls.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wueuzjsg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3dhoqbxdu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xxjabubh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3aumbmrql.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3fpqbtsqv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vbnuvjtu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zrjzjoka.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ixrytblt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jfcinzjy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ladlzewb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ruylbgdo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bqydifho.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xeehlbyb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mluvwfwu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3yixtzcia.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3qbydgvow.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3etftqfad.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3edykdvhp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3opmkwawz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zsgrlcfe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kgpdfxef.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bogsfzrf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ppjlyewx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3lbrruvxh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fkhqyhua.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3waqcgyhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edhdulmu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ftpmjzti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etdbafva.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3mzjyryay.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3osnawmak.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3dgpfidpn.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3acugkbpy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fjxgpezq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3yfcsqwno.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3xcizaije.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3czmsuvzf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3otkgqbca.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ayjtzcpw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ocdhhvii.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3zpewgqdv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3oqofvarv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zgksrnpx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vcgixfzs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qsyvbbdv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xnngtwwn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ccrajhod.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3owfipegx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3moiyjyjy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ctvsrvvk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dxfwvygd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nvrdviut.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3kxuvgyei.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vykbnjbe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3dvhnjdps.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cfispvlq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3riwbcrro.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3tuobabuk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3oeowcjkz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nzfhmpay.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uzntauob.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3phfjsreo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jwrqvmlx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3smtabkcm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3mdbmiiaq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hwnxnczk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3snbsgvmz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wdqqmchm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3sqfpkwma.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zhgmxeak.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3cjoqylrn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3liwldava.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fxyoioxy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aqingycs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ilcnsffe.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zvvaimaj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3eqiscsnm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wymlhqnq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zhwoedxp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3addnqxgv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3slleueku.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mamocpnk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zltyjerf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3phitfljc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3svxlcqra.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ckvaqnxu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ydeifzxk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wckfiydn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ynpanack.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3njawyqtp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3cywgipya.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rnfihbjx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qvohvnjh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yvgjnsbh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3kgywyhmr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bfakdfzq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ztdlwmjb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ydwdztrj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3dmkrmcwk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hfivyqoy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3floopagk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efxdmybr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3dgwcswrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uavrwsyk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uqmbytoh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xcatyevi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3yjcxtiez.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzybvhyl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cfqwhxck.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aocmhpmt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qndlveqb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rmcubeuf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3sflftvkb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qiyarswv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ypvqqoln.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dyllognt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yijmzntk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3orourzsa.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xgvgckoj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rpelnfkz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gwiovjqi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pdmxdkax.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bfbvojit.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3lrztchxb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3elvzshah.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yjrgjqzx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pauopnce.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ygdauxpm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3uaamusbq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gewehfhp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3aqumhiou.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nzvivmsp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vhnxqiho.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3giefevrl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pecosqdd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wbatirqw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rcslitmd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3onegsrtr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ovgbjrzw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3sypgdplx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xjnwmqlu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jijgpjiz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jfbbfwmd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ikjcfsnf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlgxqlnp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3akkksehj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lckbomam.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zelyhmat.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cgdidbow.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3nikonvek.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vfqswjgc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ikwwxszl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3osnxhvwg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3omonzxky.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gpxvcoop.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tjzfdxxx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3muzmjwqn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sliqcbac.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gchhuneb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ljjpxgvn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3yhsqauou.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3whuoruez.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vrrnovtg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3bvfcwmmw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tgmyhzwo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3pdyuxbuy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sbthspnh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ouywannm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hkfirqhu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ohoxittl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qoddlimw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oivumjct.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rgakqppm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3glyeoqhp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ackwermi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3nevtlogl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebmgqglq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3edibdyin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvbzsqiq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ldafmtle.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhbwpchf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqowbfj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mfznjeij.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3btprmdng.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3feaothrp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aellftox.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3umhwuxav.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymbiglvm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kbmidcfi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yehiahhn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jogftjts.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ekyxfvjp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jlekbyie.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3klscrjja.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nfavogrh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mapdyfxa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hsltzwwa.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yikpxirp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kddwbgip.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3imdbntsm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pxdgbert.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zcwowaza.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mktdtdbc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3fzsdxkpj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3znetapnl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nzblbxwi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3luviugpg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zzkdvtcb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3npdiywpv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nxqaccgv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wxzfcasr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzquglxv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3afynjwob.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmlrvvbj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3babdhetb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3trgmjqpv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3znbjsckm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3aztuailv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjcdwuba.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3koaavakm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ccivkwpe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mmnjdecz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gpqkmidh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbuanxcl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dtrybepf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zdicbbkk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wicquuei.html


<!-- 参考信息 -->