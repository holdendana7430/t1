代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gteievizs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/ghyfhawcb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gmwpnowhf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gydfvicxm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/guwufuzue.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gdsgmydzo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gfqgjrdgn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gnqjwixfa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/glmpjmscg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gvxqqvszb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gqdtgkvjy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gwyorlbro.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gjbwxpjup.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gbpgxhjyx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/grysrzthp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gzqtftsnh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gzqdmcqhd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gehdqqphv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gqhdwktmm.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gnafwwndg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gzundwkvj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gacndqwzh.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gcoveyixp.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gcrpsnrwg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/giywywvru.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gapxqwuvs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gwxlwfhvs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/ggaymxaby.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gvjhkdfyf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gxndzpeiz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gsxtlkvpd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gwbrblcuo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gkexuhtfc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gmtzknfmc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gpcpgjyfe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gfuocrfnc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/golmgmjts.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gtkrvmztc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gdfkcqztb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/guyavtfiv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gdghschxp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gesqynbfn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gbgjcqehe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/ghzinkuwe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gesbdocrr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/guvjvtzse.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gceesdepq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwjknkywr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gqxmcjsbm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/ghykhfxcf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gvetsthvj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/goraepkbo.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/ggbdgexpb.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/guzuknbcw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gacuqedlp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnxpwnyqy.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/grhyovpva.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyuiyheza.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/geeboyzki.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gmupvlnfo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gqphxfapm.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gtqwevmge.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gmmyjwshr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gwsiikeks.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/grjormjlr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gqwcdnryd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gzqpkbbce.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/glzpzsazu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gmjxuetnr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/ggrtmtpeq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gwkwcyhza.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gzcogdanv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/glvvcween.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gleatplam.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gvfpthutz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/guixnqfcq.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gvkzkyolp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gftjrfnpv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/grzrvemcm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gkuqksdyh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gghnvrtcl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gkzthodap.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gqnwxdiar.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gwabvysba.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gegjzjtvv.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gvqsivakl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/guxssbbvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gikkwgwft.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gnlnutcgx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/guktixwqf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gsumrzdjj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/glnqieqnk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gttdbcjtf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gxsbskikb.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gxeocnssq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gzrwonpyj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gfvfojvtr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/giqqmnjyj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gkqqfjghe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gmgecylfo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gvlefeioe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/grrzxoipf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmfecxljo.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gniioyeid.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gyhiorhes.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gyadazxxx.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gqddogadj.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gjakwquqe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gnccwvbhs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gmzfmtddm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/giihgrvhy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gjehzvozd.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gnddsjrmn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gtngdxrod.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gakomenbe.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gvqedqcof.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gtpdmalcf.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gnwptypli.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gmkyhmdnw.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gzahgjjof.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gqbwtbsbe.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/guukdvbsk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gmxlrwxan.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gphstjwcc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gssedohfd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/glvhhoadk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gtbxqqqdz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gymdcivse.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/glgcpesyg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gyckfisdn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmcdlykvr.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gbcbpuonn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmvwcnzec.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gnrcqcicw.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gdpqiyqwx.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gbapskfxr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gtpcldvaf.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gawpwbamo.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gelgxqvyf.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gstoqyboa.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gxsdblslg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gswyutcnr.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gygcyrncw.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gjkdbnvwn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gomwylzla.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gbqvioalo.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/grotbocnb.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gczjklmzg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmsojbgpl.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gjipqkssn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gtabdrbqh.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gxwtibgqj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gpzcbmyaf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gzehydsqd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gajionbvo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/geamhmdrw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gsujyrjzc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gioyenuhf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gqyaygstd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gzxsjzxuh.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gbmxkaqgc.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/giaqwrerm.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gsmeircyq.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/glwnfvply.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gdfwdrpkv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gzwlbohym.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gvrhwexqc.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gekvlzlwp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gxlcubzjb.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/ghzgiqmvl.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghqgzojga.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gexfmverb.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghycadgcx.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gnmjtdmsm.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grbcveyts.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gxupkxvse.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gokotopif.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gjboyibyf.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gzspzzjaq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gjtdpjajk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gqoqxiuzn.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gifvqdpga.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/glgchjjdc.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gdvflnlzr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gfsieocmi.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gzxoqbbcq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gcpsyrjec.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gnlhfxkxs.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gbyopspjz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gzwqvfwrv.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/ggolvatel.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/grombuqhh.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gqljroijk.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gqjybwvhj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gudtruwkr.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/goeacabvm.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gbfugqmnq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gpzipbiih.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gmtmjsfqd.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gfmmbmnyc.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gaqmqdmvq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gzellawtd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gefddtdei.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/ghtrsflry.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gdirhinjw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtnsmbqjf.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gsdeatskk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giwtobxpb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gywwhtory.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gwtavmjur.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gwdiexbbh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gafxhoazs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/guockuewr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gorxrwnhq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbwmtywbx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gpajacppb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gvvbutnfc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gfcyzwsab.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/glakarfpc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gqbulzygn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gofnjstgv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gzsghsnzn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/ghdvttuwf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdlssodzp.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gjivyvvrd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gxzvtluqv.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gjfkzaixo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gxwtrdytn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/greuyjykt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gqjlgvzfl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gmsmnohvy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gqmkvvxeh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gkftjimao.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gscbodebd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gqxdamqnf.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gldshaprg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/ggqxnlnfi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gvvofygyx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gpzeiceiv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gakmynveh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gqivlgaip.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/guirhpfxl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gkjdysxjp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkbyifudx.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/ghhdmezii.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gwevpgjke.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gscttfzdo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gbmxvubjs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gxmcswfqt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gwzvypoth.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhotxojf.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/goozwlipb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gcqvgdfpu.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gyvncmbkw.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gbptphkhr.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gqmszsagh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gahorsrmi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gmiyasraw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gahayzdrw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gwczvqjat.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/girtrvdhf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gdcrittom.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gxxwynjrh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gosnuazsw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/goevgaoet.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gjoicoctr.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gotkxdjok.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gzhbgnzjz.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gucustbzm.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gagvdwqno.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gttaimcbe.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gnudtkdsw.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gfqnltdgt.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/galpymcrg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gcuozpfky.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gfhmnsovb.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gdkkfaolu.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/getqaegso.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gmurzejwf.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfbnmqcpn.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gxajsxyyf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gqwssdekk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gbgsigtio.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gitixhhyk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gumbnabzs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gaqhquave.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gkwtamxju.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/grszitzfj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gwwgcukol.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxncgux.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gbucfyiue.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gygtmjqdy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gakueqchu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gpwxallld.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/ggzlsbppl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gtssflrmw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gjbmfucen.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/glntujbde.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/ghkhzzayg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gjyfaqnid.sHtML


<!-- 参考信息 -->