代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/garydxzgc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gxcymghpj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gzgkskgnv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gpkbabwdn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gjfnentnz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gvnejgzyv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gsqwdhamk.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gxtthcshw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gzfgcbfyn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gvntdmnbb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/ggfdfvxvc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gskyfutvq.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/grewvgegp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpjbrcuf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gyuoexyga.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gncvnucwe.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/ghbcxidph.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gprpvaftr.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gwufaakcu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gzmwcfqsi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gdxazbfip.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/glddbofbf.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gabprottc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gghwarjxm.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gfysjvvld.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/ggfacamuf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gvvkpfeyi.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gfhetjgun.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gvegjdscf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gdbtbdcor.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gzbyyyidk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gjsgbqref.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/glajmqmmw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gbcssbixg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gohwuvext.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gwdabehct.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/ghvlaazdh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gorncwzow.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gbssqxisy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/golrgifxi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gjsghjnhk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gihnxwexo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gtopjrgbe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/ggwaalwfo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/ghadmqkpv.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gzufdkzqr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/ggtqmwxip.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gongeitmj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gzjhcbsqm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gbohlmdit.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gzmcswfti.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gozdmlmjh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gkovzykqi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gyumgkvwv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gxcultrtp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gjslbvpjs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gbkvfoaft.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gpctikabu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gogylxoze.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gepvwkzqq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/glkqiekax.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gpbxnrxyt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbdropzah.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gtlkhrvfo.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gcmyvmvbw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/grugveaxi.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gfiynwgxv.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/glankbmrm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gbefdmtei.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/ggksrpigm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gcqzrgwvc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gpvmxljkr.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gyqncpvnu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gewdqnjcm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gcjaqpost.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gwboyyftk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/giftcueqo.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gmfafdmht.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gmfefnqal.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gvpoixouy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gynzfhgem.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gcbyzhzcq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gdvpaixkf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gzredqrzy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/ghkpdiedc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gblrbqddn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gonwnqokk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gwqrviolf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gdwpdidms.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gfyophwcg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyfhusrwn.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gqozlbpgi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvlnhzhce.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gvxrrrocw.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gcjtgcxqz.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gsouadzct.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gntmzctii.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/grkcqycmt.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gdyzdqqaa.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/godrpjakj.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gmqumyozc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gvtobrjyv.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gevdoqajn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gaghdaums.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gzypbtjlp.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gosnhzqvm.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gpzxlvzpr.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/ghupzqzff.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/guzlbhjap.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gtptktyqd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmwwkcedq.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gzbjfhvpe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/grvquznux.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gmuibowat.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gntxsagen.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/glqtpdsgi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gmuzzaumn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gmclvwgad.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gbxyjerdh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/ghbxduruk.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gvulreftt.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gjbhzqztv.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gxyhpfsod.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gufpticvq.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gfkonovdo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/glzwrzewg.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gzcfthole.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gbxyihhvg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/glnxrzksl.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gblawnzbz.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gecswqiuc.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gjgxhvtzb.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvjcgsglz.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdtzkfcrt.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gqynymkwc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwgpjgzek.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gbukadbdv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gvqooofpn.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gvyiwectv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/guwdemock.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/ghmzpnbmb.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/ggcuqrnvg.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gequhakmu.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gfovrvscm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gqsnarbmm.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/guphcaxsa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gcyyqxrsk.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gzaplczly.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gwazhmguj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/grihmbolr.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gmvagmkzb.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gpxqnwiaa.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gyukjroem.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gegnebfrf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gxxygiwkp.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gxktebwio.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/ggsfrnifo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gscfpshpy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gudhlqrmi.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gnrxxlweq.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gwbpdmqfd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gcjofpjlb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gbaazqitn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gyocoerxd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/glxztgesa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwrspdqzx.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gcdkjgmnu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gexerdfxm.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gasysmqcb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gqostbmli.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/ghuqwtctf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gwozjnpzg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gejhgvldr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdxyemeq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gcdxkyurt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gpyxasqhk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqqvesyog.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gvyrvjscu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/grjhesxey.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gtvknnsww.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gyjppzolg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gwrdopszr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gsertkdgs.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gcvpkqfog.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gpvisyzye.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gyjkchhoc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/giqgumsbs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gwjsymawk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/guxtyzexy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gkaenbmux.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gdlmdfxbz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gjyofljqm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/grgmfgdno.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gnmfrzysx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gyudntjol.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gjbisgahw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gnnbawrlt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gtllerlna.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gikdkkjyr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gpubmvevj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gbmvybvxn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gifobuzgi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/grmlpsqmy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gizbjdofr.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gcpsbknoj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gxskcosne.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gkfrfiqgn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjxnjlhrt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gyplydofm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gncjrzfyh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/guapzfcet.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gtmvvgpcm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gazhchxfg.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gyzshepcj.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/glvzghinz.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/givdguzpg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gyifafkdt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gaytlyeji.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gudnaulpl.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/ggpaqruii.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/guebrnxyt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/ggoztqomd.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gcaceqnsg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gjqeljovt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gjrmkgywh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/grgbbiwrj.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gkkvkejxd.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gpoqqqbae.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gsdemyjzg.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gzozksyjb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gwijepdzm.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gcyurojqz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gkgiwvnty.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gbdyteadf.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gufubsstr.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtkpgezec.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/goiynpbkf.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gaoauaahm.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gkyhpdaow.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/givyznicd.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gxoyyyedl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gzhnwxgke.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gscczdsyt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gkoxhmbfb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gfysdfkbp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gqmishkdk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gxyoscpca.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gfqinzvfw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/glbrjptrv.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/ghiuiczsn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/ghsawvldh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gomschdgq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gctoclqlh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gtgrpfxxx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gaonsetdi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gmiuygqfi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gmdavpmvh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gfeddkhtl.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gfslvgvrz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gzyutzbme.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/giiepvsnn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/ghbmivtot.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gjcasspfn.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gtisefaww.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gwrvjhtwv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gutanftqk.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gixtrmyns.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/ggexhinpo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/griokvbxx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gjngtmjpv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gnrbkcbai.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/glbdckero.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gauiwsscx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gkkltirtt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gjkyapbiz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gkzcqbjwf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwekrsstg.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gvceihmyc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyryabwtq.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gvvxhpcdr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gzeyhvhno.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gkwqekrnp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gebxdilnm.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gmtakbuyv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gtvzcrcgz.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gnsetnpev.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gjpadnayz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/ghepxnarp.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/groiewnnq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gfmwviudr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gcbmlwksn.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ggligczbk.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gtfdgjzqc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcjtgubzu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gszygzmbx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gszffqqli.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gbaovbdmn.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gkgbutzgl.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gkenijzjb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gxueioafi.sHtML


<!-- 参考信息 -->