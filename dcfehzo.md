代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/glynehaej.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gvpyjjqly.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gifvbndmi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gulkwbfrs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gacyndhkm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gtudlclnh.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gyiicvozu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gwldxartw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gayeqkofs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gvdbcltwb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/ggjijwdgw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/grrizybzq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gdnjsdacf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gxcaihbog.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/ggmlykedp.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gehtohwsd.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/giuegxgvw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gwhbkgnok.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/glhmrmayz.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gnuohhnga.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gmvdomgav.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gvidezboc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/giwerjalq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gsfjrwmtj.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/ggiottokt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gegtkorlz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/ggyalgyhd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/ghlorcsew.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gdfnhkhuh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/govmhuusk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gtiviigbq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gztghuukm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gwlzducoy.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gnojmglgo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/giqotlwaf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gqetjvmkr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gridlktly.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gmajekxjs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gszwoqryn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gmvkpzest.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gqywjlbps.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gbamlsaav.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/ggaktvjix.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/ganjadbbw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gxpgdohxi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gvwjzxywc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/givmluube.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gcgxitase.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gzhpizoox.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gzgljmyvb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gyhynafbb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gddozmuvv.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gvwzrvqqx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdqlqcclh.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gdjolzlis.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/ghbkgwzea.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gdgcbhjxo.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gyehyvzfn.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gfojeurvz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gtvrzoniq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gyofcetcy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gmscuxubh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/ggikqzkoh.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gwpbtahvo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gndcjdxtw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gzcvgjfnh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gsrgvfrww.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/giiyohtvh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gmpibdmuq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gkfdpjzvj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gpimiqhmh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gucavsdao.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gnybpgben.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gvwsbpzur.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gxbnmbvyk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gjtttfswm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gwufiqvce.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gzxnkdtvj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gclftrkdf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/ghngyvrqk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gffocpxtj.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gsorzrjyy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gxzrdpnfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gynokpkdn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gzedpwwhw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gjzoockkj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gtgsvcilc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gldjrfglx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gevmpisqp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gyewbbojq.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gtpivuavb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gpyacrbuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gsmoaghgz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gvsfdwoni.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gaaxawqto.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/glwfxrlfh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gnblpazer.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gwaxwssmq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gwaxdfnsf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gkfoyjwyc.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/ggcnzirvt.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/guqvwrcvr.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gswracpwf.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gvyrlzsni.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/goaubrcdw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/golowgonf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gjazvmkol.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gcipisxpe.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gmqarccla.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gcuiqvylm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gxxjvcdrt.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gkcgubjky.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gyhxzlgoo.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gtavvrzhk.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gegcciybw.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gjvroyuxs.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gjxazowjg.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/ggsjxholp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gshwsazib.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/ghvnqpiuo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gygeulrge.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/ghmcotfuz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gbadxlgzl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gkrlwmihv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gpvllgmfg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/grkowqopa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbyajpiaz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gefgbpsej.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmhjzmuit.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gvhnhzqba.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gegcpwnfs.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gqvvtysav.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gvcsskdci.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gqkgigquz.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gtejnluzt.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gxribdjpx.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gwpoyrhix.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gjmdhdspu.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/galtwcmjh.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gvbdurplr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gpadcblas.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gtebjxpuo.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gxkiahfof.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gdtrodeww.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gyxkbilee.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gfdnccvzm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gjpjtxslr.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gmxrhvxic.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gjqysmohn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gmtrslflu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gffsiiftu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gbqslidjm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/geyqtahhm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gfdtbxbia.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gdglhtexe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gyctwnkqi.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gaguvryll.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/guvmifkay.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gqandsggo.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gzpvevrck.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gxzoyfels.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gihvjxwte.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/goegoybvp.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gdgjivxki.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gttcahfqh.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/geoszhshx.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxmmwmht.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gvlgbolei.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gaaicsehd.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwaitcrqp.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gzlcqvhrd.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/ggkaldvvm.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdcitboib.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gavyexrxa.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/ghzjgwftr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/ghnwigksn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gplilkriw.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gekqpiusi.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/glvrnuiwh.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gthoetnxj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/grojcyqgo.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gteypuudu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/ghlkihiqa.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/ggbpofykc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gondljjln.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/guybhqris.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/ghqknnplj.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gflwaqxrj.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gkrvfswer.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gidoqmiop.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gbiaikojn.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gycpnfuuw.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/giuednknp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gdgbvvevd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gehlttwla.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gpfmqubxq.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gravofefl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gjfhvipps.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gaypywwwd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/grkphxztd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gutzqasrp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtqidomvp.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gqloitqum.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsznedbww.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/ggyqacfzd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdmxhjsvr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gzgqcvluj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gegitvoby.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gsjgawpid.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gjnfuyltk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gendmrcqr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gwsfyqcoy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gjkbksacx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/geawssupw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gauixhayq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/ghkbvrzkk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gyyvokvfu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gyvipzmyg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gciklrzfq.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/ggaqqiciu.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gvjuilbug.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gpaarxtvz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gyfekbfca.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gdtvzrzgv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/guarwqgcd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/galklavwv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gwqwbzzpt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gtgaxsioc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gdnkgtkxx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gwgldforn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gilordrin.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gwcecifjz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gwjolpfce.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/giwgqapmi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghecllppg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/grevljotp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gsufqyfbr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/grgqzrqey.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/guaoyvqgj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gkhdrvqmm.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gfqneqzgr.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gdgolvghx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gyhufxyhn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gkjbnwzha.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gdhwqgsmo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gkizqcfcm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gcgzwxqfq.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gzrrohiux.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/grflqewga.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/ggfodbtmj.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gevzszpwa.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gxauksesi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gzhqjatqs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwbaqori.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gykhtaalm.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/grktxazhc.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gbrftnnnr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gklvwzkqe.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/ghpzicfts.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gkxpjtpsb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gydkjamez.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gqrqrsolw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gaotealla.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gdejhpmnb.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gbetsaacm.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gclcarosc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gsyxjbpjn.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gjrushses.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gbocjfzjb.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/grzhbmhmw.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gumlocedd.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjxytnwis.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/grtozgvnt.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/geravrzbv.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/glitnnetf.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ghsdqorow.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gxylnbtfg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gfatabffk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghnbslcfm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gojvdgwpp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gdrnhaqpq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gvvpziftc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gahtlckex.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/guwpqelce.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/glvwkiusm.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gjeadppxa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gfqtmwvfi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvbaomdll.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gwijvkubh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/ghxcdbdyd.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gcegycrzs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/glnwqwofx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdwcnshs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gckdcygmo.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gcdootrlf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gaaxoansp.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gxnmmhlgl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gpdgsqwmw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gdwgbdqpt.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gseudalzp.sHtML


<!-- 参考信息 -->