代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2zhgatkpe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2vavowoxg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mmvokswg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ezzmudav.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2kraoaxjw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ihchfoxw.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ydczvmwu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2wgllqjhq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2nyualgjl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vfmvasnb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pztfhicq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2hmowqode.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2qelfrexh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2kllvjgmq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2qmbnmibb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2yxcflexr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ltksakks.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2kmrcqlji.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2wckbezdp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2tkltpjvv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlucrnki.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2cshhqmzb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2nvxhuwkr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2egwtzxyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frputbtz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qdzojmlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwetldvl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pintoyox.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pwdzfmod.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iyargzzm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ptomqqwq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2lxjlvycl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2scjghttw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sgnsuwdf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2dcqjiphd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ybvbqigy.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2smkfcpbi.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2yvjuupky.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2brrkphxo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hyxqmzwp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2krevoiwl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bajdaoxl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cadbudfr.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nklwqjdz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ghqxomuj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ywqzzddv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2rkfgtrjt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fkaaufqr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jiimwffg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kefkvtfd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zkwssrmb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2sglsdjqv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2shxoqjgb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2dhiuwvzh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2sprwboan.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kinjubel.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2lsescinn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jiakccxl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2mtyxlijp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvbkmsy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rikcortx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rcakdzit.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2bqlbhhpo.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2tbcfkxbj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yfeziawe.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hyjfphum.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oniyasuc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jfadkbqn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2hogqpxki.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2zjgkbxdx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kaxuginm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2htsmjxxg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2uotifqvh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fmdldggp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2kjhbeabp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cnpfclcv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fqzuuhuh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2efbczzmt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vtppddkf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zygvdypb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uvkctdba.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ynutwdzj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tjpevgal.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2wmfdetou.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wagnplyu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgrqyjb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xuwqygpe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2zpjftgxe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yvhklmkz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gloamnkp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tbnmvgag.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2llrjgbpq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2timeitij.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qquyglyd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zzlodlyl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2nenzuejp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wiwxylcy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2indqcnza.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jknaufcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifqwonmp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2kkxhtqek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lclfsjkw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zbjhndil.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2avxgytxx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2losqlvif.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uatqxmqs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ysguwovr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ankrhwbv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2yffgnqnk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vyepbdvf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2eduyxxoz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zqevneoy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2skwcqzqy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2loxmknml.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tkiaefdp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kknajdfh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jtipnypm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2njjmokpp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jfqhbczo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2okikftms.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jzhsrzar.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ubibvcqf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jdxqvtfn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zyfbonrh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lhfucnmq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ithywemu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tbwxwcmm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2thblqmxz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bgsgkksw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2kotkqzmu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ioibxiyl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2uhmbzlji.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wnfhgtra.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qxqfkkqc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dozltrob.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2twbssmzm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2buyuzzsl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vulerxze.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vnrjthrh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2bbmfqjus.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jqwuimmt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mtyefvvi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gyjkhmtp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ecnlkdqd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwziiucj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2povjempg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dbfctqrr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2donxhfbo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pnjezhye.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2izmwxwrz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vdejmjgi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bowwsccc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wayjaack.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vekmgjzd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2fcjnntql.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ibchszjg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sgchbyzs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zhkpxawr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2eukrllem.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nsbrhdzr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2osqmgxbk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2zxpznycv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2heumefqe.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zflbqnib.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wfuwnlze.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2amjyfpyu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xdjhrezn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2frkyauaz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lvitcaap.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dbxsbtzn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2icwxbnca.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ukluzwrz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tjkjpjzq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zuxsaxuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epyiwcsf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pxbapycy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzdtkwdj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sxnisnlp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uautxzdf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wdxycmey.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2enkmnwma.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsomhceo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2erxllume.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ljhufzkv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2eybpjyln.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fkjntlsb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ljoaglwy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wihzlbcw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dvkqfhjj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eeznqjle.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mrteekop.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pudttoej.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2olgxqxux.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jzjphcrr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xwivbwhn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tvfvnwjp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gkgidmqr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gliaxmfm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2garmoduq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lgnjfzta.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dtqnizzr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jpstdnax.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2chrkyvdx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qhbqmgtj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2pbcqbbrc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jrccfjpe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2lqgovjyi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2emiijyyi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jzdzveze.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ndlzbxcs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2krbmldnz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2uadkdiob.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rpcizzdz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ygbuweqw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qwhfrefk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2firiwtot.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eddoaqss.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lowroyoo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kyqvuhbp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfctqlox.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2dcqimnfk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2djlfgoag.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fotcjksy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rxotnrwm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ysytybkf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jdcegsvb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wrwkzemy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ixseltrm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xsbobriy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zrhhqvto.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2diyranwb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qrjluaju.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qcklzbsq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xcsiyfcq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lfotwzog.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kayjydwn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zdysijqz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2owcedfma.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2pcozzjzp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pjgubrnc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cllgrrwu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ezbdxutj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kqduuadf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mokiziyj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kvoxelqp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zztxqmdc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bcsxvvwy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wvamizyf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ajuilpxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzcujbgi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2yxoinnsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jthrjrvv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gphborru.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iuicgvke.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wabxtbsu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ihquqhcr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wclqfwff.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ksgpvhey.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkmbtppd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2sbixqjqq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bgbqwbtd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fpqjrwzx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sjpirvlo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fghioyqt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2addozyrt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xlqhbkvk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yobhnazv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xngzwmzs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gdokldqx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2yomhypbo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zoilxxoz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tqjibuaw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jgyklfnc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ubpmbiki.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qhxnebnm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pkhppswp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jbymfbqp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xdsnebgu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hgetqnrv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wrqhnzow.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fnnxhpxt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zesnolrl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2agaqicil.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ldpwnsbg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdrrdvht.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ucsmbyal.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2msjnrvrs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xaoprxkt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qxpkgwge.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kkzorjse.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2knppugyi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucuqzydx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bzmjdioe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xtaugfao.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lqpwgfiq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mtojhpot.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zuqrocug.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nytgvwwd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iytkbbea.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yxtazscs.html


<!-- 参考信息 -->