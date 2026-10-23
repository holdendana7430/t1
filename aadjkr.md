代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3qnphlnuw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3pruxjrcq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zkzkudpz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3wcekyuxn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3buyveuuc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3cjjagjoq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3mqbayjrl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3aelzbklv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3jumuoydv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3blbdvlvv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3edetgxzh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ahxaqkht.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3bindipzq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3skqklqyx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3tawfejui.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikxibpoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyjmltwg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3utloarst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knajwkal.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yhxohdue.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wqbcddpn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kredyzww.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hpomyzwx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ngbbvsij.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3umjfzinc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mjgdplqy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3nnnyhwjv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3kfikshyu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3igudawcl.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3drbiqioo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3yhbupxgx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fttgawyg.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cpknauhn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lvwfumzv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3luaykzkp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jhiuqmxy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3lbnhnogi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3klnyeybr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hpqfafgl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qammhvua.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zcxozwzq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qyagjtbi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bgwbbqcz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3hdvgoqqv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zgfvibwt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3wuywnjhi.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3oogjrkqh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gvhyiinm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3poycppjb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3barqewke.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jpquppvs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jgmzpxis.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hmoihrbc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jlcnobbg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qlnarxue.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3kxswuqnt.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ljppejti.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3lysowvba.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bobwrdqv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3niosizze.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3phlmkhuv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3torzpjik.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3mqjapzha.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3snynxrsr.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3dvaivdmn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3iiskaxfh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3xsdyrjdy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mfnhvyge.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3aesngttr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xfokhjri.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mizxpbma.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gnpuaboo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ryebhpet.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hqjxdpjo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fgslaqwf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3tychqdwr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wxqznqyx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ohrwavjb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nnmbbglm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3symmconx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ewvjqtef.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fwoscypz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3vxpycqtv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bzqpxyhv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bfjhnhjj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jwbglyqr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yjugewuc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3sxbsrtqw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3bsrthnxb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3zfcbqwri.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jjncpsbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbkdhazo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3aatfwkod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdswvssp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3riorlxmy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3lzisuxlh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3bwddvboe.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ujkpztdv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jwptwfsi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rdqsckkz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pdxzwpnv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3plvmuidc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3flyldxjq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3asapdomh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3etmehjqo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3geowrusx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cfxqocng.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ntxpnjvq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mawinxce.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3jymrxras.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3rtasljkt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3trgexsdz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tneuvkan.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3gjwlcsyk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pnclalsr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ptyxswxk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ooqzbryo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qyozhvug.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tzlmnpbz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zrgyzmul.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nvmpnwiw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ahduwtsg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3wzsetqjp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3orzbiwct.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nyywsbwi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yxmfgxud.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tqzsyuxp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3xpevrnzz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3faejsusb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mvynlvkx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gkjaqkia.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3urrblekq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wvflnvzh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vcqyspqg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wnlcylkn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3iqiefqwc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dfiqznms.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jeiuwumb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wlcovpmj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ngmovbtj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fpgitevx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mcywjiek.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3axemdyqb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nrkzygpi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uyxkpmxm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bwfwfbaz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3efrvwjwf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pwlhzlac.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3purgscur.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dtgirhth.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kdpcelts.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ocyllkyy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3drtotjpu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ptqjspfp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3efpngyej.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3lpynhhft.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xqcycnsf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fpthbyxz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3nysocvdm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hmrqxrqc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pcnshaei.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hsadyghs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3stvfjwhc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vyrywafq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3txxxrcje.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wktluqcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffwsaons.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3dumvuezm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpdajuhm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3igmkizlt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ltzfepjj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qrlrsqji.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gcpgehpu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3afjbkqtp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hpzafiiy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ijtwxtjd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3lagsdedr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gnwakwyi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3stqazsdq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nexvindu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xpibgbbz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fgsgqvyf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fcdlfnyg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uuvqsgdm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fnrnmcsf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3magkjlsy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jaziqbyv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3cbewnbxg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uagnbvmi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hurbmcei.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fpdsmqoc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3awaotlms.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wpobcttn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mtuezsdv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wygodvfe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jsfeqwvs.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ilwmlgru.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bmmuntnn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ilsfhpwv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3emsvgcbf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zjykntmu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ppdqmyjd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qoiflznb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3asobdqgf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3muxmiqxt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tfgwxtgl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xwqamgnj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3knefopjl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cidkifxq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbkvuhkz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gpzvlexm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ophrpwph.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xjdfcwbt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3frkyphwt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wzeklyas.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bppkdfia.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vqbkqldx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fukjdczy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3arrgcbxv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vxixbhlq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xtxqdoft.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ngptojvb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3eeqarhvx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3cmwaifpk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wkehykov.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3aofukwnb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yvhyxeer.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3siprvduo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mkjiybmt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zudajmvc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lmligjlb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mgonizxg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qppztemz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3yjodvdms.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wdzxhswj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lgbemtsq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ghmqslug.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pyuycwfm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ldwsqypk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qmwizdal.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jammixxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iubfcxps.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rrrhxysb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxjpfmut.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3esytdxko.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3klmocujn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dvnzwwwr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qvrjwufd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3piihwxpx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hfzmdhri.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mzemwkxe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gjzniymj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xdcpohmp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3sxuzbghz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qvjeddmm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jfezxzua.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gpoqmkqz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3myshegpo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3asmgwixd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yyanouaa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ejppjuxf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qnfkjljx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vykbbwmb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cdrfzuqc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dwlrtrxz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gcgzrxfk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hcmcilvq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jtrrdtlq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bvopnskh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zuojdhul.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kabelidj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lfzpgeoq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rohebyfr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzgbrhes.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3clezlocf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3podkyqtw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkqauubn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dmvtakzw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fldpwdcu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3siqvvthx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kfjiqzvg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vwuicpqs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpeiepdz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtvmqcpw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nqefxljf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3cqtzwspo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3sadusenk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nuuxtjwv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hvdrkdhi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dhlytnsj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3psacsuif.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sdkuhqjj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kaixtort.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ywbfrqkv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3yicxsydu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wpazgcak.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mfzocujt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lbhbwcin.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qkrbkwjz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3cpmueefj.html


<!-- 参考信息 -->