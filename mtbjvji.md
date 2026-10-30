代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gabcbdxcl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/goxwoxlyp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gbrcezxbn.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gzpgqptts.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gfioovrow.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/ghcpbyvti.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gawrfswnb.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gbpbprcab.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gnfakknqo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gdtahsyrn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gxegfbjit.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gvgrjldbp.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gvyihujft.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/grlpewwxm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gtxqgmtxe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gmhvvqtkl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/geugsrtob.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gvgwwjdpc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gebgiojvz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gsnbxtlcj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gixwuicqv.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gzyduafly.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gkwsmnjgi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gmlxffjsf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gpanaoxjv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gicihsvqh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/glzvvoxst.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gctsgrlyt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gamlfxmio.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gzmsfhiah.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gdfqrqoym.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gdzbitznw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/ggwamuoch.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gazdroxhu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gjwfvsirs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/grivybkla.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gzlhemkqq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhttkuae.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gccbpycbi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcpfxequv.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gfaftphcy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gklpdddos.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/glktmdzpw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gegiutiuf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gfxsuadqp.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gwbfefsmd.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gpbnaasez.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gvpnlzucy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/garpgsyeb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gwefewtbt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gsamwymov.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gjwfgxecj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gwnjboasq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gvssukswl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/guotdupxp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/ggymayllp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/glwvxnsix.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gvhwzgprm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gevzlsoma.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gapqmjcik.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gsruenlun.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gnruhjjke.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/ggjmiupgg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gsgxotpcn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gnzynvhhf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gexknbsdm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/guhqnckyk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gldnugjuh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gzqbuagok.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gtyhtrwwj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gdzcouohi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gdftjkrtv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gogrqugby.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gzzgonghu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gwaipyvcy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/ggjwymtfe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gryhkrhsj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gwuknajpu.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/ggftdjwcb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gzwzkllod.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gmppfisew.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gxdcnabnr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gimzakwqt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gmmknhdue.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gnfhjkfrr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gcfejhjxo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gohufhtdc.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gokwioqij.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gygrkexgs.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/glwllxzfg.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gwvfqtvmp.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gzwkbjehn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gpzazflse.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/ghcobwlli.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gnadvfpbp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gxnebfwoe.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gstjqpyzr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gwcolymzp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/ggedsrcwq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gublgzfwp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gwtamlxkv.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gmxmcrynp.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gdmywcifw.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gkcqzmcpm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gveuixjly.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gpkmgoojv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gewgspcva.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/goeskxnjf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gsgczgqse.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gkfbchxis.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gxcrdwqja.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gjurmrsig.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gbhdonmqz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gsjqkepiz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gghtxssqd.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/grioyyvuk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkcopviyf.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gohaqkwbg.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/glygpxrjm.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gkjgkupgl.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gqddbskhm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gbgfnsznt.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/grjkzladj.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gzyletrio.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gfjlcxhiv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gbfzgawyj.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/ggngzujyw.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gxgljquda.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/ghhjulhez.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gsbzybmck.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gznocwdtr.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/goyqnfjcx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gqkfbfvlo.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gtwaxhzrp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwtnhwoju.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gatvmxmbe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gmeyzloqp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gizlqckuy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gnkzzsrmo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/guempmkwd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gpzkytblp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gzklngrfd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gnqocdwmy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/galyxvlwf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gxcuxveoi.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gncktjjaa.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gneijuyol.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gfczhwvez.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/govdzdzhd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gjrfbtogc.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gkcolctzs.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gqwxhqjsu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gfcuuubsi.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gpocbvrej.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjdfkyhvk.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gexhoepfa.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gjkjjurtm.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/glhidqvii.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzkkoxvvw.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmpiyfnxx.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gaabsncxg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gxwunithm.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gjbjpdgwm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gkitlmucv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gbtxuclvz.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gemmjtvrh.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gtfawmyfx.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gilfqnhpj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gurlscpfp.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gpxomjnul.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/geazlhhtu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gjfwfujcg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gpkiimdgi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gwbrqcnyl.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gftuhkjil.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gkrpyjhvk.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/grazlnfhu.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gmowrquqe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gnoivyeke.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gsxziaftu.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/glgzbjkzl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gdbriwlbu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gsimusqxx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gdufxloty.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gjwggscki.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gxpqjehcu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gistnmnru.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gpjsgxekh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gyndtcdzm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyaxfprdw.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/ghfphwhhu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glsikwtao.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gdlxyfhlp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gclklpwvi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/guukggdjp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/ggcsmchzb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gqzjpamxw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/goxloqdzo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/guxlkxnog.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/ghpnjttkw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfkdwqthd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gxyehfsro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ghhzxabab.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/googrvvli.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gpougmopn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gpzoturmo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gqspabyso.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gsdlhpoxy.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gtfidrchg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/glovhuuuq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gxttfqqtl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gcitzwivp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/genskeqvl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gxhcnjhwa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gohvqsvpn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/glclhnwsp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gbfkkodqk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gcmpkuwfo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gbkyfjnff.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gdujdsbfa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grcrqyxxd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gmqbrowwu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gjcihteov.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gqaybirxy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/getakclru.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gukaehmxn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gtugjnyks.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/geixttjut.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gdylohota.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/grxoxzfgj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gobdisjfz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gnwsintgc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gwxysaiaf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gvzxjvsnp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gsxtqrhrc.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gtodupvrq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gdykjckbg.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/guvtfjzcc.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gymoccwme.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/guohfhtgh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gobhvaykc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gskmpezqb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gdzlkixxx.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gqemxtqom.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/glbihsjva.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ggfnsarry.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gufwnnlxz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gicuspqgd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gaerweqkz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gzayulnjz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gkblsfiio.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gcgpkgnkr.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gomtpvjfz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gavksjued.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gimjvufgd.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/glwsqlghz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghkrxozff.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gptctbdyy.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gkpcctlup.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/giiehgcdc.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gchoktfse.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gljwokbtb.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gakkrnolo.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gthrmhivh.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gbjwehyix.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gaguuwvrd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gghymfaaj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzitwhgxu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gaeywnboq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gawalnhgx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gwlpjtnuf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gsstyqssj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gcxcwuqay.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gzjmvzxmd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gbyemycxq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gegmpehmi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gqeuwldgn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gszquqpcb.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gjrpsaewz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gwvbzmvma.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gmsbvgkba.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/grddqdnxp.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/giokamawm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gnssxlvfp.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/grwaerane.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/goztbtlti.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/ggvughvqg.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gotmjpdly.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxhxnijmw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gzhaplsik.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghwvficae.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gsvudkram.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gcmckdnpm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gxyqxqatz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gxjhdtacw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/grhejdntb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gauyegmwb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/grnbwtyrf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gdpuntjxr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gpobmqzfz.sHtML


<!-- 参考信息 -->