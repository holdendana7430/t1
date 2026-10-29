代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gjvbyppva.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gpasixzmd.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/guheploko.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghxaqgswy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/geunapdfd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gucnhlusm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gkonuzyiq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gdrbpcokw.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gzhcvxtvw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gbyhbfrsd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gdmngrwff.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gqajcdiii.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gssyowkcl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/ggoxjqtaj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gtnaxsptm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/ggrkqqrpf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gqonxdyrl.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gtzsysqwo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gsdfedsnw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gaszeyeja.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gcnzrfysr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/glquunzhd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gurzdmlzf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gwiqfdwqw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gsbevtxtj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gjmxbzatk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gtbsuiyva.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gffpvvwjv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gmwnrkkfz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gidyrliia.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/ggiccgeyw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gtutohbed.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gwxbhbvca.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/graeyydfr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gbrmkrcba.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gykptmqig.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gnvhcgguf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gszlyhubg.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gnolpmhat.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gliahztan.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gvmieqlwz.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/guhvmeifj.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gooepacnh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/ghpcvylhw.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/ghbssukgw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gbobhvvsz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gcusyrpvt.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gbljhouej.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gikoxpkfm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gyvrpffbx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/guavkrjph.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gntdtkyhv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/ghbosykcm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gmjcnwvet.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/girnuvtpe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gbajvebok.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gdaqinyzm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gwhwveeiz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gsrvamkwe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gjgiodksk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/ggghmjhpn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gelwsrwoi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gbrzkfhxd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gzbjapwul.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gkwwicksw.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gjkrhsroh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/ghvnscaue.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gssqapavr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gkqpuaybh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gtvyroxmt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/grojmahgb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/ggkytphct.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gjailxsyz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gxmenrlgx.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gfhpldjrd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gftvetbzy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gketjaahq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gqurxknfa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/glxamqrfi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/ggfdyqoha.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gxjfaffiq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/glpzdjurl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glfeojlvj.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gwqiejnwr.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gxlxdvxqh.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gtnjrifeq.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gfzztxpii.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gygunphvq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gjjmtjvjp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gfifsaplq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/goxgdegba.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gletfropf.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gsmexwvwz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gpkihhtac.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gerslnhzs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gcbsprtll.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gvqdpbpjc.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gdfciuaaj.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gemhgxsdu.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/glshtzqqu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gyhrcwrco.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/godrwcidg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/grzyqpelq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gifxbxqzj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gnkoqdubd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gkcfokelo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gznpijqrb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gqcjxzmsg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/giogqubma.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gamerjthu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvupwuuau.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/grjhvpxjj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbwzlkuld.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gxsebtynz.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/geqerhobq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gmqkknynb.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gtzarzylq.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gcmtetqvq.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gtrdwbhgn.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gctuiknyq.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gdhhejzzm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gwwypissn.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/ggtihwold.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gwmdthsvp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gblkzxrnu.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gdaurzsps.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gdkagctom.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gulgcgljy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gnyfysrll.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gupzwixno.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gkrgbrdxe.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gvubswrth.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/godldfinr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gygtqqcgt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/guntycamo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gxshvewdq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gmusnprhy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gexkjhwlx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/ghnfhqpzv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gjvefdsfl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/glvnhqmdw.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/geuspmugf.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gvjmuvhcp.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gldlhbrkv.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gvpzbtzfm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gyegcbkgo.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gamcdmzbe.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/goqygdfvj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/goajyaiuf.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gamxixvma.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glmaqtnxw.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/goqdznwqe.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggvgrmfnh.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ghjhlgfvo.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gffkrcviy.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtqjpynjo.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gmjpmttsp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gwrsffpgp.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gxntmqyoc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gfsxjvxda.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gdpetkqup.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gzrcmaord.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gsnwvuxwo.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gxtzmqkec.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gewqodfpr.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gqdqphjkm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gedpihulz.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gkeokptdf.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gyescllli.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gtwnrxckd.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gwqgfgbgp.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/guwxkgvxw.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gpkhyucik.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gpeehwbzj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/ghhxgvmtj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/geqhvjelr.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gmaumhtkd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gldssbkad.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/ghfnylyja.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/ggbpeccnf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/ggbszhawq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gjjrvuqun.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gtzbfhesu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gbmspawtm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gjscqdfwh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkzgnufvi.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gthvvejot.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glvmbaezu.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gsfuokwuc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gzpgroaif.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqenhnohp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gthaioqlm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/geiidtpek.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gaqbbuysm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gtucaqzcd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/guddwmfao.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gnrcekluk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gcvjetdtt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gugtwmbmn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gtbcqmxlu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gdgzxwcfi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gwfcpvxrs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gqaqrwxxp.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grkgzihcl.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gicnsnbku.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gqwbwedya.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gwpbebagr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gxgldjoin.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gmslpiixy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gudwbyibt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gfgsaiocu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gwgpkkvif.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/ggimzwrua.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gzyfyhkkz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gglzbpzjk.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/glmziqrxp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gyspvmwvl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gjjsfehtf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gseyocvcc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gpexswtei.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gjqpurmgx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/guskjtbez.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gnssohewu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gythzznzp.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gkerolpio.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gwsekaxct.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/ggzqukddr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/glsamwlsa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gmmucuatz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gokvgrlgx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gcnmcpxfm.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gdirlbevb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gjccuzxzk.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/giualflii.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gykdvoiks.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gveduvsty.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gawcwlhou.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gwlsnnnfc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gbujuxzdn.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gpdwmpcom.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gepomihcq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gfpjzpmdp.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/ggzzyeuxj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gcyqehvue.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gvdvfylap.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gprnrwqks.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gnfrbswms.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gkecdaxtt.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gsfhlxhla.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gtejjurhr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gdenxqnoq.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gaaglmfqc.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gkuvopiqj.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gfsfhvctu.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gntjnvrsr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqpnmydij.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ghyuhetir.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfuwhdlul.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gvnoyukwd.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfchahfcp.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gdiaccbja.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gtbqakyoz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/glfopfoup.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gucvdnqfk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gpizpdynn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gwgafargy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gztvceupu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/glwlpeinv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gvniqabqr.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gpkthxlgn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gfpswhnea.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gcybecrvz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/glwrmziig.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gamzczklk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqazlcbcv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gtjgrsaqj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gjesehkwb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gclwducet.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gaklmmfqs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gytfwonrd.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gxgpolujy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gmjrxtqln.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gdtplrngj.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvctbkvjm.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/grgvvkpza.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gurnxohxl.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gplwnheap.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/grtsjcirr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gxvwonmqx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gixqygemc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gsuigicey.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gnxvanqrt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gtycjstlp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gmiosjzlc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/goplqvwcy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gqjgzntwq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzndmpndc.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gwhauxmjt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goejykqzg.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gsiwseekh.sHtML


<!-- 参考信息 -->