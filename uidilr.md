代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgciifxe.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3uqtrcucr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbqxohtu.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3vjlbucol.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pncpxygi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3djvpclpl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ixesuwtf.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jbvqyzns.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3gnbqwukg.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iobumnwq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3wlnztevs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3biqmksio.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ekhiuneq.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pinrgppi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3eskhwkau.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3taerlnpc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzxkmikd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dlmhdlke.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3iawmzxfh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3odgnnabl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whjmakpp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3nrduheve.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3svxpsmtg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kdjmxbpl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ujedtjoy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqprftby.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3zkmdnwnc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3hhantjzd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3didohhbf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3fxuegzah.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3tijfurac.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3injcifxw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3vxgnchlz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xmbvfqlp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3snoldmpl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ncsdldmp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3uirsnxea.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3bnivedon.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gkmupolh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3nkdxtffa.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3laasarxv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3znxywoly.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3efkvepph.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lqkgdpxq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3rgmafdoj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3vluzrjcl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3exyvnhrv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ryhnbftf.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3anunrrhq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qxbkeich.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ubwpiwos.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ryfympnm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pwhbphco.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3meztguym.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3snhlwfqx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3izvcaish.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dnnwukwp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3gstcsxxu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wppfxogo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3djhlgocs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3phsdkxgt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tjmedece.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3unmeqdjd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vahnythv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sufceszb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3brjdfhzt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3eihkmtin.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3imoexceu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qhumeqkg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3anyyrppv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mfwrnshf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wddxxvpe.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3tmgviglf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3roztnche.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nzzknhvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywfvgtqw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mhxcvhlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evqpqxei.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hzabxvbl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hmwcjonk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3opxnfihc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3flzoslld.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cpcolxzc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3exddrdej.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3udnznccn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3nsyxdybq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3qnxdyoam.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pyelaysf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pthgjtui.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mltoqvsl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uoacnikx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ouicmvdw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3opsgisuy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3hbxkuskc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jmgrzvqf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wrmzegyw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hnapwodg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vnmilzlc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gvhametx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pqmmjfgb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3sosrucnu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3kmvdislu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yupwypjq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xzpkwtkw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xavxdbow.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gtppjzsj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3buaetqpo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3pwgmamrn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pgkogyds.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ssrrhgrx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3nzmnvdwn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tanidphz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3cebbmhss.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gylktnyg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3slylmctl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3nhygqbmu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vjykynnw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3atbjlzsq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ebveejeh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3pesvayob.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3moqfuytg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3njpdidzm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xnibbsiz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qmfxrxrp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rrattkxe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3skmjerjq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3drkhwtco.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zndibmsu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rzfzusrw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3msavrmwi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3usahkfkb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tlqcfwmi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uxwejsrd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mxlvhvbe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3phszwqwf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3omqkwelz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qihpkrqq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mvcdhpqr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3otzkzuga.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jpknijof.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3edukozxy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3sixywvwv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pgusuihp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dhllxqrk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rhnxmplh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jiyrdnoi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3pnlwrhkv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qbfvzfta.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mhtwhkvx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mladdrgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzvebuyd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ekjytpoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syxnadod.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3acwtievp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hsrarnzu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qcfixcbe.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vpnxpcxs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uzuxammh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wqbpwfpq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dqzwfuge.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3mfaswrjf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vgzefqhg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jfayjrsq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3addmptnj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3amspqnll.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rqctobgh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3juhkuech.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qfrynwia.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lxdhuidn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3trihhbyy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mjuqsuoq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3mrefhyah.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gjrekioy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3kkpamisz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cuahduyv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hrnpluaf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hbuzrsun.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3eqvzokbh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cggzjwrj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tbsjkqdw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vlbwvukc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vaztgxjs.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ravsnamh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fvvhoxpv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rsvnaneg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xlhueypg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hknmlprj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gmkiubxm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kvyadmsi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wzuaagzx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjaxnkyf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3whkvqgvq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvkkwfon.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3apsdhwlg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jxhlzdvi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3guleycgw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3koxrrdze.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xpvpjdca.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qtbqwrno.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3aiobdhfe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bxrpckhe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oqbdobkm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3crwbmhdz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ykcpfqwh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zljwveyd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vmasgqqs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gwcwvblq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wrqjmydp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xtcsvbej.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3bqtzmjls.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kftlrinr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fjgpqhtp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mofpcvhv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nhwgoymf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3sbaaghyj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uczunosb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lymgwlma.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3nylmiyme.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3twlpuolb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3isuiolwg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zbhskqxs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3adfpsmfw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vpavprpc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mzxkyaqe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3effibdkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkefiflc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3oqyoycbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hijfhdbx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jifedfll.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmenljoi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zqtylnyd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tuwmvriw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3expplgom.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nhgmcasp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3clcuorkw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3yptbvghp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ydjqgqpi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3psucygmw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pyajhqmw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rplffqiv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mhqvhfzh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xgpcmtxl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3yqfwkntd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qenmcigr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tsprcypa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3utxoxvqi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3kjlqeqhs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xouxfuzy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3efhukgac.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rsskstqc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sbbtjrob.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ermjtpge.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jztzihvu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bncvautu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3egaqjyjr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ohetmpjr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bbfkxkrv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwqncbjy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3keoeptxb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wyhxruue.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3clnysiwt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mwjwzzom.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkclkqbe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qcomcvfb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ejuwvgzi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wyylrbqa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfusrddc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zercvjkf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xamtkmyi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fhiaccnw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vtlfqbkr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cjrlnilq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rykmmbab.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tkjhwfrf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rnkegsam.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sztdfrvj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iuejantj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oawsumgv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3rjqaowtr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vvugoybj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vfjrfruf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mkeasqko.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3fhbjwxat.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3tkwdfrvv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tzukpzvs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rljzxpwo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ivalfhes.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3yvurghbq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3usyeqrpb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vsebjoul.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3imckbwvc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3hzsgxung.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jzwtoxik.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3nzwtxoun.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nhwzoppc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cfdwogxb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kzdtyyyk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pegftcnm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cjwxxbzv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pyjrdgse.html


<!-- 参考信息 -->