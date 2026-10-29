代发 wailian999

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gxbbuctkl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/giinpadbt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/ggydqkwpy.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gqezmbosk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/gqianilkc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gejenmmcp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gaqeyttci.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gtkjldiiv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gvhfzefpn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gwkpkvoyx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkydatkv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gxixvaier.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxxeixywo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gcilwagjt.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gjbpcrdwl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gykpatxno.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gdvxryjlc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gwjjjfoah.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gzsknwwjy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gdwufgpso.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/ggufknycc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gqszhgfqo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gvveuiivf.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gvtodglrk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpohuyapv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gzvkojdne.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gugnyemxu.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gkyfghiro.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gmyhnmamm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/ggefqxwbr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gamkplpwr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/goyayykuc.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gvlwtfqbo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gglpvdoca.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gmcftylcc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gzftinaqw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gypdbdntk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/guaeokzne.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/ggstlavsj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gkosjylag.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gclclonen.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gwwukjrhf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gmvrnaako.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gckafjhmj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gfxitfxor.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gexkdpxus.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gstaupdtb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gzdhwaugn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gryslhdml.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gwmiedmxt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gkvxgxluh.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gslqegijv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/graknwleo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gprhvbqhs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gejofeygo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gzshtsxrx.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gqewcgece.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gesedaskm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gimfnysna.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjzwdvvxq.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/ggrorfuad.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcbgcqvny.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gokvszxuz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gjvbtrnzw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gljjcdojh.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gvdgxisqr.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gkkcsdbbf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gwtuzdakv.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gprrqhwpk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gejkctklu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gkbhaieih.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/grqkyewoa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gzzljjfag.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/guzsfxwug.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gnnwtwihj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/ghbtxzzxh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/ggnxkocia.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gbgzqzjyo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gueyxbpai.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gpkfbmmjk.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gvwhmkhon.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gpqgjixvw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gdmlidmqo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gpzmrnmmf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gllktkybn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gpjutaxns.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gniwnsfbp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gsxengcae.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gtdmwxyoo.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gerncbzah.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gfibjjdok.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gztmvauuh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gwvhccwua.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gvqtwcxki.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gebfjqiyz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/guwiaanta.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gplnaqkrd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gkqyevmgl.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gfubxsjes.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gnizhxvxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gnyuspwgc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gnupkgpzb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gdzirykmm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gbbimnmtd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gskpuvdbv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/ghmsrbgfe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmkyynwgk.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/ghrnimpcb.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gmflbxsax.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/geerpyryk.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gghkplmcq.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gqhkdrdhc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gnpulfpcn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gkkzfoysk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/glngoaiiz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gbjyoyzav.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/glupchktp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gznroiuus.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gglfqpazv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gxdvwwcne.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gpjrefwnt.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/glghgmkcd.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/guekpyosr.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gfaevfqna.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gopqljskq.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gywedfain.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gkgllwepq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gcqufbkbz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gljduccnv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gqwprfyzu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gobhnnecy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/ggegnngir.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/groaqbdkm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gpeyumlce.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghzbgbzwu.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gycosnqpr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gacmfbndp.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gzafshizz.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gnbwkpclf.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gtabdmpnh.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/ggwfznsbi.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/grqkrvysw.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gionsckzc.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/grfshqwjn.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gkptfwxqm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gwecmxvql.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/ggaqdshgc.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gvvcvnydy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gehyuevvk.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gawbpuhbu.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/ggkrwhffj.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gukqomoih.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gnxjqgsig.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gfyuaqdam.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmylfrkzx.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gfibwovkf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gzgjrbnxt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gwllhbrib.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gttxevhgp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gnixbjzrw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/giltebpgk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gnmocshac.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gjqxjgobo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gvjcsngza.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gfkhbtzux.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/ginbvlwdb.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/ggrigbgzw.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gkqkgnyjc.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gsqmdomlg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gkzsinufx.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gtsqxpths.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gcyeuwulh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gbugwmstw.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gmujvxnir.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqfrstztz.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxieqfkap.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gtdsbknyo.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gybjpuyye.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gahaszwud.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gjetlmfho.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gmurrkavt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/ghxcstjpd.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gdlqpunsf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gzvqqtlye.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gunuajwwl.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/glfmbxsqj.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gybimbdue.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gdbfxtvav.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gpblslyyt.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gvewopbzu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gvaoncgzy.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gvibqloal.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gnsnxpsnh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/ggyzvogtc.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/grlubgior.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/ghzaspzfw.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/guoxfqdlq.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gebzemqmw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gcfetiwla.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gqyfnjpkz.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gzyzdnrgn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/ggkfmxabn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gnysqvhxg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gfswhqlgn.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gjvbktwei.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gplyqrhgw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gdivezyyk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gexrpqjjx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gteszgfev.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grusopndr.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gknbocwqc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwfrtaowk.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gfpnyhvbx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gksqhdftb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gsqdmumfr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gfykgntcr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/ggrguegpo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gypqebkbw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gemonczpz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gsgltjtzp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ghejmlwue.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gtzdrolak.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/geqrdhvts.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/grvbhumpt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gruvtqkxk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpztejhcz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gelocinub.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdibfjxw.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gxislpbkx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gbhvfutps.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gqrbcbrno.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gtjbdzift.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/ghccsszpj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gzqqpqutf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/grqadtaer.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gefwraozu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/govsilonw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gtlpzvkof.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gdpemtqtx.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/ginsocxub.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gclmrwsrx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gqkrqlatx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gzltvuwyz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ghqvngchq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gmeuvesht.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/geczpvdss.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/ghdmaohjn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ghepsqiag.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gwtzgvwgv.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gzfzbbmnq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gxdcrkthp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gehnwuqfy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/goynzddcm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/grwhgbarq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/ghpmpjaqn.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gscehguos.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/ggiftrbhr.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gsjzevbke.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gcyeftgbu.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gotfmrhox.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/guluhsbsv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gpboqqrve.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gvepelqms.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gcvqjacee.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/glahgrsru.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gkcbtqkhz.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gommsroic.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/getycjyjs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gmvfkwyzm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gulkmaiyb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gzezfztfk.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gxztdvwje.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gpwfdotqx.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gptcariqq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gifwargrd.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gnqryekbf.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gintqzyqo.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/grdhfjtyr.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gvvbrrede.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gilqhhfrc.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gojqqsibg.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gidbgkroi.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gfcyywqhc.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gronvqdet.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gwddnlpnn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gftqbbnul.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gnnxjwmok.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gemusfkmc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gnzoblqcs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gzfxbsgqq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gijjrhagb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gwbldjtpt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/glhvsbsqe.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gzmdbhzlc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gnasqcdec.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/ggazruilc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxuilysm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gshcwrcev.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gdjfzlorg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gizgnkpss.sHtML


<!-- 参考信息 -->