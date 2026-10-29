代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gdsjnkjfk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gplddabob.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gxbuibgig.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gkmpnyavc.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/giipgpwyt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gswryuvrx.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/getopyans.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjqyxvdip.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gitgfhmut.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gvadbpfdq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/glkjowlqz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/geyqzshkm.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gkuhjcldl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gtkhxdqev.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnkhpobng.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gezedvlnl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gaxkryrxb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/guzyvyggx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gnrgdukzc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gpnjnkdio.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gfqktvkkz.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gfjafcgxl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gubzidesu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gxcxoavdo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdeshmazh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gchpaqgxu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gdgikkghf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/ginaodalv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gtbbmteaw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gjaalzxpp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/giszuqexi.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gzgaqxxiv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/geijmgogx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gigqmftnn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gkvaymcgf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gviryqzcj.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gurwcxyfk.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gfwlevqnb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gakoeeqst.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grlkxapmo.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/grmsfbfbu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbaorrlda.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/grmszkhnw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gigucqedx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/goshtekgl.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gfbztetxg.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gpcwvjxmx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/grhewieiu.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gcirygxfp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/ggcqckqza.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gkfwyxmlb.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gooazrkxb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gdzyuxglc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/glsdemaru.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gdpszofsd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/ghnqkbzqf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/ggsxafxqv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gysoxapvs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gksfrdrqa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gtafpsmzw.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/guwaiwwzf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gakxprtqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gdgmitwgk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/glsmwjzwm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gquroqgzd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/ggqhyoivq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gpahypmpa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gijjipndw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gkblsqjko.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gfaamijpb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gyvvjkfhi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gappszpyz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gcvsnnhym.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gccyexrmd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/glmiqlloo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gwmskhwuo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gdxfeznxq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/glcyhvjox.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gkyoompwn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gzftfrqap.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gbwckjexv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/getryopvb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gwsgofaxu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/guzviycsp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gkdpfeqei.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gpgduvsof.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwomagurg.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gqfdwgysb.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gkmyoobqf.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gedkmrydr.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gqkdyspsh.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gtcodauxr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gvfrpnuds.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gwdjfsrwd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/ghnppklrv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gmelftpam.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gpvyfrcmf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gimvgvxke.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gyecapuvi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gzaajycos.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gpkyopiat.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/ggifawwti.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gitdfrkdx.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/grcrxmgvu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/graajektk.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gqocpgzvn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gvdnyjzmd.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gopkdicra.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/glqhhixle.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ghrsjgajc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/ggwpifbgq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gufsuwerz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gqxucigwv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gvdzqovme.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxnpjljgs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gvtuyeatl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmgjqmypa.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gpvebcdpf.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/glilbqilo.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ggvgirqmr.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gsxhnqjsn.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/glqyzwjhk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gytahbsua.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gxszcglqy.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gogswqpct.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gqojevgxb.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gskoqgfnm.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gkzsuprym.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gzdywvena.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/guohtadef.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gnsjbvozg.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gtspyqnfi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/grwrlrjnk.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gdhyuwmvb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzxyoyioc.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gsyledlxv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gechnidcz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/ghecpricc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxbtwmiqf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gnayrmetb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gmfiindkn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gpnoeagfn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gtjatclto.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/genlrahfh.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/ggepjiltx.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gsxpwrdgb.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gtknbuhbf.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gmkyhfkxi.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gldninfxx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gabmzwysd.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gmuheckjw.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/guxkrstmf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gevckirce.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gdvkgjpdo.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gjwapqhla.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/givneymul.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbhcweoeu.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gzmkskvbn.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gldcxarby.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gavpuibgi.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/ggzjzqdya.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gfuucyqdz.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gpyvfkaak.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gmpugcexp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gsaqfebqm.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gjyyeagyx.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gerzimiwu.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/guybhncjh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gmdndprmk.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gkteziakf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gylfuzpbe.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gdhipppzz.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gjihohanx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gcrsuguty.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gcazstoqc.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gmyngsilb.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gjchpjsid.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/grhazfiwe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gvmnylqeh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gkpxmspbt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gflyckvdy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gudivicdu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gsemeloyu.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gdygpcabv.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gdrpiuzvb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gpedluzky.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gabfqhxua.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/giasbvwfz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gqcigxruf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaezdjvcd.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gujrqzicy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtthyqnnu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/genneyqkz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/glwlopkwc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/grclprccf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gojwqpmed.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gwfppbyek.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gdmajuzvw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmfwasrdf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/ghmmacmss.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gasfsltjz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gbhqtosvd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gdndlvfgd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gwbwehkys.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gwebmejca.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/glycuzzvi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gpghyeuvj.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gtewlytij.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gumdeskbn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gymwpomyu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gsyjdvyar.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gvypxxlow.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gizcnjajv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gdjrphbii.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gphjhgipb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gnizeidie.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gpuhjtekd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gubthqshi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/glbfbcnmm.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gxgkvuxze.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gqhxkccxu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glhxwkjcc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gdmzojoin.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gnqyvyynr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/givzaouyi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gjcjomsfk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/ginqeywzb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gfsqcbjvk.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gaemdzsxg.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/ggvgybdyv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gsnbkrmuj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gvnrhhixm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gbnmljhwv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gfwummusl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/glqsrhlhu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gbltefuxh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gzkitykml.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzqiuvhzq.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gdmjexcyh.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gjnzfbcgx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/goincrytt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gtdtvotbr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/geukgcesz.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gvvjyfsgj.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gobujhoms.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gcbbtccrk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gvuyrodxw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gylcbszup.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gvktcouef.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gdffcjlsn.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gcgeluwwn.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/guyhycamg.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/grpesxgmu.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gfvzhbjte.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gaxadqauc.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gkwgpaoqh.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gldxokavy.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gzhzxnssy.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfycufqli.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmevvwouf.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ggkfboapo.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gbcjhtami.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gbacwiawj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gjyhydjly.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gtwvxucvm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gelyaykxz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/grbksimzv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gwetvsebt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/grythjjjq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/glwaqdiyl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gnxxtkgjr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gymuqxgkf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ggpdoitwx.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gvjfpfmrq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gumtimgcv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gbchzbvnx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gxfozpiyh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gjsmlkiuu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gflyjeulo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/guxeaudav.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gqnluhvar.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gtvsdwztm.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gflgmufwe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gxwzsogvc.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsqekjris.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gmwzxnsot.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gmltkddzu.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gorzujhkq.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/ggczsylxs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gcabrwilt.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gdqpnoecp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gofiobwyr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gnolpsevb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gtiwgntjt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gwkvlbvup.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/grcoghbby.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gthkgoipr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gylfjkrsj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gcyjaxeed.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gamghvnfc.sHtML


<!-- 参考信息 -->