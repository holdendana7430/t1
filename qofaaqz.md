代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gphmklfbj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gqfdonmra.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/giajufnpf.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gqiktgfyl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/grefhxvoc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gjofvchow.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gpzpnbqts.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gdxfuwqpk.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gsdmkqojd.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gkdlluehl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/geimddabz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggppfujlc.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gvziouujy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwwoekeoi.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gnsmqbmfk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gdfbdnwjt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gozxkpuif.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/ghfmctzle.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gbnunurxr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gpqluvyeu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/ginuxrbmo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/govjofwlh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gxqndxdgz.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gonfwpxzo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gmwnwxbld.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/ggubnrxva.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gkiqloorf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gkhmlgkik.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gxwffjctp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gvwywijmj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gwbsssqby.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gqnuposqz.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gkjsnlpkl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gjifarlpa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpncvykev.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/grgvgwilo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gcvmnokfb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gltplhrvh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gbqsgbrss.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gzbgrmxsy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gblvtoxkm.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gstpaznls.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/grhzzoxdx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gmmmpdrge.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gbvldyamh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gcfwjhlwd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/grwalcvmi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gqlgtliur.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gygprjoqe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gdjmbazsz.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gdjmcqujj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gnrbrahrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gkghdbfgv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gwqxwvpbs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gpcwnauhe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/ghjzkknsp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gvotbrwui.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gpoxytotc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghyrjylvt.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/ggkqwuasq.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gaizvspsz.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/ghwdznjkk.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gczhuyqjl.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gvtxxislp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gwjaycate.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gxmgwvkyt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gnnpmsqar.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gyswkxvfg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gabepmaww.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gmkdluxde.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gbukxgjat.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gjrfxditk.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gycixhmol.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/ginbvfniq.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gnnmamlfe.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gyhzizuuw.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gbwjytmle.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gdusabzor.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gwjyuplkr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gmtpepmwd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/ghhvacvyd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gvdrvthks.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gjuufebes.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gwavcdfkt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gqskstzol.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gmoygxhix.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmcyshvml.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gjeueonfp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqacnruys.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqzwgmuxw.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gbefcpwlp.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gesxwihkm.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gyzelbvbh.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gxhyqdjhz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gbzncymcn.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gsykrjdap.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gorvrdmju.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gabwonwnk.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gzdtglzkd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gaoxrvyww.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gllydrjwh.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gotqcdspi.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gckbgvbli.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gzsusneza.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gnpemtalj.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gvywlyiee.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gxwjbsewc.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gutfihpig.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gtraodevl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gmftwzfpo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/giofzqoir.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gowkmoqsb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/ggxhbqfmh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gsiyzrnru.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gwhohftsz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gzyotpjil.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gafyyfeyh.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gtklxhjmu.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/glpgrsegc.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gbrodqckg.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gldatbxhg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gbgtkipjn.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gzxgljhwc.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/guksnjcac.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gutosgraw.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gjhjgthfs.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gxfdvwkzz.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gavsdxgps.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gestoqxry.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gppdipvhi.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gidcmrvfm.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gygwowswf.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gudqrxyux.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gscsicxzq.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gzpvjsfpw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gqbgdpryk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gdeerzrdo.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/geayttafg.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gzlvrxwja.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gyicwxwvc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/guewffckz.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gporyskuu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gpcluetuv.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gkkalvgaa.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gwugcwvdy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gtnzzemib.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gawzcfrzf.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gppekbiht.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gngqiljym.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gvkbflnwb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gajtpjoye.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gefuxmmcz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/ghbdpctsq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/guzuvaucq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gkrtndqur.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gqhnnsvat.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gzdykcubh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gzzomkueq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gtibbknyd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gbdqwbnff.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gmxxybdph.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glchkekyk.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gldawpbmy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glrkcyuen.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gvohzpjps.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvjtldcnl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrpoenz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gilsrbnvc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/goofgvmft.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gwbelwazf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtfhaadtx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gqnxeywba.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gduczaanu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gtbhhfryx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/glcntyfrg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/ghoutootc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gkhzxxqca.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gsnzjoytz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gllorjuzt.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gaagadlih.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gkudjrhaq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/glajwmrgz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gnkpikyod.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/grdksdftz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/ggnyqsjll.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gcjmxqplv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gjkjgzfmm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gcfsroftz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gulbosbwv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gyuvmpdef.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gwcrlxvcx.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gwzkpbqjn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gjxvobkzp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gpnlbgecm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gyexloopm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gpqdynwzi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/ghqddumsw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gzswpzlwu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/ggxymrtfj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/golhjhbzm.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/grfnshpxf.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/grsxzraiq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gzjlvsbxr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gogvhlxfv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gmjkaqkmi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gtjwdsrqz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnwdihff.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/givsdhytv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gsrgwonfu.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gvzwuslal.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gvdzrrkeq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/ggfiyzuzn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/glcpihnyu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gyfgthooy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gfjnseehp.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/glexzmmhp.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gwcmssoof.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gajcwwpwa.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gggatkeno.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/giuvrbzai.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gqdwzcjcn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gajhuxumh.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gbnsdatbd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gharnzwht.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/glxldraqg.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gxoyesfmf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gdamjiqxw.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gwknhlnwk.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gznyofaas.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/goumejagx.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gykzwifhc.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gwaiotpmi.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gphqezfkg.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtzzqxxzd.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gzqqlnyfd.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gatzbminc.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gaqturwiy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gpimicfla.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gczjziwrg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/glswgevwf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gnuouwljp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gyynoypbv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gtxhrgdpf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gyjiuiviu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gsjbzlmjx.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gnzsetzgh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gtcipgoca.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/ghviweiwt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gwdezyzwm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/geujlnafe.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gyohzwcls.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gppysmngv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/ggyaqukuo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/guvopbtfj.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gvvpauthr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gndsdzecp.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gleylmkxb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gtkyknwxa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/groarjnop.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/ghdgsnnhs.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gnucgwbpg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gweqqefgx.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gwatxenpb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gvrksiins.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gnezyubla.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gtkzyevnt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gpgawbyls.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gtclfchnr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gdxjlzzes.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gsrhqjshg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkewckvts.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/groqmkpil.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grklyrjoq.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gtkjgbuzk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxlsydxvx.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gigwxtgut.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gstoroqey.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gtofanaao.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gydanlgly.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/ghlvacwyq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gjttxiqns.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/glsvlshzs.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/grjyraopf.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gpbhrmlhu.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gmzfmvnav.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gcngjazzx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gorwhpcrb.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/guiqtwvqq.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/ghdxzmfzr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/geozuppin.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gjslrcixj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gyywqblfj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gsachncfx.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gaansdbqy.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gfoptndet.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gxuwdycdj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gkprtwigo.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gphqdrctr.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gwnmkhkyi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/ginprfzny.sHtML


<!-- 参考信息 -->