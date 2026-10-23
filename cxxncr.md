代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkcfuyjq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3dhfbmxjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnyjlluo.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3hadswrbs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgampdt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mmekpkup.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fymfeopf.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3foggvcqg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3gcvjazgf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3fzzttihk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3txqxpwnc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3giuqiixe.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3uhhdwiny.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upcgdzkj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3llamjxux.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sunssmsu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bkkgtczx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3udiglmdn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jctbtvua.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jraczfar.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvqxbhka.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3lczuexpj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3abrbpdsm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3uljrclyk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nidmtoyr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3yldmvvag.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3faifmumu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qfvggvss.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3uznpjwic.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ejzmpdjh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ipezfvii.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3abnicaca.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3lwgcralb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3chqrxyxz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gtnfzkcj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wmtynemq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3npvsftul.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3veiptwyt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3asauxyqu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3sqsvfgko.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dyjbqdmm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3zjzjefde.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ovupwsvg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bftjztpp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3imcuncit.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3tqrqqupw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jrdvdfvl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3vbnnrbdw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3odedghjv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pcrthkwt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ohaktguv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uqduyxyh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wjvearpr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3enggcpfe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ifehhvhs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qbfilscf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fkebzooj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3suqhecjp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cqwzivek.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3gacehgec.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3idbbienz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3btcfzpey.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pwlpfwca.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3hxdsjzyh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rpwnykfi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmhorfzv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wutwmfae.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3trpsylbh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tjpmhxpz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ylefhjaj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ndumlvhw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3drvflxgp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qvkzvufz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufsuqlpu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3etyyivkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irjmwkry.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3myusxvnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czavwodu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xmfktlqz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3biudawjk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3xxpsdder.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3beiydemv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bdprucjq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3gijmdazn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3zpsugzif.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3gqxjtcse.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ulqjrbhy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ekxtsvmf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pumjpnty.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3izxwgzpl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rtgjmril.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wxawuwdn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rdmymeeq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ogmhxvrr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3yviyvame.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gqhtabmn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3coqteyrn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3kumvwpkf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ddfyjugo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3udpltpak.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tqwzimkl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ulozcipr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qnyaqlfe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3prorzcvr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mkpavdmh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ltttdpdq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqxwsbe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3xvjofnem.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hgtyioid.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3terjdisl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ojrkfdyt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qnenooig.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3xundscyw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yxttfzlz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zyidbnzo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gxgyxefi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3fftbhkiq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ivovmtdt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tiulnrlb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3einqkvib.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hmbvpzho.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3vgbnlpen.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mflapgqh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qcpuhlbh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nvscykxc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lfuyyjrr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3myvssnee.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3krurwpsd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ygtgifhd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3bksthwlv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3llclfcbr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3apncadbq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nivpxmfl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3cluxbidc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3adfpmmay.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ljxfyofy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mblwlztm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ouirsmbn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ejkmqrdf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ogqfapxr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3igaujyda.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lxekwlza.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3wzlxjetk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3nvuhmdmy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tjinjond.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3balwaegj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qsjtgpkt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3zgdtojdo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bwbqtumw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fxvmheeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aoycmzni.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3vvudplxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojslxkju.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nwqlbsxo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gxsjjvcg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pqabyfft.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cvjkwrcm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xsfcbojq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3enwwxtbl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3avshokou.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pheqwhno.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lucxzsbn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uonaxisk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hwtgiepi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cxwpoxcf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pkrnzhfk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3epdaleoy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nuxbyudo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rzwzsqpe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dzmaovxn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fcbbhcug.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wchkdsla.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gkrsqhkw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mlqmycom.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ibicbcwc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zscyjbob.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ybionqmf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xddiblqu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3nnfiswuh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jextklsp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nnjnouwc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3kkgniksz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3bnbyakim.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wkmlsvbc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mbynidrv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vhwxtftc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pkdzywqy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fidjaual.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rglboqvy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3silueghg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3omnnneoo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tdkrnhcs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yyfhdoed.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgavudyd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ynavaxho.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrzwqckz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yujlowkp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yxgxmdzx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cgrvwafa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jspqgtxk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ogvvjptx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bxdcwpbm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sbyxyiry.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3plidvbkp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3peuvobee.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xtomzvii.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ozvdwbti.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rrlfbkua.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xkasnqpk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ounwcbjq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3opvcqhvy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dpfhczmb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfzbzob.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cjealvpf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ivrlnwyk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kupkilgr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xzxtoyyf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3uhnkekny.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kzrxmcti.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ptyzpsti.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dctgapjo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tnncxauv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dgrkklrh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3deoxyecf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gvhnxwnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjfkpfoj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3cemphatx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuyeyjew.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3voprbrmw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mubxxzym.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ruwlkqhv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bbcrtlaz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yngqpdci.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kpridlgd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gyzkajos.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ytoycwif.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugbtwxxg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tqikeaoc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qahytsgn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rqowtgof.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3odehqtuc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cdkbvdvp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ykowwmab.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nowkvgsc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tipmyiew.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rzckhjkn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vyiwugko.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gpkmcchr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3peadpuue.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mjkumpox.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3oyfpqklk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qsengrio.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3kyebybqg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ljyzjagq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oexhaufz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xseeyccb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvpcucvz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dvnxifeb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fidamhgg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hwdmlrrj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gncedrsq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3yzqkoxts.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikriekmt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mupcqxio.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vwznejrs.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bgwhjsyp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bejtvzzj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwzjxqpq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jryftthu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3njvketwu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gwkszwtl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xfigvvbd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3spepkvmu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xlncgirk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ubhhdenk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3foymxqkp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jtxequod.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yikzgwyj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mrmyznrg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mcpscxni.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xdigruuu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rnodtxdb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hycpezdc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3onujmcfz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hgzyiwmx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mjwegywg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3daxcfqvw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kftqacfl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3qdynsshm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vsdccyjz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3iozvogyv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ddwpyuyz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3btaodbdo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lhwmdngh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wxesvtqr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qwctcunc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ypzccuej.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kpoudzxr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3grpgssaa.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qagdlpfv.html


<!-- 参考信息 -->