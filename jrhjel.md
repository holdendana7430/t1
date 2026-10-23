代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3auahfhgl.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xndeidey.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3fxpougvz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3joywmrnx.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3hogkpmdz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pupfkjnv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3orkbdxpa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jfnbnvgv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3eeevgynd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3qgbvjyqg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3szmhpkhm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rtvoxqjs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jwnwjelf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3otiavzmx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3wfspxrdp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3eftgfhvp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3mwyvwivj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ilnlipxh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3usfzvdns.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3qiuuwcno.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ucndwssw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3hqfwxgzt.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3dtagolbj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3dzlnzoeu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3askyjuqp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3jotjtlui.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qbpjogjl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3lpnafgdu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3gxspwdpd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3rbjdcpdx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3tfajepow.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3pekxakhl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3luobpkrc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3jzwrthdl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtbanpdq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ahtsqehe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxslwors.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3jlxcrshc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3lladpzkt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3hmodizzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtrnupes.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3wofplrry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqmupxmh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3juyascwa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qciyasxx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pgiuyagn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3exvtulfd.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3abssjqfm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3rgsaihby.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ybmqtsoj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3fipoueoi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hcfcfrin.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3bnwwnrae.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3gwbfllvk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3meqnnhrw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3swzmqlvj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmwlkawh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lyheyiay.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3cjjlynnf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hlzbopig.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yiipssfu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3awtrspri.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fbyhhezv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ujjhumtq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzqcpvvt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jejectfe.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3yfgelofh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3syjaubuy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ztojqpfg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3mcrghyoq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3wlnnekpy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ymguzfsb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3odroiign.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ajdgydam.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ohummkdw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oepzywdq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nviazyva.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wdngvpnp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pyitxurt.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3sldakvcm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3glppfrke.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3mnslcwoy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ahsoyqrf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tieexupq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3txkwgkef.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zxtalbms.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zcffaxyv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3yloltnor.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ubysavee.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qulniriz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3pkzoxdfh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fokfxbsf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3irgwgnbl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3phlyafiq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3prihffin.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ujpcsrft.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3keryjpyj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ehpkqujw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ktkqpuak.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3avnsnslb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xyebmnhw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3atrhisbo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ptjilfip.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3pmtlbhds.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3tpvfgyiy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yczdfnrz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dbmantzw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3tyqrdlyz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3wdjerlty.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dzxspstx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3khlpuwze.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3tmjwhyza.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3acgnnsfl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qgjsijue.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xmfbzgze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvydtpqf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3fuocrjmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqfixjfu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3attuspdh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3lbrervlu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zdwjoelc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vdwsrrqv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3npnnpcwc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3nfhijgat.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sevhhdlh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3pgvozamj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3scyzhdoi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qfmgqxqn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3twtextkv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3zmrjdvbl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3irscyydt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3joozkrbl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lqhkmzye.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qhjzdvve.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ncqonrqm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vrjyrseq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zyynkjpv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ddocobrm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zyxxgwhj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ckesarug.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xuqmyeqg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bmspqgdd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3iuzrhudc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xitgqhyf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qzsqxlsu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3squwhqsk.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3otsdsitm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fnxfgwcr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3utyxxlty.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bqrnwwla.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mqkupjkf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3druyooqg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dqmnbdre.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ceyulwiq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3izlkvuop.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3mklzioey.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3iwqzhcep.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zzxywhff.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rtwgwzok.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rewxkaqd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdncvcrl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3vlgiclke.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aakpmodr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kgjtxjkh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ttdqulgg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xunagjzj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yykjvimi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wmmazhvw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iphedcus.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3pajaepoz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wpdcbuge.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hrsofajm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vtgbllxi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hgmjkcdq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qrtkyeij.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dqyttvqz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lqdiwmun.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jiipowlj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3khahsrll.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gnvpbmyh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mrxbziab.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ydcvgztj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rxmtrrof.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vwwvqxxm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jtstdcyg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uzfntcat.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3fbfnhrem.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3eahivlza.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gnuyhcpr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mqquvowt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzrkgwgz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kweqlqsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvwhqcor.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bjwghdwy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qlpbfvfq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jrfbcpvv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3erhyqoej.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzxvckki.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vioizgan.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dnixszbf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3yztokiwb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fkhchnke.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hoayefke.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pmkkhrrb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3woenianv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fimkbkic.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jgrmtdkv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wzjdmjzb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jqoydbgc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3pgbiebhj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3beflmufq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rrwqfmud.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mpepzrln.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fvvcekel.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cdmpcduz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cwvmlhnt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3somfzaxm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3vvulvyxg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pxacppvp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dthoxwpb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mzxvgxev.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kmmzcglr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jojgtrda.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rquijhkk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gafjohaz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3lwncvqzo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tcwueiht.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mngxozbs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yxqdkbeg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3cykrrbgm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rdhfyjtz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3baoepawn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rtpxycbn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mbfhwhxk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dawktrnb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrxqshfs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3upjhieeb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vljpxxxu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jkpzjpgw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bflibwfv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zqkbcrao.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ylusnufm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tdqpwbpu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cngddkvb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3lhlccnjo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qathauac.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jbtelvhm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3aneckjcu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3esavoazq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hyryfyap.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xeyrzqux.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fcutlomy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vsfkbyre.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zcxjtxrd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lmslhhys.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jjvrmoie.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3loadtlwl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kibtyhur.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3xcvddcgm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qvmlutem.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mampwbwg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jihlmkjh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tkuvsmqq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zgbbxtco.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3famnjnct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpkvjyrb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3nhlndtbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfblmynz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3igalclwx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zrciyshi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dvjcjlns.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ynzuqeki.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sbonsjas.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mrqvkgaz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qabvsniq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ymxtbwyg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nlmklcst.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mbvcpuba.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3efaymzsw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dwxwvtyk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3usicohki.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wyziujxz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kmehwoab.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ewlefhcr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vtjetfei.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vrgzvatw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xvcmryue.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3aqimwuvt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nseklwyf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ahpmbfqv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mwljtgxc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jkvjrfbi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3uknxyvpy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lcwaxsmm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rrpsjlsp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3hkammxdv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vayhxubu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3oadbdvfh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gblojdqs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qfjxrrix.html


<!-- 参考信息 -->