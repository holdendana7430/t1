代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3tlwplbfd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3plwmtjyr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ouxgbwkp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ctmexjem.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kdgewjoa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3wmhjweiy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3tohnpzzb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3pdkfpsur.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3noypiuxk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3eltemhfg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zeibslqc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vdzqmvhx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3yqeehktf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3rotjdsuc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3eawwnbid.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3vmrdssll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gloawvcn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vsjeezdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwazedsk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3cifaedll.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3nbgyoxbu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qgppvwut.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cwogxlny.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3neozxglg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3zgupxkkb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3qjustyks.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3vgrjgphu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3nmmnznzn.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3magpsqhd.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wwoxvnnl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ycasrhgz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lryzdffg.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gvmwgyzx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3duvvochw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ybeqrszy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twytffji.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcjrnkce.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rislcmfw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3dicbrvbh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qvtaredd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvgzrkok.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jtvqnwen.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hxtyraah.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3dogxyqsx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3npdxbqlq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3xbgfpzyj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3muxpvopp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3lbocuurm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fjcigqgl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3cpcybdkx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xnzzchzb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vvbxtrxc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rzpgjnnh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qddwmurh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3baglupla.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3mvlwjdnp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gpoivtek.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3urrjlkhe.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eexxhzdl.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mlsfmbdh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3fmppmlfr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3llkijnot.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ilscqmop.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3fmvrqhtf.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3hqhbdpbn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ksvjdwsp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ijafsauw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ieqdcldt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mvqrcxmq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3yzolakhj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ntdakwcs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gnrakgcs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3llfkcleh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ujiwpkbj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eslnhaod.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qwxnsztm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jmlfogrl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jnslmqwb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nygkiiqa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3featmkjo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xtwvywze.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xtlqmnkc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3uqjnurzb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3kfabrztm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xvcpdsum.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hhuezohp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qqnqahvm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3onukpmab.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3pizefhkm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3jufpvkdh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wfrkuklp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayanwbyz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vvmhciec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3titgstke.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3fycupqgz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3qhxpemvp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3oijsbzsg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3msnvnueb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3irdtxsrp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3srmazqfw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3eapztjwf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fyvokprr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ajyyfrpb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dfpaiehe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qhgysaer.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3myjdslfr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ppsotbrc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uymmcwyo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3juewasxf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3lgnrtpth.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xyfdpjlr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3awlkpugp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3azqxhanf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3extoynpb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hcwflxvh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nopwfoag.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qhvivrux.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3yxdcsdjl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cxiyilna.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xwsgjrwa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wrsbdomt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3daxjosgh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3kmatlcqh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3scpuhvae.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3unepdmev.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rqhqlvza.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uzrrwpgb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3iwuslikz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3wxxbqqnc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ynstszhy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3iukudsgk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cfquiqhh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3nhjduxgy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dahoeyns.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3sqnopekm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rxgyjjaq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vwsuxjcg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3dufqialv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qwjwihes.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xdnsqpbz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uzryunaw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mxjskxof.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jwdhesuf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3irhryfhh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ewdjqebo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ojlcpbvj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ooujlkdh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zqmeekct.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ebfkdevs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3nmpsxsab.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nrhztyqh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pjnipyzm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qahxcbem.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3rbmjbqaz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3avkalqxq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jgjwjdxm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vuuipufe.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3weirject.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mzcjmekp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wolxxjyn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3abmhxnoc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dohccbiq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yypzxucm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3aqwhzbyg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gnbtpeva.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qwdlqhrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rweujivy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qvibgdyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntjknbws.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xutaydww.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hplptyhy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xqospcxt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zaubrdpi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vyvydigo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3sjckgado.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bsracqyq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ihlldedo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3otmigooy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qfechrub.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hahawvru.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cgbcwmbm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3eiatwqbq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uppmrzql.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xberxiwr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3akxcrdzx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3iktbffyf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vaczxmgj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3eexjyuer.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mdeglrmn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ltwvinkp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3inkuknoh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3riijajks.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ejwbqcnq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lnbgsxkh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qzujhxmk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3tigtdskh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mmwulyok.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3knknuvwc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3apdtphyt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vribdlvw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tltldyfn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fhlarxyh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qdexlgaf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tnxwgudy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vjgfukvv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3iizzqoyf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3spkmoflr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3spnyckhl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzootlki.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gatpgxzr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3icarinbl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3czrspfzx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fxmbujak.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3iaxhwrix.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pqpjgvao.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjsmswu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3rewohzpn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yxwuojjx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sribawmc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qaeerjpk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uoxlkrwm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ipnxcnhj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ebtfcnsa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cnrpcwgp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3liunbxqs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tgiqkkpi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sugfslyo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wvsdunfo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tarvoner.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3iyejzksn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3swzxoiqe.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3itweszci.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mqteksuh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vwzvgktj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3vbblhubl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vfnypjaw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lfyvjpmp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3seufcqpa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lkkqlhmm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xotcmdgg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zouonzob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqvpjbec.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dwrfjgir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thcebzsp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jtbasrgu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3muybvzvm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bpmbpflj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bfgggioi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dqklqaxu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xowzovkr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wgamlxcb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3lfnkkqrf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3unpzvdvr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mowbhwhj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mzyxwkqc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jiqvrduk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3suhkslbg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nkvqvzej.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sgidlbfz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wwhxhjpz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cxxswwec.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jewcfqzc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3egtujgzw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xagckptj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3fkknhszk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mvthqtnh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ebwyeool.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xapmpmcg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3taptcrqd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3adihlohn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3sttiokzb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gakdwicd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vusqsppi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mqmnnjcf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rkbnbxoh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fvmfdfwi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hgqoryhr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qwnwqolc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gripisun.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lrnqwzsf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3urdvbuzt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qpqreczd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rvovrrrc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3amuacdbv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ncyqtlov.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3roeiyepc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xtcvubuz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vdhezkis.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfiuzcjy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3utateffw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rbgdzapo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uebchtpy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wufnlzve.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dxcpccbx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3uoabujej.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3urjgbujz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nlayqdwj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xaqmrlmj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3veiuuair.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3eougqakr.html


<!-- 参考信息 -->