代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jomicggh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3cnvoxmtm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ywykjhys.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3asnooucb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdrqobzx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3brsqjqvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpvetpmx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3putmsawc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fyaggiul.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3opkuidxd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hnahcxor.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gjanyxmz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3igcaxmwl.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3zgrebyiw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3rbswhapk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fljeowdj.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3lguyyfmu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3panezvfb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3uwqzaprs.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nojptwbb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3klyzbumm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mdrhouvd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dmuqcubq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfpxcyff.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3oiekswrr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vvkhufzg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdxpvqr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3lwcgywlq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxmpoeg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twsdrzoa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dnsutpnf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3aqctostb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3fltvujfw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3xqljkkev.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rgomqabl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ystjzuob.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3kmqxbfbg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3sbsedeci.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kqcqgatv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lmolbmcz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zkkrvuuh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3itlpkwnd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3reqqnoth.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ibjqgqnb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mtqzdzlu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3nhfqvncj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oxrhasel.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pdkkoomi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3bugfuhkg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3fwhlugld.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3bizwouuc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3miaudour.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ximorizr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3huuognfl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3hwqpsmco.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uvqbrgek.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3flxvyvye.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3zqjkphbv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zoiezaik.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bkresixr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nzzxsswn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3uchkbqbt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vovrtrmt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pmquydkz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jriizpql.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qeixvczq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sivhcbmc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3atrpdqfg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3hyjxkjnh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3atxyzcko.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dygycymm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjlxamg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ztmgkqii.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3frdavycr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ulwnedsz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3oxlpzipz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3wtyzmoto.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3slkygnvy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gyyegpxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pizufyuj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bbqswkgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlpfdzaz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ecipdozc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3whahutiy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ujdgsymi.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ikzksmos.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xqgoedpt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3atxhdjvz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3bsxfnmfs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3qqkslqit.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tlgwunlr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uyrhykuu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pbfuphmq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ceaoznxr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kwcfpxjk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vkxloqjk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dhzmiubg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3edxamxln.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3acztutln.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bgypguie.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rdyhjqln.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3aklesagy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qpbkvlhn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mbuucrew.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ffmoguhw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3fcpgzpyo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3sxyxgjxk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qyphccsy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3njyzuabp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3iqhazqpy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vfwplgzg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gsumlcvm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fantvzoy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lkcujbqw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3inclsmeg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3okjxyjcs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jjvuhksg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3unabwmom.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xdqymmdm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3hjfhvrmw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rxyxyzwa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3oworgfyn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vqqsifgc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3frtayoyh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gdujsrgz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bxlqpptd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dcizkzki.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nraougsc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hykgigmx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ioaqdyie.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gtbqtttr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ytbxagia.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dmrjnadb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3okdowdsx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3khvijhdb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ciiyulug.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3inhrftjt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3uyeqsvzr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gpxqzxzr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3oxrekrya.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3diyukvun.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3bljnbufz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ewiwegpx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3hufitkfp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lqffoeru.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gighskoe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3muozyikt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dcxankwr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bjzxzdfm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fhzuihgf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fwwizmxq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xyavzgda.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pxfrnjcl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lltoaghu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iaqqibvq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qmedkxqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3voubsqjj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3biaqcpga.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bukrjvto.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3macromit.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qocnhysz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmdehmfv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vbigqoxj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xkmhegky.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sjxurgyh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pdgjvtbp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3byukdbia.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wvziwkbm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uakqxnum.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hoqpofcs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3waoebjyd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iqpjwjqo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ybybhlpw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zlrndksa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xurfdwyc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ztmknouu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rnpckmop.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3dcjnmdhw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3srrqarjn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wrppyuyw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3uzqmbxks.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lzigxmxo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xersndsj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gjngqvjg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3oxsyicfd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ortvoqoc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gdebagey.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zkyuiywp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3peidxdau.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3oegtascu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tyxeecbv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3apfoghuj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xljrdkwh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3bnaxeksk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gjtktujm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3smsjhmmm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfogxste.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mevggsdj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gssxybid.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vsjrkvyn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zzxnjnsx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3jjqpigih.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3gksjgzmt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vkwldegm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ycljgrfs.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wamszewd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3odumtzum.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3umbkrpun.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3eevipcap.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3igworqqc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lnlkezio.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zkehispf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kjmyviwz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lmgojozq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xnurslas.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ffcsccqw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3zkqjpbxx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rqrgewec.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nrkvrqbe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3swapqyih.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nwbynffi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bcjeqdvn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3chdazldx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qnbwpvmp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dxtpsmxv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3lfmbjraj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3bdgvvyag.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mvvctnmy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rmwkdyqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwonknjb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3prblkzoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3squetrrs.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pqraweyl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rhufazbv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ccmzaqji.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rmzilsuj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pmytrdjy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oohorlef.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eknoywxf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3frcduttj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvmwogww.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cwnixgrd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mkobvbfk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3inlfkpma.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3twrybaja.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mkasnngh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tyohlqml.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wcbyxqnz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3utjmeqay.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3cxtgilcc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ylzkqpzz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gpjjzhcf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fgzvaofz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zqecydjv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vqymlknj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ooeqzezd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jafsanaz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jvkvkhcl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cksfkqjt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ktiyoslo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zziuanyp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3liyeqapz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3babljvto.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xwbdxfoh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvbkznrj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wkmtfqov.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhwmuxqn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gmcjozsk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lcpbcssx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jlksfomx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kqtnqfwu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sfhpftfs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lxkqodav.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3jztbuqnd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3audkahrl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jgthavos.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3picsteel.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vjmfnlwj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gucuxpwg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ynlsiqiq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uxejxsjy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3inqjleta.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ldcdslwy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3tettnels.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fzzeovgy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3llfxorpi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3klclzalh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hbecnuxm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3atlqmtka.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3nwuacmoo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3evambwhr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3aazrewyk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3clbkeqpt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jjgiczhg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gfvgmrdn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bdfnnrxw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3knavmmwy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vmoexjmn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xjkviqkw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3otfkizhi.html


<!-- 参考信息 -->