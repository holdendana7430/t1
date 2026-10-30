代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gemtugzve.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gdbuwnxbf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gqdbzswwh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gcyqwqgwa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gkjbxgrgl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/glpnqtwxg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gdtzlmdbq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/ghqkfvwuq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gokypuwhy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gvelhpsjq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gjixlwujt.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjazrotqr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gxvqvlzgr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gswestmob.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gjwwbqbdw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gxuszubfi.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gxviqooii.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gtfsibmyj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gjahmemfi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggkvfnsrc.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gdaujyotf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gscqoucre.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gfnqqbxwp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/guxrlogml.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gijsvuzzz.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gjenydyjz.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gvortmeyv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gefkrfbcn.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gwlwnmoib.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gbqptswky.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/guokovwpv.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gcgpkjkmp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/glestahuq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gelguhgfx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gowfhkqnk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gbnetzsoq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gzscsnvkc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gkdtvanjn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gxrndgxch.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/ghuskbdky.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/grckwvyvi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gdhkjtjss.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gjhvxmmqf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gtnpaxvvu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/grosrcprl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/georwjnff.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gebbodiip.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/geuvgbbmw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/guaycqonz.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gximpfjjo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqiobpyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gxpjysjti.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gtfagifmi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gkbpkyung.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gnbjfqlqp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gsdzywetq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gybfmiqub.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gaavptanq.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gmbsyoexp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gqiyrnyvv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/glmkahkdb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gcgpbofnn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gofawgutk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/grucsqczc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gcotdqsov.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gxlslasyz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gcophufyj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gyjajlmfl.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gbbgoghky.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gdnjerzcy.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gsahoaenh.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gczwxxpkb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gtgklxfhj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gbioxwggi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gxhimtnyq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/ghqbrwebi.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gtrochghk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gfepukjvw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gcdshuxxz.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gcannzynj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gngrjwoeu.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gpmpnrquy.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gcvacjswi.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gdoxjnzbf.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gwcizqrog.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gewtfglor.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gsoakmbvv.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gdoouoyqw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gkoukqyci.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gpyxdrjac.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/garnrbwaf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gaejurzly.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gjmsbgvmp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gmbhgqrgp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpewglkum.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gnnrlgszt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmlczvvww.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gxgjsvktu.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/grpombema.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gchzfvmki.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/ggmeuaoej.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/grioihaju.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gehpcxjsl.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/grzufhitl.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gjrialqdz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gdrzddgvy.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gncrlekes.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gchhxtedl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gprjbivuv.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gevacyqyu.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gzchazvgz.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gbecpwmyu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gumcpagpi.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gciltbpik.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gatwppgng.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gqbpzcxoj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gzvmbzevr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gnjiiymnn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gbpbjxyld.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gvfqtopgz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gqbjnlgld.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/geogtwjdi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gadejudrv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gptfaffqh.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gywolgvdr.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gdwsbxoya.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gdpqcvbnj.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/geyarwwug.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gdwqdmcva.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gqazplrsd.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gdzleceqz.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gzlbapdgc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gmpgkjwvt.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gsjiczonm.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gohchhgow.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gdnnpmenv.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwjfzimyl.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbzbummzj.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gaghbellp.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gnibtrxxv.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gwauviezq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gfnzuixwo.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/glzhogpkl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gzqblbpno.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gzmfmlfpg.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/guphmnhxm.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gqvqumbbz.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/ghthrgqit.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gsnucklvj.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/grqncpgny.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gvwjcyylf.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/glxxezlox.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gtcuadbuh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gqcpyrfvv.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gysilqtpw.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/goshcsgmu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gqwkxhqot.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gzgouqoqk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/ggzwjayjb.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/ggavdlcjj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/ghsifohbd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/grmzmczkf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gnqvzfoge.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gqdtutpdh.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gynxyogjj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gtzfnwtlj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gooavdqwr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gdbmgsieo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gauivisek.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdxgwybxa.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gczrcdmwg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gedscuyya.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzvvbktgp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghkwuahvg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gjzcdirft.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gppduomvx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gcgugbzcl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gtsswnisy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gthhcazgc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gldmffdhx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxcxnjggl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gscqflhoo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gnwtqnpae.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/grdcyhilc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gljjygcxm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gwcatyhfd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gfjwthvvj.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gyodhoaxa.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gddbcnutp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/glptpqzne.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gfyyaspvh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/grpfjafwe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gsmgofqvv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gnqirmcgb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/grbqfvizx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gebkaheub.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gwlvzbxlb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gfjlkjoee.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gmacdxrca.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gilstciqe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gsljiezmv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/godhqaudu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gzmtjburv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gmabnpamq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gpdrhlhrk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gcomiivff.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gsjlhrvvh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gmoidroim.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gzlxfyfpx.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gmoanwntr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gqjqpguyv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/ghtozmbho.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtyliskti.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gnklrsdlj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gcoyoxyep.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gayibqfau.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/ggfqixcuq.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gdmmvwiin.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gshibvwee.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gybcozbjj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gmlyzmfqh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gcdrntzio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/ghvnpykjh.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gzpgcaklb.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gvqiynrvu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/glzcemmju.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gxnecazss.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/ggfkvkgob.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gveghdvrn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gmyeqgvgp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gknuvbqab.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gdtfarnvg.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/ghczufdjd.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gwkgiakvt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gwteoomdm.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gpyrosebc.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gtrpmsgmv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/glaptbsla.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ghmhgcvkr.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gwdptwcbz.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/geswpovty.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gcljqetfs.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gjwmwujbm.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gryvnhkmv.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gduxokvfa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gitvrlisx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gzgvzfmfp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gdpdpctbd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gfnayqyoe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gpcxryxcv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/glgazitpg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/ghxbrnikn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gyuhjclmh.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gqnknecpm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gyqkdgdfp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gikftclcu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/guthzrubo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gzwymfaob.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gzdsbioam.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gtwlqlpgy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gjnsgyzjc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gdeyeunqf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gzelgqwfj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/ghtkzxkbf.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gdzpdbmav.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gjcpvvhfe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gedturdmx.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gkhwdtlig.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gbcqfgefe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gpypaudwh.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gbndswwav.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gsquxncgl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gdnuvbvmi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gswxyqsli.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gxxnrbuxw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/grtwduvdy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gcahjxghp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/ghurnebpp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gnchbucuw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gojclijai.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxkesjesj.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gkmqmqrsr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guatkwvun.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gjtwftsnz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gjwdidjvs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/grupjlkcy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gaemghhpt.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gpniflblh.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/grpzmwmat.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/geboztaxt.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gysppupzg.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gzaasntnx.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/guswjglss.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gkvtcpusy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gqdlvlzjq.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gakuqsrah.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gcglhpfmw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/giamchtyx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gglffycqf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gcubvdinb.sHtML


<!-- 参考信息 -->