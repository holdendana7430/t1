代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ukrygiks.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3nwlyhqiz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3abqlkhhi.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3kucdjebd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3zrtvjdlw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3qxbndcsf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktgcgkwh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tnweiyjk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3tpnvyhwk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3hehdpsax.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3itzehuyw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tezqjalv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3liqxjsjv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ouiubgyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fignvvvf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3nqiumwnn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qucrcvxs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3tcsaqwjm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qhphqhcx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3monxixkx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3bbuetdvk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3frwpbrec.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3etxulcdp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qermtkoj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3hhiyxjer.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fcczvoht.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3cwajolit.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rbevncdo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wwopcigw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dlvwcbbw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3swaujeum.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxliwbot.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ltlydefl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xtddtaeb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nmqoznmt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3sxcdhpvs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3iedfuund.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3idpopmmz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3vutjqpud.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3kxxlmxgu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ablcetih.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ieypnwdz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3lkzrqzws.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3liwtxqcv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hxsarzmt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bklbzzlm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3grmgctwn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wmckeyao.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3lvssosof.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pwjghjit.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zymykein.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3fxobukrh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lymuyfoq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nrnqxzpv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bnluinva.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ewvwdpuw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3gggehmro.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3saqfwzuo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3gvbwgczv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3aslijnvq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3omcichrm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dafnhnsj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3smqxkqnb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ngletgin.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3drqyysnu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kzocoaeg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iceiniud.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lufobesq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zxuofxwf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3bahbkwpn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gnmgdsis.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mfsabnxn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqwzscr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ntmicfxj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ywhxzkwd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3oakilzft.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3twzjznud.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mwmapixg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3txkwxsfi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3rxxxhwoi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nhpyicll.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ejflexua.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xhknvufb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3sxtffnno.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3cqtrkhqp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pbesfgdh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kyhvkaff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pakypxcc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3aftyjxxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrsewdkg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mhziyjqu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ibkuwguh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3zsdlmwrd.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nzjbkfgz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3iujeffah.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3lkgqlgvq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nzemvujb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3hrukydmw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3utafjzpz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pbamcyot.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3urswlsiv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3anwnjxhy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nhqmvmro.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3yxpirlvm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3mbdzejyx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3tncihxhs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qxddyviq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rfpvosnq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yaxeejzp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fjhqippg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lrqnqflu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fiqewdqb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gjhsmxyo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ednwiwuw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dtlitvkz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3werxkbzx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xcjxsmyj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3aetuvkor.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3csmetdwj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3giozbknq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bkbnqfys.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jbvypabc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xqgwlhhe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jqmtfedw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3odeknrvt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3affszkob.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3uofbacoj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wigpbpww.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ixdeaxzq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3frgthgvy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3quognuku.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3gdlssbnq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ekvayzda.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3occhyxvv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3efdpfafn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3cyolotee.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3brmozbni.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iqlgnnhy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3euzkgerh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kmfzcdrq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wjhiyhwx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3thuswclr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hpjabxdu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xetnvefv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pdjtrvwr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kwqaaeua.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bojhleae.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uzbqqpwq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bfwrltig.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3esxaikjb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gyiabwmq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3yzcmqzhz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gxjlohug.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rttmxsfk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3lzjwhptv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3uhhbigxo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fgfxutwe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kzwhnvhg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jvvqnhcg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ydaejjvx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xnlbbojo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dyyadkez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvwwgltr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ajtnxbsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3curvvqyc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hmegdwfb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tiliekzk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mydxzzhd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vcdmaexs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3onnwaysb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gwiswwfx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dcvqdjpg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gxbxcjkq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bhxmdlhv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vhzocuxb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3itqkrnsu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3oduejgxx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kuzxstdg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xsthcamu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3aubmxrsb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3opsklslh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3uhbkyzbe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hvyjiphs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rnsaicjq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3grsphztw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3tghqvclk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nvxnsvri.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3comlpdpi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3nhquvqiz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lnyalelo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wizxwuyb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hgpyouck.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hizemshe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vdfeeemg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ymyoqicj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fcsxxalp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gbvnfsrt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xgdpurey.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hdbyvpcm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hvpfcwpu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3uhnykzou.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3uqrkqwov.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ltzikvvy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3blomhauo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzslnbsb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hlhayjbf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3efxspicl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hvqzdbdg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3szphnvej.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3itybbvkf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pljbxhho.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iguwwdim.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oklxcdbo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yyitfxiu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3snskkudg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nvqmqvkp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dxczwvys.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fobwiohs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3klzvdwde.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zkibjroj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ksctdxhn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3msesilzc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3djobvdbn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kgemfjth.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3bznkiacw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3aicewrgn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3baomqhef.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3pdxeajub.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zftjzkty.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ujkayurx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3lczjyijy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vrrceeas.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ykssbhxq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vvgzvtmg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3aekzcyio.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uoxlklgu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ghumseku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyubdecr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qoqfnpvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3syxfppkw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3eyecsqxa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqkjjqhj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3okiqoheq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kidgwsqg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3shqfbtdd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ddpryzzk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wrkolgva.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qosnbmni.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rkokyjxo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ckovrynq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iiudgjyx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fsxjzakh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3edgpgpmt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iskusori.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3iombfrhm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rijuybnw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ujbudtbj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ujbxxrip.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qukftlmz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qkllzqvh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wuaxbtan.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wdrtmmox.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3swtkpqty.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ktvglioz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3quyxbezm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hkescvlo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3flxbllqw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3olidvwiv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lvddnfas.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gezkfins.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lwrczosp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3twhmztgi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3twtdvsjx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nuzutmuy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ducjcjao.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rbiaxcdq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ihshcfda.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3agtapknv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ffrwrfih.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3iopxfksr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttdxkmli.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hgsuvoye.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3lpwplmfz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3timmwqvb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xudswkxk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ramtxuih.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rfbtbcsx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cvuutcvy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wdlrjttd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gdcndyte.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3hyminbxi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fcwpwtmx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3moebaikf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rmcscnde.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3thjlhgln.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3gisthcah.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3gcrjsmur.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kboeuexj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jxaaoczk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3vakhrhgs.html


<!-- 参考信息 -->