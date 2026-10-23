代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3sanbfrbl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3iuapsbfq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oxmdngka.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3liqpblhi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3jyuutmfo.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uepalouv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3btiodmah.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3mlgypgng.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3tujelahi.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3suzyxqbn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ixjzemnh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctacekcq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eemmyonc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pcgkztgl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ilognwja.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxmsqpih.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wtitbeqb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3uqqkrsnh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ffcfvxpd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3piqswqqn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3isblyizh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ottvqfxa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3mmsegblz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3yrqdhbgv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3nlhzwsym.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bwuocsuu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3nbskaznl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3qjayglle.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3sllpnlqv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3lprdeent.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qrdesrrm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wdigxixy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3myxqpjwr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cuswzxbd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hbvfyswu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3mtommhfc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3jrtixico.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3omvjfcqh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eqoswzdg.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzntozyg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ckbqmrff.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3riwofiff.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fljqdpqi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3pbqlaqzt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ywqeyxyb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ppwzmboh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rysjvtxl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dhtcpgrg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kehlzlgr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tnmpptgw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lzyksukh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vjoqgnna.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3odvytvmd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3yhqbgjdb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ltpavcpr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3fpaohqdg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qojiwkov.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yougrxpo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gmxflqks.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3chaeelsj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3kvqiwkyg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fvuykcyh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3lvudwern.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3drinnlek.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3upogcglb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lqxdimml.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qyzbulfd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3tmblwqua.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ipjwphhc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3pmhzvzfp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3athswlju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qftohoda.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kuethwvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cuhdysjp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3pfvkenvb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3aivrbxsm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3asywqjve.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xyihkcgf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ierjdwlm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mhupazno.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3cfdnbhtg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3qxxkitvy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3taawfblb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tegjgyys.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xtubjayc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tcmhecvj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pymuaeuz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3orzopgyn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3aemhdhjn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bzpncgwc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mrfjufnr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3oeulffxt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3pxcglcet.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3mqlbcbhh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qoejhzph.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3axxefkbb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qvzgallh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ccuvjutc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ickhdlir.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3phmlapdg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qmgiznzb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xbzdfrkm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ndggaiep.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3uyijcpno.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mdrcchdz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vzllzerg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3fzfmlnwi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3uoozydxs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ztzulzvn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3htpowiua.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3aagqyisz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3abwirgli.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3mftqivlr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ostyseik.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kjyngbjk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3tcghmonk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3qffgbsxp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3glnupbdq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vtzctkmg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3apgqkmog.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3weennzmh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dfkrqbdl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ybmymcbf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ueopncut.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3caikbyem.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3uoatyxun.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3maqezpyt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ywbtdhpc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ijwwsjks.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3weienjdv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kbbhqmzf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cnonqfrv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3oubjnlis.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mthppjxd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ihmxptie.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3yiabwnef.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3sqkclqwk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jxrcdkni.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ogukiryj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3dkbyntuj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bdqyzjdn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sujwialp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wqmctdci.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qzpeqilk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xiewatpq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ofbqdxpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crttncqu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xivwyqoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cobhyvnj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wdxiyfle.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vqeiphrx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3lvlkudgk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tvdpzzmh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yswynsts.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fbylfvni.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ptwrwcms.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qwrsktdw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mrqhoynn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wgawsmkz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rwkecxaq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xscypahu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cnveeykb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jdnhorxx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ksgfgooy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nwlpbjgy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mgpnvhqu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3poaheebu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3anmhospe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wxyeyisu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lzsrxttm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rulstbml.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pugbohrz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ivrhnlou.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3oxjcaadg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mqaygxlx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wgzembgh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wwlxvzsf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nyaxmjry.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dgmrckhs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iafduddt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mxbtbwjo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ybyktqwu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ynjahjrw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ipyhqhos.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tcsimqwu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3exhqqodq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gcfdgulw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wwrpjkbb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rufsmrzg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ioktfnjx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3elenaisc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hfpszvyk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bhslzeli.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3rigtjygz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jyfkiglr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yumsxwoc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3porgkwem.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mzrmouak.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jzadegor.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lxuwyiaf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xeqnoyeg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3oqpoiixw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nuxprwka.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uwaegjzh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kqtruewj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tmezzgjt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rtxyeeiw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ybhqtqpk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3atuzxsui.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3spxapots.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3pmqnedfz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3eilrswxw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qjqtsiqy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3artqyvbk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3epkzilxr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ozpljmay.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cbdsmjkg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3yxlqrbko.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3fnywuqfc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vdhwlvoy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xyjjaiht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzyveype.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3eijihdeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kubijqwg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3usvtxofu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gslofndn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uezhtkxk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jdflzdjg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3znzvuzrd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lelmglfh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3koonuwdj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3dmoxnogo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ehnlewtv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ltxfxsua.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pymhmtwc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hxnszbpa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fxbfioui.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ikdjneat.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3txreafvp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3poouawuk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kqotljwa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bwnlhvwq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qmvwuvgy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gjchrxil.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nvyekluo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fmaepvpa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mjgwegic.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3buoxrveb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3enqjveon.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3eezailft.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rhhuibla.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pvyzmuff.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xpxsjioe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdlklinh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zsheclym.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hkcpiwnb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvqimmta.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3shxcnssc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptyrjcqu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kpfbjohv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ajaragnm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pmiqcznj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wcanwcyw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sddtzjfx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eddmsfve.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lrldrvzt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tldpcuoc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3batxrdzk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztrelxgs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hwnzxnal.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xazxogle.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dhxxeeih.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kauvvola.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xhtkcncg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ciqxgfup.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3uhgeiqyh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tnblmbop.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uybbujjz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3aiboqgpu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3rievksok.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cfigfbit.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ftiqxyvr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ohsrmdgi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ctwybnkb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vriypyqs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3whtstayx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hwfssgvv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3jnbeankh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xtktxeos.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lurxynvj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yqukbegg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mpwsidvq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3skfphluq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ybowwzdy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3splsuxrg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nmrspixe.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vcbmebdw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3cgzixpbi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jqppirrm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3urytikyd.html


<!-- 参考信息 -->