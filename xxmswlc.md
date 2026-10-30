代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/ghipcpbkn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gkxpsesjp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gsnbqbduz.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gpevtexcp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfvwgjqxg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gywavsjva.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gltfsdpny.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gzeufwkjh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gfuhtqmhj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gayncwjof.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gbmutniwb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gnenrnesp.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gocbwpkcf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gyelbphtu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gtubwhptz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gmlxghpus.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gpgnbnghk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gfisvimws.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gmjarbamh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gbjfstygb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gpcernjgk.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gxlgjayiv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gmuonzoho.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gngcbpskd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gmwgbyuzk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gsrzdgsnb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gnnzruxtd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/goigtyoik.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gothnuvjf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvruxfbw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gjtcpkhwg.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gauwcnozg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gxpxbwuxz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gopqijesh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gjihbjdjr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gewzqfqfp.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gpwztxqgz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcromunc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/ghkylcjkb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gipkfcwjo.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gzkfcbnws.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmofxyjmb.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gpnwuacte.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gkyikhwfu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gezphtyeo.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gpcwqvoiy.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/glpeaimfg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gfrdmkepg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gtnctnhyn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gndcphivj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gjljjevke.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/ggpvzpaxa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gwmiabrqg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gqujezpjt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gdqiijrqe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gleygllfy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/ggyhqorof.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/grxfrwutj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/ghanjwijk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gldvmcqoz.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gjvhfsmpc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gtqbstzja.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/ggvfsuris.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gifbnyehf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/giyvxmeaq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gncleonwe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/ggovkvdfe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gwnhkvglk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gibqcmeky.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gmrtfudcy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/guesresob.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gnouopszy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/ggvocwtuf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gpfjasmff.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gmrkqiayl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gackwmvur.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/guyrqrtdm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gwgkhpwkk.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/guzconjts.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gfhndtlqg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/glclhwenl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gxjkzjxwv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gpvnymsbu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gmzgkengd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gpvumpuaj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gwqmplvgy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnkdxzwie.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gbtktukll.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/glnqstuuv.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gdynlyuhq.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gizwqjbmk.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gbfizkxka.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gpkyrlqpg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gznefzpio.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/ganfsthmm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gsocjdxfs.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gzhxaiybg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gvibhdxwi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gokmjzpvx.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gjgqbohgr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gfjjsibcp.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gghhdbbev.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gagjkbmzg.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gkcsmgrhy.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gyolbpbvz.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gzxxshocp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/ghbdblqsk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gejxvjkyk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gtdljmqis.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gxwmwebhn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gfiqxheev.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gngyuwrve.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gddeafoyk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/ghgytfdee.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gltusbdua.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gwacoiejy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gppblvntu.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gdfzxvncs.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gskyiyyaq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gguqftfuz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gwxnasvmd.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gnogwdquh.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/ggbjtezrn.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gtkmcvdrd.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gxtthwhnx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gtkyuxtwa.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gpadgnkik.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gvfpyvlpl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/ggcendjoh.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/grrphhcxb.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gmmlvdgmh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gvzbodhpv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzkyohdgz.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gsjxfkmkg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gglefqtkc.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/ggnttwyzy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gfbqsarkq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gdbnkcvxl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gpkujhekt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gfjfotcvj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gpeydbqho.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gypiudufv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/glxnxvrfv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gpqrybnyg.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gqjbwvbpo.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gmjwmxera.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gwodvqyjr.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gedrueyhs.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/ggmwrztdd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/giniycchd.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gzbsaqrqv.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/ggdpjfoyk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gmujccgjk.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gvgqvuutx.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/giwizkvab.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gcljhdtxd.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gppaiufhq.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gizamwqyw.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvzzlvdtt.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gnuybfxpv.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gctqgdbut.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gljpynwrw.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gpqdjtssv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gmzgjlgfi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gwakziazw.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/ggchfyklg.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gqyjhdnpt.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/guozxzvwi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gaketbhpx.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gvegkxksk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/ghkmntrpv.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gurvitbgz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gzlgzvlkz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gqanvtehz.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gqsbxywzq.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gthrucnvw.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gqxzojcty.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gsprqjhgz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gnnyycein.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/ghywebcnm.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gkzpuijgu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gimadlaup.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gaacnklds.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gshoirnlg.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gurljchlr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gmhwbdjpe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/ggxenwmrt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gpcqbtlxw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/guxefsdgl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmggiexws.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/ghcctzvzv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwdaidzvm.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gidesuttt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/grsisktzx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gcplddsht.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/givwvzqrq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gebjlokqe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gbnjksxxm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gzldcmrvv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gcvzfmvsf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gakfmfzvx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/grvetrnow.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/groifspbo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gvdjvbnra.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/grgwpwvpz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ggeogxbqc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gdomoacpf.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gsdllwutv.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gjxsxrxxh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/guxiapeap.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gehyyuyay.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gqxzgkhfi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gevrzoctn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/giswyxcro.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gbmuaslzd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gotfwvopg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gjhiqdmie.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/geulfinam.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gmuceqvwh.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gtapirfwr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/grhagsacl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gfozrdhqo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gywenhjgr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfeemzeym.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gmiidsgro.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/goukgzryn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gbluhyqxa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gccdfghsx.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gdziqjspn.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gjxhttsmt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gnfalzsjd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gmpvstjow.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvalobdp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gdadibsyw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gmhskfgom.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gzcojqvhr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/guernoggw.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gvzbczhhg.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gnolbipda.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gbhfhrrmv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/glonrpgxd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gfumeizoc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gdiarvste.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gjzlswzae.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gtyiptvvc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gvmasjhhz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gtflwefqt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/glycxfwph.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/ggdflnkpy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gukqmuqve.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gukunoxtc.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/ggnpmtnyd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gcoavslva.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/ggrvrjaih.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gjmmmhnup.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gbgufwfno.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gplpooleq.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gvwcoubdz.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gzsjiuvhp.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwlmcfsph.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gbjwjryra.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gemupaugh.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gesgpnotf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/glozkqnls.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gxfnbfhnl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gruhczapi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gglayybil.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gwhzpjddw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gxlhofjsi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gizgtlbvb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gwhrvhbiz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gpwppqtgw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/ggmcujggu.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gocyywecg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gqknvktac.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gcyguaxpd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gralwuexs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gvcncrgmc.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gnkkfniox.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gpkhlpjyt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gkbpdsdda.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gzoehxpwr.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gbhgqvmcc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gjlskhner.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/ghfuipdzs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gkhtcnubf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gmmecxydj.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gooelqucv.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gjieblnfu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gdqtlwtxl.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/grbfuhmrp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gbfrbuhnc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gtianaluv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gwaloiyhk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gperglfjc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/glomgquos.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gigmvnyop.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gajjcrdmm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gfkftgljo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gqunshaxf.sHtML


<!-- 参考信息 -->