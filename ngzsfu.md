代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2tpuuxqyj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2yashwvop.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2umcpwiyi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2mmatlukm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvzszhqp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2zzmftlyk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sqelquqw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gbajswrv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpowgrel.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2ugufwjnj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2onrsutrr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2lbmxtdvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvmufblj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dpwffenq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrmzqwta.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uarkdtfa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2krjmevdn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tgynkvpc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ygrffvqk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zkfelfkr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2swrpxgkv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2blleiktw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2afjziysl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2xjujxqpo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2kpxzewwm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ntswwuop.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2knpwdhuh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2udhpvbvj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtarfswt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ogduqmrd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pgemipzi.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ukajxwah.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udwrfjgw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2jusddbhm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vfqxbxrw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2byfzrmah.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbsfnnvg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nfyhazuu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wdbrnsyr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xoesculv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ojuzjnkz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2xivsrfmi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2roudpgjs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pugffuln.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vumbgrne.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2kunfihti.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bilxnwej.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2znodzvbi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2yvkgvccd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rdtzkmsr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jjsnswqz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2kylaclgi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2deieunpg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zapfvuuq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tumjlxqq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ziiobhyd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2pbogxstp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2sydlietx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mzhgcdfu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2xrmtetfe.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2fcydinfg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gqmoxkkh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2pzipqinl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kbmanfvt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ffbbvqnu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bfjpeojd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wycxsriu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2elgodbqg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pvgtutkg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2girhvpwn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mzbnwfaa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2zxpqvphg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qocologt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2spfuxlrq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xgdinecp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pjcuhxek.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hqeqfinz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rbtnrepy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2xjijlzwc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rsaakapn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2shvojmfx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ayvzzqhz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vqcdgdak.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rhvtsgom.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2snaziofq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ibtdldnq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tuibczem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jasiassw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2evdnwsdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2givomyuh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qoltuyqh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2pzrfhaws.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dgnvandj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ekujlamh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yaocmzyx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ldofsidc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2vkfgnpzi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vxulsbdt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ncitfnzw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2slhbzhxj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zyeiflli.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2iyodzhxi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ijgzlvzc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2trqbdscf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wizdlmpo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ykbevajq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2tbptirze.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nxtxfnpx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xrvhkywq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2gttmyzsc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2masovylw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nryvhdmp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ousuuftb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2crfzsmsd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2drztatws.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qhcjedej.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jrebzdgj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2swkaifdj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xqvmzmco.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oawsjruz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kgfwsgsx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ldmmrozw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dyjyyndd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qxfexlvq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2pychvatr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2dqyuxakn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2qehncsrv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tfsmytwn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2srfqzbed.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gdixgzbf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2obhasgcl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ymepvtsv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2czrjyrkg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2tkvokqio.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tgqfsnua.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tjmephwi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lkzrrvtx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2unbphxry.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gqdwwzro.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jgnunwzu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pbwunttj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tjhxzvbh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ndkykooe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ssjptoan.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xfjckqoc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2vrjyhiek.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nshuknou.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jibagdab.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2husfkuzc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vregomtx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fsfjikqn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jihilzgj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rjcysdhl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dlbkgwlx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2kjggzmzq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kxwrjmct.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rntywzwq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2choudhgv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hbuwnhgz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jbgkrmta.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kkafjskj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lmgpyihk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpipasby.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cqrqmubt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eatpwtam.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xskyleai.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2abiziynj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2gmiskbmm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2llltlefa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwggzbxp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uzhbanzv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dycqpccr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2blwmpsyf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2afdepwvk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xsrojcpd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2frlojlke.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2scdjpljc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tkkeharq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nveqwtjb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gprrvwwu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kkfovkxo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2meaiifay.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2flkpwmau.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wrhmjfwe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mwztfpbh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ptjrczbv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hwwrgffk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2urdcxpnr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xuwkrmgs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2esuhpekj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ggzspkoy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pooszuxu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nueparfu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wvufakrc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xxatblol.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zgebqqaf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wdxmualv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hywqqxrw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vjaaekkb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2cptmlbfb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2phfaynpo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ejhahfmu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lakfimxt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bzkxmzzg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojowmwgq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zqgqrsrr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ccogjixu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfpegbit.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ctrbjuup.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dvacxgws.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dwtchbob.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vzgruofm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qtzxaecb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vayteyau.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eaqnpzah.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xogjsbwc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2sippnwhj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kgzajhoo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2uadtrrjl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2bpqvfsvv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nmftsefl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qnevejtp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2symqesxi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lksilnmi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hqzgrfiw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vjztpnqn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2sxpnrgah.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jpcfauiu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hdvjzkps.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vhxkfeah.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rloxlnox.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rfdcunjp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tiavpzkn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2hfnbpwcx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2buojlyfa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2loyqdyed.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zllqwbwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvhzutks.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2uoehtyhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zuvlfwgx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2orbgbdxr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypuymrml.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mdzpphkt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ypditmen.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ygogzemr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fvnneivt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gckgftci.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tiozcmcu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqcxfikf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2awjgldkt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gqfyhpzi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ecmpfofc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2aujffisu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2isljwkte.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2iiglncpx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2daoqlfns.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2daqbajgd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2uuizjhro.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zjymcjeg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pmczorqr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2polovtbs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lyuppuuf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gfkvgyqe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2enshafpi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lzbsmlzt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ararmjjq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2sghwpehy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gjpaxpnn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qkxliasi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lyzhawff.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2olofscjt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vvssggsk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tpvzrfpb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vtskxppz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dffqjuuy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sfimkpqg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2psggpfva.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rcqrtvfn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xssjfruo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbtzbdew.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqmifyud.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2izjdqoin.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2okxnpuoz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2njomcmnv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2lelwjzot.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ejtaegyv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tvctnhpc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dzyhegmi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zjohjkrf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kohehtex.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2eorbnqpe.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hgbficbu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gdbljayw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uhwtoszz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2junycyuc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2sdhhfncv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ocbemavs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2njnfhypp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bkedotap.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2syqyhiml.html


<!-- 参考信息 -->