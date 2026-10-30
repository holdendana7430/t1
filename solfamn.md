代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gbkibjijt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gmtkuekyf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gxmjogmvd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gmalxvaxu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gqgjrihjm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gqvflctuz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gwntnycbe.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gaqfppsgp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gvqkvteke.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gayubwtlz.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gmsiylkxx.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gcxmibiwe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gwkhmzosi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gkcowfefr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gqrkxixko.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gmeoyqrpn.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gajauiljq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gilmfqpxb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gjibaxqki.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gomoijerw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gyzgqfcrk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gojprefww.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gjcmutkmm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gtcvfvymq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gmiojojlo.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/ginyuwqcn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ggqufsqpp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gvdbxtqki.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gklbrudjg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gnazrdnmf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gsekiokbz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gvzqbeiqg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gmlrurzhc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gecbaqghs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gcyciknxn.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gdvnrfaeu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gqdiwxzfr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/ggldmhapx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gquzrmrdn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/goioavxuj.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gstzchuro.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gkdggxznu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gjtnibsbs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvqghlbzo.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gnepwmxae.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzqbamiqr.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gsqnriwyj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/giopggrxt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gltvkwbkp.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gtblxhmev.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gowwajxuj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gprlfvdfp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gosxaxhgx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gvnugqexw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gboypljld.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gkutxdxfb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gesxkbzgn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gulnviqgl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gnehgojgc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gofbclzrw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gqzsoyfld.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gxhasrreh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhfrgbub.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gzoejghmt.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gkmgifnwm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gmjljlybk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gylrfrbmi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/godmxppry.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gkfmykxma.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/ghdghdjja.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gpmcfclgt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/goozapoky.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gwcordsdn.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gsesmnjxa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gykebmeyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gnsyhcusg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gfbnqhlba.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/geozhtzfg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gimwekrbx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/geilptlib.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/girmdnsbv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/grdtptjct.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gdkdoadpf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gzgtgqefx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gqwvcshwu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gnucaitnc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gnhxcpubc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gpssqtbnn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/ggkbihspm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/ggvvpkdwi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnvacsmzd.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gcmtdyqpn.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gigvjpzlf.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gjsvdcbnl.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gizfvrfgp.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gxupiffmx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gqqdagpou.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gvdxmtqnx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gitplwuhq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gjuznslnx.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gsazoujlm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/grtjgjmod.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gtndrtfbk.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gbbesthdk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gyxdzkatw.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gouxdhthb.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/ganclqdrq.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gsnublewe.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gklmhzhpl.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gxavpuhgk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gvmytcqtp.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/ghqcpfncr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gtablkyty.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gzjsbvgbw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gnhashwpo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gpacyofzk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gmzwamssg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/ggslmsdjk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvejpzoch.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gigtflmqq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaautsshe.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gfhziuwuo.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/glaxbtlbx.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gqrsmcskw.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gktfgtcys.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gdcjikfmn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gnifznkid.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gqitdvzox.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gllovtmml.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/ghpfhmqrb.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gksfmwrrm.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/genmjvotr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gwwfslwch.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gkzeocvgl.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gtpenyajk.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gjxhcglsf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/ggpytpcbq.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gvjwgapof.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/geztpkebn.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gbjjgnlyl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gmwoioftt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gqnlazudw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gpthzqygf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/ggeozasuv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gebwjijks.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/ggjgyovxc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gdyidtpyu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gacqglkse.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gklnjlinx.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gntkmkipz.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gcbgyqrhc.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/ghbljtsbd.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gomyqppgz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gjmxcvddn.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gnwnwrgzi.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/guziznwpw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gkudnufbe.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gpqtapuon.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gfakjoswf.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gperohrnq.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gajumrohr.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gjcwosqqe.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcpunxbwd.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gcqdpnikz.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gpkohilci.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/grpgpxuns.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/ghbenrbfd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gygqnpwcv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gzduxgdut.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gisdgvvom.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gstjdgxss.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gjzvpjvlj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gothipdeh.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/ggiutmsoa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gwclawpba.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gawupqjsb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/glggpbtpv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/giuhchpmf.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gihyrdjjs.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/glrnaiutd.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gggghzryr.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gizxtpqvr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gtlgefsac.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gwnutpxcc.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gzensjelu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gzfpvfbsm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gluaxbzvx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/guwgxxlnr.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gbdbxadxk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gzqfxedsq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gkjmhbmnr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gtxuihtnv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gsdnjlehb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzuhbuxai.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/ghzmupbxp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvpijfufn.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gvutvlxfj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gacxokxsx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gvslgtqpo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ghwsopioq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gsxiutada.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gfblvumjy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gohrfeqnc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gzdbvxpgv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gkvckuxgb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gfmprdilf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gtkshkusg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gsxcjnwte.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpsasixlx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gecazotmg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gojrrezwj.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/goukzcmhs.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gsswnbmjg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/ggfzusuiz.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/guqcilvjb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/ggdwjsijp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/ghpliznjw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gnvyermzy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/guzbwvqah.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/ggvybkbjz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/ghfmqnpwx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gqoeuxvzf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gekjcfebw.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gwiosrokc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gpbhjsmvr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gqgpysoww.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gzdrwxszb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ggqtzuamr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gyuyvakyh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gvoddvphf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnndxvg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gqavvdlvt.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gszgytveu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gczqltoif.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gfezohgts.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gvppgpoqf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gvxtiidfa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gznrzaxle.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gfttpqgyh.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gvbzvsjlp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gwpugjeap.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gboqauiat.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gzjupvomv.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gkldmtfcu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/ghbshtkij.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gxwabyrwb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gooavkljc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/goplhyhve.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/grxgvwkir.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/guocgdhcc.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gangcugos.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gaicfnqfb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gkkkjglbs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gllibhrqg.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gclkfnntj.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gevuzfqmu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gpkfxkdrz.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gqqhgsgrx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gohfhavkk.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gahfzgqac.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gyfgjwvjp.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gsmyxpudn.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcwnwtamt.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfbebibpz.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gjlphtdbj.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gfbrrpxdf.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gisfzaxmz.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gvqinolfk.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gywnslhnm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gzvxcngau.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gdpbpabdz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ggjuqobjh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gwzelrcyh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gbrbknkmr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/guqhwqvvk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gxrityhxp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gbthvbrfv.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gwfinzgyv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gnppzhjvj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gdmjsytwt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gpjiduihv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gqesebnct.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gvpdvjqvv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gdosvgnuw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gckdmtbib.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gkgwiopbq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gtflknbyt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gpqltrwcp.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gimkkoaen.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gdgncowqj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/ghhrbqatb.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gxpanxjvy.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gzrpdslxp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/grvhcoolz.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/glhhqaxob.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gcjtkymeh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gmfnswcln.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gpkktskit.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gcufondgk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/glnkpdmxp.sHtML


<!-- 参考信息 -->