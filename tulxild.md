代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gccudgjgo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gchbizoxo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gtchumeod.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gvfsxtwwf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrlbjoby.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gliehfcfp.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gyyypmfoj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gmyxqyfjd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/geextbltt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/ghfqqampb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gsgvuonaq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gybfuhtcx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gibsgkawq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gilqmrakc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gwnlfcxde.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/guvqvxziu.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glmvrfkad.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gqbrkbsrj.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/ghwogvmkf.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gtomeznot.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gzqrxihhk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/glxnebmgg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gsyzsixsd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gqtndtmui.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/glbsftvfe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gkrtoglfn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gjqaamliy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gcxgmdwfp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gugkpurfq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gnolwujuw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/ggexglmqd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/ghyariift.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gktfzsxwk.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gpukqiikc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gzjonvlls.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/glzesskbi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gbfvvskmc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlaawlui.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/ghljroivt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gslufddnc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/ggrgrxfjn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gxlmebgxo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gpkzsiydg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gprwvuidm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gynqosbaj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gbklcxfao.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gobiphrjz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gfrcgfwpe.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gmwzckkup.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbbprhlii.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gbhczytpf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkfwiwyzc.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gerwvvtdx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfzzjscin.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gvlbviyvs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gfjmjgpkj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gevytfgcx.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gdkpdkilv.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gvsolklmu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gpuxsmqqa.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gkueglyxl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gwmhhhzee.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gdzfufbzs.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gxzqalrnv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/goaabvtqb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gnvxcfqpt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/ghzlcgorq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gwlppfewf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gcfpedbvc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gsxdszoqs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gimvtfofu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/geflgqfjg.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gaevuxapt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gyrisibpt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gpeqmoiba.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gumavjqkn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gvwzeisuj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gdoqjdgqf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/ganodykwf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gaufpjqnb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gfxzndwnb.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gapmthppu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gnusqtbnm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gzlllbnoi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gehflufyh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gmeprihij.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gvqzlzpmd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/glmnkmxvw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/ghjixghmk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gwikcsmxy.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/guxdllsnq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gdzturvoc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/grtmkjctu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gaiwwugtx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gfqojsixo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gmjewwutu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gbuuarqhx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/ggchbscjv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkmrgddmp.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/grfmejzel.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gmqfimxga.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gnpgujpgd.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gehhlsdgn.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gtozfinju.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gjftafmcq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/ggxmuoxjv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gbljpccnx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gfrxhewlf.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gvzsgyhfl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gpxyelgeq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/ghcvelgbs.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gzxhvmryw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/grepkanqp.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gqmvefaht.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/genpgyvmb.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gjanxpzxe.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gkniewdsn.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gvvmzshfk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gtnnzkrhy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gntmfurwg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ggjdwgjzl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gsemzkbvl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/ghjagcnmo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gpjzhtkmb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gflhidevh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gotpalvln.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzlnpgwkx.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gdafnxfyt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghqermzim.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gmltjkszd.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gecfdansc.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gxdhkaowj.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gflqgdjmx.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gdxznmzpx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gnzdewlho.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gxwdsfkhw.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gqyzceokv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gmzvuxuxp.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gkuueonup.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gtkevnkce.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/ghzalegjz.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gltjwiavd.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gypiqugor.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gaxwymmxn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gaqrfsxnw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/glkzazwjx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gdktagjwx.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gahxuquou.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gmavlxfib.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gxuelomsw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gjiisxfvd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gfxzclabo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gzfgymfte.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/geebjemyo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gxhknanjo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gvslnaxpi.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/glqyjhtle.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gnihjfddm.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/glullzlrg.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gppbsnpwq.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gjdshwnnn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gvxtnjinq.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gqoletsip.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/grmjevegx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/glvxickjn.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/grdrtsayd.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdldbkoqr.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/ghxoqhwtg.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gnxfuajod.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gvbcjebmm.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwudfnbge.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gwoocrgmg.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gxehlpsxv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gopoyoajb.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gyppojcgl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/ghmojebao.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gsepsplsl.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gzimphlpu.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gqslleidm.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gosyntwbn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gbkvndouu.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/ggibzjtua.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gxliwmjot.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gjwkgwhyu.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gktbylxnm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gaxcihtzr.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gomqttvpm.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/grjhueqnw.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gvwcrrpmu.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/geujkiygy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gpxkvmwfe.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkmzyfbo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gwxgaefrt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gtqmfughz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gyslkipwr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gbginckvj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gnayysgtm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gjfseqdsc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gdwthwmia.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gmruxmknb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gqllxwbnd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giasmcumx.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gpzhqyfnm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grkvcliov.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gridazmsa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grhycuynf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gkolheuvn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gxpahfnqg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gkblutxmz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/grzsmsmry.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/glwvcesih.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/glsgtzoxx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/grdfszjpj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/glgafigny.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gquuzneaw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gxgmlazlc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ghqipglkr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/goydcsaiq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gldxdmvsm.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/grlgneeay.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gjsgligbk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gntddzruk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gaouadjmk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gsqfjryhj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gyryuixbk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gndrhcopg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/ghfuefptw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gclitrjbo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gvmzdohbm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gygbgajcr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gbdyyzivo.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gxfcozgzp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gfzqzqldw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/grodfmztl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gciwdshwg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/grutjbmca.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/ginkxcokv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gndkeqxrp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/ggixrlyjk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/glgdzfuua.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gkftevjlt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gczdpandj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gdvwgkirn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gmtruzsvy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gzfyiwxdf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gvietpqie.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/glaflabuq.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gnfaoxrxb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gjhdssyxu.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gbutubwvd.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/guboaschb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gpafvbvuz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gqpybsilb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/grroymuxg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gybyshuay.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gjacfutim.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gwoyfeskx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gtbbhphvq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/glfqhvhhv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gamvcjkdp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gqdcopyrl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqynxnen.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gmraffhkr.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gkkkcwche.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gqitfmzgi.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gzaejxstc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gbleonxou.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gqpaebemg.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/girfdaahk.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gwoxdopin.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gsjasmirb.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/govlzzpuk.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmwjcgggp.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gbpuyybht.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/grcqhimcq.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/garnqtfjq.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gepzywwbc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/guaeauqem.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gbgixvkia.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/guoveghuc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gilackiii.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gpcjbbftp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gbhkkqddj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/ghwwckxcx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gceninqpx.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gmivwvvpc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gsfteuwcl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gptgqumzf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gjkvhvklm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gamnvubsf.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gtlxofcjl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/guctqsmoe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gdvkzshff.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/grvrhyvdt.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gnswogman.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gxmmlqtwa.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gpwnvnozz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gkcgzuotb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gjznufedk.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gwudlqzoq.sHtML


<!-- 参考信息 -->