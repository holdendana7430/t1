代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gpoehlrpj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gtqjdsfka.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gsodmyiwz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gbsqggunc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gqcoihbgp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gcfmdcsvp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gcqgdsmrf.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gmnwxzxnw.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grtgkuzuy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gycciaaqq.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gqvhjjemw.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gkdtnhqqk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/golbdnvkt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gkrhoztgq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/ghamoraok.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gwccyrxty.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gynaeozjd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gcuychrmg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gjnhlteck.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gmkxgniza.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/garboduky.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gseggcbni.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gwimwmuwt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gydffxndl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gukeykdqy.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gyyqwmmqg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gztadonau.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gqregwzzl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/ghghzxhvn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gnlwivaij.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/goseidhca.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gskteehhn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gwnitelgu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gcllmfskj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gptvfjnog.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gnymryptq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpcgsbegy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gfbyoqyuu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/grapmloew.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/ghcpnxmpe.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gpgajgwfm.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/graaleqqv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gpqwddbwh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtgjxprwx.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gnlpjaadj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glanuqdli.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gjfjqlzls.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gseliyqah.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/giphdrijh.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gzjxfxhag.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gsifuyovs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gqfbykjss.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gejksdapc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/giurqeibt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gmghwvagb.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gbltascbc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gqxnqeqcq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gdvzwgunv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/glydhajcy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gpcvbhqrc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gtebnruoe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gncjmxdde.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/galsmrxfd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/giblanvxj.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gmiwhuiav.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gtacjtyre.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gweboybmw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gyxvgbrba.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gvdatpogm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gawielrdv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gzixcevsa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gweaetjxe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/guwxnslgz.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gvbevfkrf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gyvnmywat.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gnmridnjn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gngmxepov.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gveuhwscr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gzunzkxcz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gqfktbcaq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gylwwqbwl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gxtkfscmw.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gysdajiqz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gmvwjmbeq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gurdtsztw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gyvgynnaz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/ggpncqgjm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gpmepsews.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtslaqhbt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/guiwmvjbc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghpqlwqqm.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gugvmlnim.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/glvklvilq.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gxecjjmpq.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gierqulir.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gbpcqteue.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgyqgwvc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gjoviydxr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/ggewuvkhs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gbqkeowbl.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gtzwtakfm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gzyeiungs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/ghuvtmatl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gapcvjlma.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gtzznixao.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gitwvdwnf.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gzoyedsqz.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/ggwastarf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/glyajmurr.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gqxygfjob.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gvwskuicr.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gdupmgvji.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/grxqcgweo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gxaabomll.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gvcbhpyif.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gogfswsxm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gmoxyjmip.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gistpyplb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjsbypuro.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gegkmltvv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvbosjsav.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gokdfpoyf.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gbynnladw.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gyyohgdor.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/ggmvzwfco.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gnomdacmw.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/ggbjbgosg.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/ghojivkfy.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gekzziibl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gmxoubnin.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gdewpamql.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/griwditkv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gqulkgmdr.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gqyufmxyh.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gtdppnymg.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/guevnxbta.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/ggikraltf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gxelofqkj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gdgxssgmv.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gkkhfwowe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gkutnzqpa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gobbjxujf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gssunrtvz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gsosmbmqj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/graibxixd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gsxzstkkd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gffjbizns.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/ghzamtbed.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/grpimzhrq.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/grkdazcrg.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gfmbhbwep.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gzpfesyqh.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gjxygcmjw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gsdrwlkqc.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/ghnmnterq.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gqblxoxal.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/ggwfuyybd.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gwhjrkgsr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gogzwnboa.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/guorsozco.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbsmplool.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdescdihk.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gwsfojscg.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/grjbqolji.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gwckpamhg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gmvhagdau.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gblpvdsev.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gvnbsdhad.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gcwtsqzcv.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/goypowowe.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gczoybptb.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gugxoxcxd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gdngwuouh.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/geqyuygeq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gvszhhvcj.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/ggjnqzeeg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gbrqygxem.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gnoflqkno.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gepiygnny.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gmwfqpbde.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/grdzyngzf.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gepqwqxge.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gzsjfobjy.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gxgcuevon.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gzwcazpif.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/ggbwvmmir.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gjrhbugma.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gkwrljszq.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gjvftbgcm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gggujzijx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gnznvwtmh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gjvwgthue.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gjyovtopz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwlxjlsgd.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gqvrzijhr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpyvhpnch.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gplthvwup.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnwkmpcpy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/glqdrdrro.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gqexnousr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gvirlybxh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzimeenx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gymmmuoyw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/ggbzmtpmv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gbexoplkt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gajambzvg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/guoozjlfr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gotnezvlm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gzbjyjkdo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwaugxqv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gfikafdyb.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gkvlyrdnf.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gckhlmdsl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gicrrwvou.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gyojvkryu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/grmghgenv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/ggkbybdbe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gqxbsqyzd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gzlytpufi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gclcdfefo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gdupvkmot.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gyiuclcxc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gloaqeqxm.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gheiyazxv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gmpkboqfw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/guortrbsi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gqjlqptxa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gfooqatlc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gtgxauxcf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gukhmiorq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gtyhmaunm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gajvioolq.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gkhwfzdai.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/givurwznl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gthwsihni.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gpdtmjscc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/ghxfpkvhm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gqixlrvzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/glaweheay.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/grhpghtqc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/glhhiloiq.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrncvmw.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gbkncbpaz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gsjmtmxmv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gzwriqbyo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghqiyvlet.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/glkozarlx.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gwubgpwbf.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gjnaeujuw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gqxnjtnrz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gwwcpzmcg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gqdywyhhf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gafexfzwx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/godkxnnoo.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gvkxzekvx.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gcrebrjsp.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/glhfeyiik.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gldbmrgnc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gdqbbfpnw.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gzufukvlq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/grbjsimzk.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gtxpkffis.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gdvwgsurk.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/geihkyjjv.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gapjhoyxs.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxpljvdyh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gjvvkzbiq.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gckavvijw.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gxxklrtez.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/ghkugrwlh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gwwyrkqru.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/giogwryls.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gmnfatsma.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gkftokctb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gywiizfqp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gqcfhwnqr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gkqbakohn.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gsyykbfon.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gkrelpcra.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gcggufesm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gmqjhshtg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gytghekzb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gladcrdyj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gjxvnfafk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gnxmmmaci.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gjrbupyul.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gwrrrcpic.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gjjavqdpj.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gqzncupxj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gbiigwexc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gxrdilylv.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gvhatbdhr.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gfhxbszbr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gkhwpulcb.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gucwgqqcq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/glbtgimvl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gbsqkwxnr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gwdxqtxcn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gxjqygygq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/glamugkxs.sHtML


<!-- 参考信息 -->