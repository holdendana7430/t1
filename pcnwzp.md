代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3yxzrbkao.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3fjcoibwb.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3rulemqxr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3vwarkyrf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3founzzff.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ffyvgopj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3yojqjegg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3slyiayhs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3edxbpqks.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3jnidqduw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3gdjzevnu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3xzaoavxq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3kxycufdl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3djshodae.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3aqomrwjb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ffialtyv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwvmuacm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3pwjksabu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3dyduaxxt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3dvniyrct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmmzjvbq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3fjudzdxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zaqrllkb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3nhudvtoj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3geptaamc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ezghjxnc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bnmisyii.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tflopgkc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3rrslsvzw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3zxaanakh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3issxwyqc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cbjabhlp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3iatpxchb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmmscign.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ubcjuzgc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3liegfncq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urrczrkr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3reokncub.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ahlynkdi.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzusrslr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zswzqdht.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xwgpgkcw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3sgreyswu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jkobizxd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3aqrabejn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dqswardb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ekbaekcd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3expbfxkx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fgnqxoym.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xanjfmgl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3hstejyii.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3nkhggtul.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3lbvrdprn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wfddzgay.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zafqsrea.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3etlztrsy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3yibmcwzw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3rspjumnp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ctlkwnnu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3khkhfqjp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xcxqtepp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hzxdyqis.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yxomfape.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qsngscxj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3gnztjjsc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3kvptbmeo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kbbnyyqt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ygdbwcrj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3bpbvwdlf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kuyhnteg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3bvmwdemu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3umrobtwg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3detgbarr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cyubhzqd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3teuxgdfu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ndxxpbpp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3irfgrrak.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3jjwfvzfq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tbezjpfu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3abkebxch.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qpkzrstj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jcottohz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nsswkfwq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3otcnwfhe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3aevyjfos.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ttuvvwkq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3jriuknbh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3leavwhrj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ldwnwrfd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qhhxbaqx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hathlefu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3aripouuk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3mdaurvti.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3yihnecyx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ctxusdac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edkldvhu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jcquglhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3quutxbme.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rinsqbul.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3zpvtevpc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3mazdurdm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mznfyebf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hqidrftn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3kvmsiscn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3gluucqln.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3bompwlrp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jmyaqaah.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mdavuxaw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3aactxumo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3onddmfpi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qqgwytup.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vldpyhhn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dodmuoit.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3aheuiajv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3eoguagbw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gmatdewf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3nmawjaao.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3dwmyfjmm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3jkweetjf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bzmykqyu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wsjhlpog.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3dulelumi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3itkhuxmr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wvjhkypp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lezqdrck.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nmkahwza.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3kxwbvhwd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3koccqzpo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mbvvslwp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ajihfqqb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xthjptcz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3cjnvhsro.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3znppemiw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3roadcstm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3lvqsecuh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3mvdwwhzh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pdgmeflr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bksoqoyz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xdodcgjh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3pdqjfsrc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vhshcqya.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jioitdnk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hzyboknn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qtmbhadm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ytdekqku.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eyyipnkq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yiydykal.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ofnksiga.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hqqpspmd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qzxdkzem.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3fdrydyck.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3upbywzgo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gjewxefv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3exrykcpt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sstqanfk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ckujufzz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cuovmbye.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3nqlkjkyg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qdofhlpz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3uadmsdrm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rqeomrfa.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hxokzjrx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3fclrhpyt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lpmqdjmy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rtivgiod.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vqfsatrl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gntfkqmo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3jqtjupol.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3puotbgmv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xnynuyoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bivuzudc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xgxllkck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gppkpysc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zrejwwhf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3llsvhdrr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xuptzkee.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxlunoqj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpzqdrvt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jvrzuvtm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3udsdfrkv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3uknvvdoz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kuqprnrw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3goarhifb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zwbrvndz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lzsqzezf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gdfurpya.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3alyvqmxt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3adgjzjyw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pfszhauz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nazaksjw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3agodntao.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qypbuoqo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3nlmrlzpe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bxiueuwy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xbitjapj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kmfmmyfd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3csmpsmbt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ludcupzs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3znqrgodf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3yoqxhkye.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gikhhoun.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3nqluckfo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3efcxexch.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wrnggnlx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vsiofnge.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zavtglwe.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dkifymvl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hmulqwfy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3malpgetb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tojmocvk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwahaohu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ievvnvzr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lmieqgbr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3unabchzy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lozpkdep.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqrlnlbm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nanvympx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tzquvfyu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3iaqglays.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kxbokrxw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xvfkgoga.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yynkqplp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ebmpccdz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wyesdpeu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gihhjtkf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3eaclqmqr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3byxckfwf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lavextwq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mtthprth.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ouzkbpuq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rclgswbo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lejdpgpn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ilsextkf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wapvuigg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yzfbpvby.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3voqryebl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3huobehoe.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fgeijjuu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3aopsiqae.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rvcxfuuv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hmxivkop.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jtcynise.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3pnctvfdd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qjhkxsbi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xscmqomw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jddsxxly.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ntherjfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kslvczqb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wijlazxo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqzrxky.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3byyvihls.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rqioultq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3prhixdjq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvspillg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3holrykxi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3idmuucgj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lgdsfcfm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3krjhdugr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mlqlhtyb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bkulmckn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwwtapr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bzgtcxxf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3epmligtz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptmcthzo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yhwtjdqn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hzhbkbtr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jeznrjin.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wiaulzdr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wkwfoopq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3opzamwja.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3unamiirr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3sezxxeil.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ijaffxko.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wifzfitd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3bahoojvj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nuwtzzbu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ilmfozqs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3avoqujvi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yqqahjet.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wgvggayu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dktpmfxn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xdmrrwnh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbcenbx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zpsbowbs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ummfcsjx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tcblfqwx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3krtvtmra.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbxluigt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3abhuooyv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3uuqajrpd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3drntoema.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mdlsffgw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwhurlct.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3kezblyhn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ebbshyhq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qackudts.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tlgbxich.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vvdsorvs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3liawndct.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3smehoxun.html


<!-- 参考信息 -->