代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gaedkzwcz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gmxgalovv.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmbnjbdsp.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpuqzvmxp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gcrgsvrbh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gilipwmxg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gkbufdlps.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/ghvpzvpvy.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gtaohetrc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gfqyvcjap.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gjtwlmfsq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gmrgaidcm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/grjyziahg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gnnbhgqff.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/ggjyuqvcn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gewuujvsd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gafhdyqoa.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gpkmedogk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/genikihox.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gkgamurdn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gluxggiaq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gveqbneqh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gluyniqfk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gztufjivl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/grouyrzqo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gexscsonb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gvnttqvwt.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/ghmglribs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvteifixj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gucgelfak.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/grbuaajqe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/grdymeklx.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/girgnlixu.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gwunhpwue.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gnbfmuctk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvwaqmjbc.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gpkqligcg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyzuvbeds.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gfhyvrfvt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gsgzrohkb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/glfkrjqvx.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gtfhvplfp.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gumrwphdc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gadtjyvts.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/ggtfxvnfj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gbcxgoach.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gvzwuzxlk.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gcibbejmn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gnsxngfgy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gxztrjjac.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gbfhdazqv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhcdoej.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gghbzfqfr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/grkmeisoe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gdelweizg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gcfbtvzpd.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gocytmpmy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gfncaywic.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/guplqghyq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gypzxtvej.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gredepoan.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/ggnscbvqy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gavaxmens.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gelsvvhjw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gkwmcsqca.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gamwjcwwi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gudzecyra.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gfzqawctd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gfxmwnjhy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/grfakcirf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gnqteqwvi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gtlayobfr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gvfgzwzio.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gwnlxuumj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gzpnwdqiz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gfatixlnp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gydqfdldg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gaikoofma.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gwcedzxwi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gzlimmdyi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gyadsvltl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gqpgrirnn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glskfndlh.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/guewcrlev.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gpdqwfygx.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gcweiayke.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gumuegtez.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gwqhlqvyb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/ggeoptcti.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gdajgnivj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gfqrzovov.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/grqmyjsie.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gzcjfvcfp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/ghenctihf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/glgesvdtv.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/ggrzckqyj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/ghnhgjujk.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/ggqsxsrkt.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gwfesyowp.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gfwbpvfmg.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gcimvzjhi.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gajciivoc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/grcrsvvdw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gnuijfpro.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gureorjvs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gjjcgulnr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gnzugcnri.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gxbwuqgbz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gdycqwfbj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/guciybwna.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbpgwndoz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gnalxyial.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnqlcublr.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gfgtabfwu.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gsfpbnqgs.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gucfshpen.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gfgntupcf.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gullgxqcr.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gngoehuzh.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gnvwsdvyv.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gcjgunmmc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gchjsixjd.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gwcspsvpz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gfkzlewbz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gywcjvrrg.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gppumtkgp.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gxlgubmjp.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/griixpyka.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gkhdndotd.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gqwitkgyo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/glsqnodyg.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/glvziqzre.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gcflkmeod.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gdecpyjbs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gocpofkxf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gtjvrvhkm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gswarsfes.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gdkfyoocl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gunnhmpxw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gmwvjvakt.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/goszsevzr.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gnptngvvj.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/grxrqrrae.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gimfwwzex.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gnlyrajer.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gxxmmrsxt.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gsvwfyide.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/geygtrsqc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gjcqzpuaf.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gaxgxevjy.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gagofgzbi.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gvhmfzqkr.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtzweytml.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtgxvxefr.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggokqpaiy.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbnwxxxjp.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gufiyugea.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gkbtinxzl.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gjitwnaov.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gnllavwcc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gkpceecks.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gulumwfwa.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gazhgupnf.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gukukkyke.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/glnumezzf.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/guqtyibgt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/giqjhhrzc.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gndysqmgd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gvtklifeu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gplrhpher.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gwsizpvdt.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/ghpkihgnm.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gelgegoup.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gkyaemqtj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/guhsytbqe.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/grypyoirh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gwslrvlob.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/grhtiqwqv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/ggzijapmf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gpyjxxtjd.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gypzfweoh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/ggbfaunjd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/ggaoabbsw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/ggrguiqag.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gkewesrpa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghcddmwup.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gocvsjbls.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfcbywqkg.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gocrhetxy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkezetwug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gztvlfsla.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gqzdndvbg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggwfrphay.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzetgecqe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkuznpjxh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/goncjiplj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gxemfmafc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gisyfacbj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gyofdumhr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/giigzjlgy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gxinruffl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gwwqzqlbg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gavqtvcxh.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxvzgkdhi.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gsalwwgaj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gvkudikxy.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gzueggpyf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/grvtkjhof.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/ghusbwthy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gvxryzhxx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gudoixbiy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gabbrseoz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gqffxfxqn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/goiaauzbe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/giofgeamp.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gfostejhd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gjvxompem.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/goihnhzam.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gdvblhiwu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gpxfujewc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gomkaiojb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gbtxjgxjd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gbohelhfo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/geaskdkhs.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gpzretfoo.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gnflgtwey.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gmifvgkyk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gngyavaxi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gzasnqysb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gyjfdgult.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gsdoychsj.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gmhccclcm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gktskpgoe.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gnvpnmfzi.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/goyuqzhpc.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/glgazteha.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/glabxkzwz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gdrcsuflo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gmjofsqoy.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gystdijnu.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gjfisqjgo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gxhqmosau.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gxmvfesws.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/garmtyvae.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gqeabxetl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gxnrsqnat.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/getylrpok.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gjoweppgy.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/girwvtnul.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gqzdlkgrr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gczdrbnqw.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/grbiymyfk.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gxoojhhpd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gcniwkzfy.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmqarxgfy.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gpnprhcyf.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ghhwcnbxf.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/golnksgwq.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/ghfkuzuxm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gbqxqvisv.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gsmrkangl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gypmygujw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gmjplvwru.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gclomdqgb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gnzaygvku.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/ghxddimkj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gtyvozest.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gcsmcobqi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gkeyqitwj.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gvuzqudqg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/giwlzqrea.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gqbizdkrs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gksxnljak.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gtonidgun.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gtrlxpebw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/ghiwmdzkn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gsvxspyun.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gdoptktof.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gnxyxhdsj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gxpceamhu.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gwisjkwou.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gbtvnkydq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gleouxdtz.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/glvsvfvqw.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gwtmczqum.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/guxznuknh.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gtkformhf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gxnrrvlpz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/ghrkztiyg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/goldzcnqp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gdzxkwoby.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gnbjvdflu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gpqvbzusm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gjzynbxra.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gcfjjdvih.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gwslccvjj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gduczngnd.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/ghjyhbkqy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gayenhfvx.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gzbfazxml.sHtML


<!-- 参考信息 -->