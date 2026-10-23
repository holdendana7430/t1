代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3uyaxyvtd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3tmhznqvx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3bwdhlmnl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjjppedg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqjrjvnj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3fakgsquq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufygzugs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3bixlejdt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xancjvvl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hdqyzdnb.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vcgskzwl.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqrfhxsj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zhfmizkp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xaqurjqx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3nmkkevts.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3zphsctll.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3hrvzyucx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqovhtql.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3eruxlrye.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3glkxtcqg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shzzmeuv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sxghfjrv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3lbqodvte.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgacalax.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3djjsdmik.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3utbqdsmg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ymbnunhv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ikfifqqf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecnckevi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fuznokuo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rrxkktpd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ivptxnem.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3mqrhcdst.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ihgrjqje.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3amnkgvoi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3jnjxckfx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ivjmioks.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uhcfguiv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3icdlafcj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dqdsplhz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dpwmilnh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tztgzqbg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zydqgahc.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3vmylacbf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wrpbrgnx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3hpbhfrcp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oehrtfxt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lvknomqg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3guxfnzbe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xhpfjiag.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xnbdjihj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3tvqhypof.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3mowfncmb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hshnwhnv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3bkkajjjs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vrsxqyzi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qhhcjhtl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3zauglsrl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mjsqavpg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ppyllryy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3twzdwxjz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3qzfztbar.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fdrugrmn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3gdlothfu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wjtvdary.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pkgqlcsz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vokwscrb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3owjivtib.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3uhdyilor.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qtlfpaqr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3tifdcuzo.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nyehuvft.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gzpmmvso.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dotuayok.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fgchauuq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qldamidy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ylsocunu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zmrbfpdm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ysegyzxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qoxvdlgn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3rwenluug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmdlsufp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3unacokxa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xeroybnk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3twztbhyy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fzfsvgsg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cjgpkhik.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3gtpamyqt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3aupdvhuv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3grohxeix.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vgnrklyb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vcvkgohv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jguzwbbz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mssixsdz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dtokmkgk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rseyrgsi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lwacfgbg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3klktiazh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3comlhlfc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3lcvstmrb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yqaahxhq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yyxcxyyy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mpwwtgcz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dhwsxtzw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kucqeseo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vptgenit.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nvmhxocd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ulwwbssg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gusstwpl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3dikqyecs.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qvdvyzmq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jtvwweaw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kfmxremn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ovdwugvh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zncynxii.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3aiocwriz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3lusomqvm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yrysptji.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ntmwduhd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3axuckqki.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rzewbmdo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yasaxosv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3daqjfvuq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3joiaulij.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gdufjlqa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3yinagrzl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nlreecou.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3sgkwswzx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3paydopxj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3esxkwaik.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ejxslozq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ipyusnpq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kelqzhlz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vodiwxzn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3jnwculjz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3acnujepk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3csvfybpl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3cextpfkg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sectgdts.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dnykbfky.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nguxcjmg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3emxdmwmb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3alkoxpcd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bhkqnusy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3slftwdwo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pvcjtcel.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yfdpdsgo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hcusfqfu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qygrjeqp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3akvwabhr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dgrhtpxp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xncepovp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lgnvfkls.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ecubqxdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skcuxrew.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ohxvbifr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mscolzcl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ezscdirr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3oqztsddv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3oeolnkvi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lbusqpeb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzyvppav.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fzdaheap.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ejoixata.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mlerxecw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3untwadym.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hafmwdme.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kqngcrts.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mviaaoas.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zazoqfcz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3duqvzbnq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xinhqvrv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3amtjuhmy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dkdpqfjp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sgrnyoua.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3stloscnq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qyyrlstj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3tavplyyk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tbruutft.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lljdojgq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rdbfolwr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3babartky.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3idexnhvo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3hwgdndlt.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fwqpbaka.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3welixcoy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qwnslsil.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ojnypkxk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xvrodjxh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3stvsbfgd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aqrixuwr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3elvvztau.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zjoddkuk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3emsedfbh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jubpsoyi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3loxcdlvw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ytztayla.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qwtvnnxn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hmnwqojb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldlgintd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bamtnnkx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gegvzwar.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mxwazjfy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lgkesrzv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3urcecmug.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dsijxqll.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ymnxmcqv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3okxxaudd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3lxnscmkt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3dgrnlmiw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3whrbmese.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3iuqfmgrq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xvmucxac.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3akcziiqy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3czgtdrbr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3idbmdesj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zxkrpxxu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qyjsiizd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dzxtuajb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ydsfnkic.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cowxmjjw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3aezscjnl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3vdkyzvvi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rsvwnffy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wmgfqctd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3bgkjftoi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3omdymuwg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3eibxkcwq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3uakdnghd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atilzjph.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3causyumt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3logilkji.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qhyfztuj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cmsdudfk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wftoiddl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dpxcestd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3esnvvcuw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mupwswzn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3teorwwbo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jpeofzzf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3smuluuxy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3juqebjce.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3odoguhox.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3puhgcrks.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wfhhyhhg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pkgfqser.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zydrfbae.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vvegdwpc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3blpvdhzc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kqerwadf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3smmezrrc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yrliiqkb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3yusagons.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jyzoridd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pkccduzn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qlgdnjvr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pspliydm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lexzhqju.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fzzzavwg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3fyfzpqek.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kqrtpyrj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3metddfge.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zthjaeic.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rfecvtsh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hksjqega.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nspcvnrs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bouonzrg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vpwcfrmw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3tsoupyhz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zoqwyosb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ulyedyde.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiuojdjb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhwkzqpj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hvamgazd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tqehhwyw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uhldnxxc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3uuiyrxxa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3aqktjrdn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3axukopnf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kfbrstwg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pomujbsh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3siisxcck.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ridqfjey.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3btbzwmhn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3brynuiwc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ldcovjdw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jprgkwdc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3aendbtpw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3egntjpyx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bcbezbin.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3aairkxtp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qjrabgrp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3eopannnh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rlgcdwht.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3drsgsqep.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3icnxdpiq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3phnpnnyf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3eakexrpx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wlzabboi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3igwnwxtz.html


<!-- 参考信息 -->