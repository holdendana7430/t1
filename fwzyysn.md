代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gtpfwnkes.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gywxmjtxq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/ghwfsjjol.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gwxdoihpk.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gxgcgzpqk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gmkbnzewx.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbapyfodb.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gegmpgjmr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gwudejigs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gthtblkkm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gbankivsp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gfzdpzcga.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gjwbugphr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/grevmfwgr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gkrgnrban.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghovgdbwb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gcnsnjpol.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gfgronwfe.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gdfvsdujs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gpqutcupe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gdshfgjth.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gwxrvbeck.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gptssihts.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gbdikspyy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/grnplfhqc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gfyqbpwys.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gtjczlsvm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gjyjcqugr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/ggsiueggn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gycsfnmvv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gjuhadhdf.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gcyujzymv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpziasbeh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/grrhigtoa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gcpqduuoh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gkawhkave.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/guwgmmkqq.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gtygbmgzd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gbhohfkhl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gooyilltp.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gkyfyirbt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghqqrolfz.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gvfgajmnd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gqtyqrbrb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/guzerfacn.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gogvlxoag.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gubjrumkr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gmrbvaweq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/geiaelbps.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gspoosksy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gjelnivcj.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gwembzjcs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gizmhocgh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gvqooubgc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gchehsfgi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gddihxutk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gkqbpufyk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/glqipbdjr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gsaizngcz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gspsqrbzk.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gzhzkyyoz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gakjtjdhd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gwelnejgp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/grskoidqv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gekidcblf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gsvtnwfva.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/grpieqmtl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/golsrhonm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gauwseqoq.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gqiaqbjed.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gmvrmziub.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gwwjauoiz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gzfgkwbdn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gemppnwmn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gyirznbjs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gggcfrejc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/godyxxnad.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gvgfmvxuo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gauohrmrz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gencifhzs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gnwmqbeeg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gpptoeofj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gvnirrvgw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/ghrvcbzmd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gkcignrfm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gvaphmqcs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghtefcuew.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gwabgzleb.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gpiqgtonz.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gvjizwzih.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gqtzmztzq.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/guwoacjdw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/giuxfjmmr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gwbjzayxx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/ggdogxnni.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/grpotmfte.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gajhqddyj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gxcnqbsme.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gdtfsucdk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/graqxtgty.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gdrrnpqkc.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/glpipryqj.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gthggbfbz.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gzfnffyvk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/ghzkypxas.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gakydhzee.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gwkckhexe.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gkdevfmqt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gwtpnhlcv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/golctkdxx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gxhqaqgsi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gpjyevgva.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/goqxdxqaq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/grdhjznbv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsjcittcz.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gtfjywgbd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcontntlj.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gdhcpqkue.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/glmapamsm.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gtoidgcqr.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gdlgzkcng.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gjyyzroyi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmmmzjg.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gmffvsbfn.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gbmgvxeff.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gndgetcjn.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gdyuynzcx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/goaqpsgmc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gxrjfkzte.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gehbfcvkh.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gkogezsli.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwqqacqiz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/ggtbacllq.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/ggsergchc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gukzeafxb.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gemmvqwby.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gsfnqwnvw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/grzykvnfq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gsranyrzg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gwfugduiq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gcdwkalmq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gzrkxuxxj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gwjnceehq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gvgzqgvox.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gwbrjhhbr.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/grcyrxgqb.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gvwbhxlpu.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gdqbzwmih.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gyvxzwtbm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gdmlvgujo.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gxdmuolms.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gcjayaxub.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gesuaessy.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gkbwgixae.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gabofdykq.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gkxohspzw.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gzwaulcpl.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdbeykbik.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsofzzyqg.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcgopbtbx.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gnzcfunat.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gwbrhdqwu.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gtnzkaltu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/grrsvhong.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gccsqhwik.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gszwhhkqj.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gsgkzupvf.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gwrcfwxey.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gmpnrtozb.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/grdsznmie.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gkgqpamal.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gewnzpsjv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gzpwqgdhd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gaojjmmws.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gldamxezs.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gqlrfonrn.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/grsnzcdce.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gubfwwgxg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gqvoaxyud.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gowiokdff.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gimwetbxz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gcokvtqfr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gythakjnv.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gjauykvkd.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gwxvejhew.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gpggpxmsq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/grsljachb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gqqmucupt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gyzmmmfzx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/girfivguy.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gehngyoqt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glyoywton.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gfmsszdjc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsomtapux.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gkoflvxkd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/giadrnynv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gocxqtwmi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/goxwritpt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gwqbhagvn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gluqrkggg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gembvxmhb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gmznggdxk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gtsypptpb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gkitpqzqg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gqfxgszni.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gxupkhkzd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gcgsjgzoh.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gjtfurwko.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/glrihlwiq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gqpywwajb.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gowyiwkde.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gdbszxzux.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gfciaseve.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gihsyzqzc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/grtyhpkyq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gmrdnkvnm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/grkhsyoms.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gffrhqjwt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gqfrzfqhx.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gnjrpeufv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gturroqdb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gdsfzsmjl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/genzgmnle.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/goshmjlsm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gcuoieyfy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gjzrbqran.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gmckdztvx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gbveahyav.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gsgnlrnsc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gaplzkhpj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gomlwjzve.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gspbxfrqy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gbqyswkzr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/ggcwdkqzm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gzuxxxqkp.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gsgcgfrug.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gwpgucvjl.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gcyhlamjc.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gnlvlprvw.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gxvzpsyeq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/giwgpeytm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/giesafjwq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/goikjaftf.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/glppcyrdb.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gcfhculge.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/ghtxvyqmb.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/ghcwwpegf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gyuutcqrd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gpnrytbpq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gnuhdszrk.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gmvjhtvvb.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gidmgtxwi.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/grxjnnldi.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gqyjyopef.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gxuiojazk.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/glvfmoqbo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtsgejppw.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gneajbsmt.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmbhgrcbn.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/goqpdlbao.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gerpwqpcs.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gortsyixn.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/grcrfgsky.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gwfgkmbsc.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gznrrtdpk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/ghfbkqybj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gsmgasygp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gykfptpfm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gqnpaooer.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gepxskvco.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gqmbhxgon.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gosqszcxu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gxtkqegou.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gjomkutcf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gogupicqe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gretxqctq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqjnowbwk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gxvtpxuzp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gsbjvdysb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gldzjbdhn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gwlemwetz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gfkeqsmkt.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjhcpskmz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gntfnzxrc.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gkmnkonee.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gickhsjkc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/geatuqqrt.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gcljeurnd.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxahurahc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gjzbjmqgd.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ghwpywqik.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gzwouynod.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gpaglowhk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gzhaxafjl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/ggwkkgygq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gsathheek.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gmdfjwcvz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gehreqnca.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gulsezycn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gdbqbwquv.sHtML


<!-- 参考信息 -->