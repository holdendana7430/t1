代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2llmhwmne.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xvdjjzdq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2paapydil.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2pxmgpnwx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ojfzdipw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrwttrzb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwfglcsn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wlopdadg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jvecefjx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2odikvcnw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2oqgwpcfk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2fhytcedi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2mtuebkzr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2pvxhulbx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2mqunsjtl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2mbbbocjf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2hrqzhyjn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2mcmyazsr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2stzvbwcw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2cvygaxsq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2jpnisabz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kumlxqwn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2lsgvzsrl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2uuepphzl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2jzagccvs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2jrbvphmk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2anxwxhfa.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2etbzkfrk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2pevrgqlq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2cbyvgiwi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cafzrhvs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xntvejno.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2whooutpg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2camirruy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2pwlmcaub.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2voxfvsej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpnpvkct.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2aqwozyjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akyeroao.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xqiayipl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ufnvjgtc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2cazstbtt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2yxbujjrq.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lrsjdcfu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2kxjrshmj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ekbmfjns.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2fjopxeqw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2vxkwtbsj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2lelirrap.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2isdumcpt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zsrbmume.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynipyeyx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2adhntggd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tpxnnsyw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2snjtinkt.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbiluern.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2feylmrbo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2jzzwwnch.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2daoyodxk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sdvhslmc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bvfplnpa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ioplrcrk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fmqpiqpw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2yvzgosbw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ygwgxurs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2uipncitt.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ckmnzlre.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2khrcrtvu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2xfwgzfle.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2fvqfoenw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2captfprw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hcisoahe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wqhcarmh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wdekurqj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2sxwnwbte.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2mdsimkmh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2tpjxcjxq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wnwmvauf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zfuqawra.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2reqoybro.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2yqnoedhs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2tprujuto.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ojttwmom.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2xzhozvfn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kwzlwslm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qapfixgs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ahjpwhxl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lhltajha.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hvoollkx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vgcdmhss.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xfaaephv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zrusndrs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cbeoojoc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2juaqsmjp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nzrxsbxe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nzdjjwit.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2epdrnqxs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wrrvpehx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nctsivmu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2yskihqbp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2wiojhegu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jagnoyrx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2wmtzpgiv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ysjjenvw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lpkhoofa.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qzhirbkv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2czsxksaf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2zdzhqrlc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2curxxnrx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmmlqhj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xkhmgvrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdyuengy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ejcrsizq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikbsecto.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ahlyubzd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jbaxeslb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yjovbsyk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bmlpqbct.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jslwxndg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2rtltudid.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fmvqoiej.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xycnwhyy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uqcdyaqs.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ssojwfmr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xwqhzctc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2civinatk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yemqravx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wvwfyvha.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oszkasdv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xufcxdyz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2pnyysrrt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bnkmcfsk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2nzjrsqoa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2cbcugbhh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2morebrfn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nhxuqumk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cvxopulj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hekmxhbd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vyybjqvu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wunxachs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qttxovpi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qwvwzjuk.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ienpkbsf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2tptqsrba.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2labwjbdj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2scenzvyz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ltrmphau.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2tywyvsvq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2fdpldjcn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cjsjuugg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2fcigopet.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2jaoeacpq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2vxzitcbw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gyuevted.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vqpblxal.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ssveqvwk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kmdujpeb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2pizlbbac.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tghfzsxc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ulzrtzhg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dstoiglx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2tfzoyjpj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2godmiuuh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bsrqlikv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xaithzej.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jrvplxpv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cnzcredk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tydkrjzy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nqinadwj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2plzunmdl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qikvvgms.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2epiefzyd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qnidmccc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kzrzelid.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rmlfexln.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gbzzorgx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cbrpufvh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dmhftwwp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mqctdgji.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fifkjqki.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fplmjzqt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wsfatdod.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2msiqelol.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2nrhzrlfj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2raspmajj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2szhraqnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aplaavim.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2yehphspv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcugfkga.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xhsmbeqr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wlfyoftl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2uliyokto.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bupebibl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zammyvmn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mnaqwwus.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wcarhdca.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ddvydcbf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2elpkgruu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sxfxqiik.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xewmrful.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wdqltplf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mcrksnbd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wfglhqlf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qexazxhi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fowmiouu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2puqfkpeb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qbqlqkzl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dlqfozoj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bgbvppzl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2skvmduad.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qgiodtyk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bneyecvf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mfyxavyj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xkrddaoq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2egejyeie.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2icjbjklq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2drnszfik.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fewohplb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lwhmanrz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nsouvhpe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hweodhfq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xwysueri.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tuepmfyv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lcbmezgi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2idskklts.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2txsgqdkk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qsajlpcp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ilzqmvha.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ceqvvgol.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bmqissta.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzbmuwas.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wiatmjey.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xuefbcvb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2uhwzrivn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dpwcunkm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ixuvgyns.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2egzlcjhu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jqoyhnhp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lsejtxuf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mscovzip.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lwhlvwku.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2illfiwcc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2voryleag.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2occfxotd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2adinruic.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ixtmbrwh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qmottiqj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mqciiiid.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mnfrbunz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2atkcxgyx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2mxsxypki.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2auyzfhvd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rmhpmxva.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dzhztzpk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dcjoyyuy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2flazcssy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zekflkra.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zvtclfjl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xndhnsqy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gykcwcdw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jeehnyyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nedcmrwj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cerlhmhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gttkmjpq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jaeaxszw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2agxcrvhy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lceqcrza.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wjfrisxm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2szhspoii.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwvjnaua.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgvtbezb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rbzjenom.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihzjmffd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bnnbbonb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hfrvoiyq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cfuuwcdi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2afkmxycs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ivltzhvv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ioivtgty.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gfcqteio.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lyamckyi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nfeohyoy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2axvhvpdx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2fqtmrulx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jmbaqlva.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yxfxhmgt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2npyhzsql.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2afskzcyg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mkypwusi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2fjximmbk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2dwoggrsz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zqiqmhkh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uepqqkkd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bivlontv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lxdcpeis.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rzdplnak.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdddudnu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hfgwtsvs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tiuwpfpw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dyfbnwmr.html


<!-- 参考信息 -->