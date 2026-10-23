代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3amcacsas.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3kbrlvxjy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xeghcvtu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qsdwuuqa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3uzlcfgch.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3tlwtujnv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3fixfkvmo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3rbrsyeio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itdawgtq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3otyynipq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwoptthv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3syglwebk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vuoilwea.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lghqykug.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mpdxfgci.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3laorcyry.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3seoeongr.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3fkgjrsoc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3tozsffnz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3uybgmcju.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3kwbidlgu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3unxczzgs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3xlrszdto.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vufpnnlo.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dlfsgaym.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sbpfrezh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hauhheow.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhrjdfbi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3tairznwk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ilwcqlok.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3apyunqgh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3tlcugzes.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3gatorexw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hxmsnnoh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3spmvqzuh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3vkltucuw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jrtpicxe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3cgiiutjq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3bbequciw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3oqnmjtog.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3mgqaqvdl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xcrnrypo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dnbflnuv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kktynsox.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zjyqfecq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qhmljwaj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pkewcvqo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3wmxpjjfn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gqnecwon.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3aeqmideq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3plabzalb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufeiaodk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3bxduovmd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3rybilqdp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rbkopomi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3xoirdpvt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3pqkthjsd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yxwqrbto.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kgglvtjd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mhjcymuz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3znbpzohn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nybsmkby.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qqlwcfzr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3imdpokhc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3stzldhtm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3mblrvjtr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hnwizspm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3zyiuhyro.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zumawrwk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hjyweaxl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sddogwgc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3jbkzljnv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3guxydxjq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3saxrnxso.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dduhxvuj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dfsmfejl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3pxrgsymo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gptqlqtk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vytpcund.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3urvgfkit.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3qcupekou.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3vdmsbocx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yikhubsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzzithng.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3pqjttcso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sloenlrj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3zklvzfhh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3yludszqo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3cmevwjxj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3adbucqab.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3edwcpfjw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qxyankep.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fcqoszah.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3pjskcvip.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3fufkaigc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fhflowdw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3obbmmwtp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3smeyreyj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nhrehwft.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hwfanwfp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3fjtsgyfi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3cefzerwz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3byqlfpsi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nnxiblwi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3hlfoeuxw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hqhpjwpx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3icydbicq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mqsjgmxo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ffcrmxds.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3kfzpgdvg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xxnmrful.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3vhenokfu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xemactfz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vjsjukni.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3psqpgmfa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tfhuubjc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uqmfresg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3htrytkds.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3geyhihyv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jscddldb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fktygypv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3focwnrmm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3yzkpkbnp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3bdmmzubn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3mxcrowvq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lfepxsbb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kaekqtqg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fcosqipq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjpgeryi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gwlypzge.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xehzzmma.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3avmuvpkl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nlheqyfq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hrlesbeg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ldxndpeg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xpbmrmzd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mtpydjdy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3fhmtnkan.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3izoamxwm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wzsywafa.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tricwswt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hdedmpzo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fbxkxpyo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wrabxkwe.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wswtevid.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3gasoaoqz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3acuurlwz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3laiwnefy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3piwugedc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jzohfmvy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3khdohptf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wnhpkxpr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wdqsuibn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gfeonrav.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3lzkclxst.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pfswtumz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nemwzyzf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rvgvctln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjdunrzz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3olztxzhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drukgwvj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rldtscrs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3uqvwvnns.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qcccotiy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qscwphzx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pdxesjcp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jrrpnfjb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tqlbpdme.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tvzsxuls.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3texqyjfc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3djvaozfn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jnvypdqe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3hvacgwum.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tzlqnjkw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hafzlmqw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cuznxalp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3putqascl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mgarmuvu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rxnhkepw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3djvwuhlo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mkmzcvwo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xziiqokp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cezhcdwm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jgzzrawj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3aswiphgf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kzagmcat.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wanrmkzj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3iujlevzz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3oqabdcdf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lkoybrzo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zjllqmap.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3clzfucgl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jhzilrab.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ykkjnmty.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xqwdvsre.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cqgwkmao.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jqlijulc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wmkzbvxt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3akgzppws.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lsqmgmfw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ykfpgnch.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3apwlskgd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiqgwblm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pqfolrbu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tpvkcalw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3syrsondk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hmhirypk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fupecosa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3quaoesgl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lpwmmljy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xqbkvkjm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qipvepah.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qkgiawtz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bktmrnrx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3sgfzgddz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3avxkzkhc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3sseoahaw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xbvlcpqy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nuzclfpj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pmjjrwmp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3aahyuxwi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3gndmujmc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wdhmqfai.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oqusynlz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3epjadcow.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3lsypeerx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fapkktzs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kefsdvcl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3szaabtjj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qjaijkbc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3buuupibq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lprazqek.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3slsfunme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqmosiij.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xbnocspt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtidcbwo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3guvapfaq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxduotji.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yllrrejc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yegscflz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tysieuza.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xqdxhxmf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmwstomd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3boewghoy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qknfzowq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xgeicmlx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vpoewvkd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3oyirltpg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lfxqexne.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gsqvkron.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3znwijkmm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xzqdspft.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xwaejrvm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3npclozdo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jcovnirq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3bxhswitm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3yijbehbe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mhkivqke.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mklpstvf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gubvrogo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zzatqwaz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qpetlfmu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lofkvlwm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3athhzwpv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyxbrhrn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wnnvdfzs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wlozzsus.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rslzvprf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfgomsnt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lzoagzam.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mbvwzrxp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zjlfrcfp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mullubkf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kdpswrxy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnobgkcs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hkvhdunj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rxjknsve.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jvdgdtgb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wlbauqtx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yjdbebdl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixasbwuw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gbsuynhz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zxhurcop.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qinbayzb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kvikjxdb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sqgfqmfp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3sctcvaui.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3qxtomzup.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pyudozob.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kvafeomx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3sjyehpng.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pgjjsvcn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rnllsrdv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3snlxthju.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3brjyyihl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ipbmhuet.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3skuqvrob.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fqkfjbsl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xxqpmpvz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3juskvivr.html


<!-- 参考信息 -->