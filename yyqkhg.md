代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2weopejdc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2gtjfprni.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2tjpsutik.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2fpvghfmp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2utisyxyj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2pfbyevof.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2cjddoxyo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2kctivxrw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2crvzgshe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2okhdjzsl.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2lwuxjlge.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2mpukkous.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2njedwtkq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hyaofxtd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2efefpokc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2thvmplih.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2kymlclne.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2moeauaxp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2zprpzbfe.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2uyxjpaxn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2puhnazfw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2tccihhpt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2xjpiwiui.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2iaftmxzx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahkteybl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2axusxgte.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2patvngyg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvrhsehu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvtumdxx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2grcpjuil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afmgalrn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bszzyslh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2kqzxwytz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qcuriewt.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2suelbomf.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ghmsvcvd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ztmwhwce.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zzppnhel.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2pmgprgyk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tedtbxgb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2dytvoizu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kscblhhr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2drpkonvk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kdkvqcey.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwhjsyen.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zeodurzp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2akvziycc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ocjhkyqw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2oczeznvl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2qlqxjjwb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pkctrrxp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jjvgqavt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bilchusi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbiaebk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2uioruumd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2dxqsmjna.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mveofrtx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2bujaefqz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2tiqdpmyc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dzwxvqev.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2iowuylby.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jlbuqbrh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wknpcwnu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gchxkslx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2urqjgllo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ndytfmhs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pgicmrpj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ywrrgjag.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xnlnxssr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2jhtqdwfg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2etdljorj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lgbwqxxw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2bkfrypzc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2idnoeegp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2rcdamlpw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2kbbjryij.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2fpxvrvts.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2svwrssfd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2vbgnnjax.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ezpwconh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2bkuqovmq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sklyivva.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rdjtrtwj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ztqxojie.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xtiqkpvu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yunjmmzw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2srmlikgg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2lhxrnssz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hoacowtn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nnvfihla.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wwrqvait.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mgtcvfch.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ungspyma.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yidufkga.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2bxlwfxwv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mxxuomdu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gqtnlyat.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2owsyzwym.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2igokqlcm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ocysnhdi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2fvkywgeh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ipxeuvdt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cgsdqrkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eogwdmgl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2nrunfzjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbyopmbe.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zmcdsfcu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2nrnmhair.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kprskfvn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kgiupuvo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mvljrceo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mjrbfqlb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2gmqfbfcz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2pgmwzjlt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2noaklvig.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hywawsrg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2bjolalgm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gdbsvojf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pjzckbya.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mlzmuisx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2hiekjyvv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2gocsebln.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fblijibu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2cmhdmjgd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mzttzmqm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jxblnrdr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cgnaqzfh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gjyjugrd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2elsqlwtm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zxosoerl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wmarohml.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ukvqexgv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2leqdfpxd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hkupaxpi.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dgryiezu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gywampcm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dfpmhrjt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bulalens.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jesaidrv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2anytkftm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2klzkfiow.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xhyjsjzl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ialsfsiq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tdgvkgls.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jahzhkyd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xfrwkhsn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lkyqevkn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2dykvggcx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xjqebpls.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ccayntrv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cilizclq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2irozflsx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2emykaczs.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jzgestcw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zbzkhxnw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qhnlzzhq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fpuuikca.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2gdwhiypr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2arebxxsa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wtvxcgci.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ndzdtske.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2bnxutthf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ypjzzjxe.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cqotryjv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2joeuwzzt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2noroltnj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fxkfrxqd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2plheuhyj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rofyxpzv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2yfgdzxkc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2uqldrzxr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ibkvglsp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qfaqnore.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qaufupkd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2nwrmlgir.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ydabdsvu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hrqysduw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qjdnmqcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nudrhflx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gerftnvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzzzncce.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2heolhsrz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2euoagbpf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2gfreuche.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ewpkulka.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uptczwci.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nwwdrabw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uvtxqgly.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2vklbbrdt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2idwvohqr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lgocqaus.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hczlbyfk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pyrpocnm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2afrvjoms.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2krzlslem.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zhbwnmny.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fykptccg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jgnuwrwy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vwxhgwpe.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2fjduhdvo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vafbhrbo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2oaoeqcba.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cljgkufx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wajctbxv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ojxufqeu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ftnrlsgn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kdyoxlpv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2aujudqai.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cdkfoekv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yrkdumwb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xbbsbiyu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ipejnugg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vqleqroj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xmilmenm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2okwfddzf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ytdyzhie.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2kfmzjphb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2harozaxa.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tzfaaehy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2orydjdny.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wguqgwzi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfafsjys.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lyzcxcwb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xdgonxak.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvwrytxk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2sbotmhqd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2isfoccdn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ytghivbj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mwbycann.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rizldkhl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fmqqwupm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fnckhwsb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zblkrvet.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ovrliidy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2owjhfinu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rqutvcbm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2angcdrdr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gpdgbhhc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hopobvaf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qytovoro.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qvrvhupv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2glizxohx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2uxbzvyvy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mtvphlhg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jaqytzli.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2whkabqop.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ztrjymhk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gabiogll.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cylwhmvr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2nrfabdnr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2etrngsgq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yxqacesv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uiyfsqwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkecvkft.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2krycohan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpjgssng.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ictathke.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihwtuqkj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rzzzkmef.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dewvlqbx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ftdylnqo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajimicgw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iljulfym.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ropoakwi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnlzjpol.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mdnsagvc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mofhkwcs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qoedngjv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sggegtcl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tnxmyocy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cgziyjyo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fpqewjae.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2llhocyso.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hlipiqkg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lmnvmjgw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2zhdfzuhp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bcmkvzpq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gdweqfag.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2epiwqmqz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pdhnvfns.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vlevyyvo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fcblalcy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ftherehv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2gkoodrug.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uzoeevvz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dtaihhba.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pvsiyzol.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dwmpdukw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zipoiulh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hnojswvu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywymcdoy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wvimzeuw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2otyjyidg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2syczpezs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayfqyape.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjbkzwrs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vwljspcg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rlacnrvp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qexagmkh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pebupjfc.html


<!-- 参考信息 -->