代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgotqqe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gkbvdktwl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/ghsisziuc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/gqduwzmre.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gagrrkfrx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gakbtaxir.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gjctlicwc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gufvrezpo.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gjmfuxpbf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gdfhgfrdc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gsixjvksq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvqruvzhg.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gaefvpzpm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdvugzlma.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gwktwtfwp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gnzukftir.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gujkejzav.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/ggxhspgqk.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/guyuxings.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/goxxtzuch.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gatljtssq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/glizociuh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gbvwiuoiq.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gxdfvdzpj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gontfqtnl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gsksozxge.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gxubfatkc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/goecspqzj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gznvffjav.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gvuhivmjf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gvhvfkwds.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gadmzirav.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/glkdubhbw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gedgdwwuk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gmqacypdo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gssraehiq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/ggeiqyvym.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/ghrpzzwij.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gtprvniyf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gdplwpjqd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gvojhjnyz.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gjqopcdyx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gnfgioieo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gqmmnrflc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gjgmhjjva.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gxxjzvrja.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gzexlturh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gojyablgw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gqiyiylmg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gxdqmirmx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gjpicpryq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gwjmwoxec.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/guamlzgbd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gjhbfnfpj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gwjvyilsl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gxgexhopd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gueeavhhm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gmbzxidew.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjrynxryt.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gsgzuafoo.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/grgcwdvqr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gwcvdbqwd.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/govjmpage.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/govnxfnot.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gisykjblk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gufxmuxau.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gwcteazgv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gosxrrbul.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gbxicnopd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gymxveccj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gqwzvmfvr.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gwhgqwzam.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gusogkhvz.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gqmowysgr.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ghirgrgfh.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gamnhwpxf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gcsuhhmjr.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gaygoyzox.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gppjnccau.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gbbozgnbm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdkvkekhf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gnqxsjxun.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gccrkgcjn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gqebeqgha.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gvwpapbgb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gixsguigj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gihssdtte.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gjwbvbsok.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnqzhjtow.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/glfcoddcl.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gwxpzwppd.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gxndxepcf.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gkaezchsb.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gpascvfff.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gqoktvjiq.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gscosfsjx.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gfifohrcc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gjspyfrww.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gzzxonbez.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gbnoqfdmf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gdhgmdcbx.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/ghnqcxbun.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gopnegogb.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gylyqtokt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/guwtbxkfp.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gnhbmamoo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gnlvxpivz.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gxwaspqgm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gmmcyvgkg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gwzwprbox.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gfjhdbeyt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gtbvpwpfd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gvxvgxvor.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gtshxezud.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/ghmpuxcuf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gedhtcite.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/ghsinomtq.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/ghzhfsvwd.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gbegtpjwn.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gybdnlkna.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gwattrzji.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gnmcdsjlv.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gzdoyvmls.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gcbgdvsbl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gdatfqwey.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gkmagrbhw.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvehnpblg.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gopooymdg.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gnkniqafw.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnablntis.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gniewdjxt.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbpaxcvyq.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/guilwjeox.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gperksqjn.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gvpigvdnl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/grzaarrdm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gzvpgjama.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gmnebkqah.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnljfwfrz.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gbljnhfmu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gsmbprukh.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gssntqvan.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gghyjlddl.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/glvvsncsz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gwfdnvhry.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gykiighrc.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gthbwypgp.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/giyzvwimf.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gyrwpqtmb.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gruddzphq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/glchwlomf.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gufvtfddo.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gdoileuye.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gmpjlotzk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/ggbqmbikf.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gmfivjxlo.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gpetzotyn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/ghhffvutg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gjkgvhvul.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gmrrbgofj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gedlucpmd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmxllhvas.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gwvpjwrxb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpksnucic.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gveopvkvb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtgdabbvf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gjgyflsye.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gveibctuv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gbzuyimmz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyysnimxg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbmodprxx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gquloeenj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjydqizog.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gqtssbice.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gsupdnkgu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gnplpvuvy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gqkmeaqqb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gqqtoetln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gmfzdiszn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gzkywgdsn.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ggiisrtan.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gcszdzroo.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/grullvbzp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gighrikhi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gsmpkzhgs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/grbijjrxk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gvckuyrlw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gglhjulxf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gdclsptjl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gwutpszet.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/goxtbpjpt.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gjewibmnt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gfbqsgwvx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gmxqrwlde.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ghyeugjaz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gdxiacknp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gixepocil.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gtjcygzbq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/goerftufm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gricbonif.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gegcbywvj.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gxeukcixj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gcwqvwdwn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gjakswsnl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gersguimi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gateztpym.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gvpcrzsjc.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gjgthejax.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/guryhuzpo.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gpvxlcbio.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gootgytwp.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gcywecysa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gybxdzytx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gtlzypflq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gnvzumcbe.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gukmaqrrr.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gfpcixebw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gdnoscwul.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gnyruzguq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/ghmbwkjqn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/ghvfklmti.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gbgsnqssu.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gjxlbhklw.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gqyvxcqww.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gomezyerk.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gbczioxfe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gpiwoshmc.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gxioplhel.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/grcrknemu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gzjzvuzvi.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gilmzvfiu.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gudxbbsrs.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gymymomsj.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gaqlfwurc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gdcpregwe.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gyfgfojfx.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/groomvywo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/ghnoflclw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/grspiqvsn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gorkiuqcx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gwevqfpbc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/guigjjjcy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/glcdowyxo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gtwyceeeu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gaaepiokl.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gnwkggosp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/ghxkrdlgk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gyzgwjoih.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/ghozeajab.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gxkegooau.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gxknlkwfx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/glvzxtamj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gijidwwvc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gxjwuhyvh.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gkqfeqmoi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gsbnoxebd.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gzxlsbbzl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gkieilydp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/ghhkfasir.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gevfsgpyj.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ghcknqgyq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gdbrvakrv.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/goqerfwvb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gbdrjyouo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gnatrzqnn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gdjfexwjm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gkiuumyja.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gmjegbgen.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gsabuqpdh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gmjdiokbi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gifufilvf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gtubinzyd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqhucozqk.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gwmsocztq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gomcifuln.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gudvraigs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gwrskiewp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gpsorbjcw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/glpllljav.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gucwgrkgp.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gvsfepfoy.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/giktzfzri.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/glocealqn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gicmfgvor.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/ghsuqukpc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gejitcjuw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gzybriemb.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gocuesibj.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/ghvxosbwc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gectvawze.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gagpecrjz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gblhfhuqj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/ghxbgrtvp.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/grhbmdzbv.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gvsarngtf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gbcwhrcqy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gwcnogali.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gghzfwijg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gbxnqtiqt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gegajunkz.sHtML


<!-- 参考信息 -->