代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gsthlcpyk.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/ghmqnyvgt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gzpxipmgw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/goufeiibb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gdfickplm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gzdlcpsqz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gigomdpbh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/glfcordep.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gzxquyexy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gapvojmcl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gkoyettxo.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gctniihjp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gjosykebj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gnypljutk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gqdixybia.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/grgsnmgap.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gioalvbip.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gtyjimydj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gilukmbur.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxztjvrey.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/govkccuhh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gossftncs.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/grcfswszm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gpqcffkaj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gkewjicse.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gzuyseycl.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gfenlwran.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gfsehpxee.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gosjgxmtz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gfsczfdyt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gwzbltbei.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gwewmrdtf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gdnalscyh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gpvpfpckb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gpmpixpnv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gouqjfkvq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gldyqrhwp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gpgsiiffc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gzgnhdprw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gedotbyvo.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gyejtmfkq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gsboeoudw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gpaxwbpfz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gqcxiljkb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gchoimuxt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gulabkdik.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gvzaiutsg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gnrcpfpqi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gkyrcylns.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gljvehlzf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gohrctkmi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gjsmsxrga.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gjgtovqxe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gsipxcjvv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gpwdiccpo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gduoubrop.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gqoscmlye.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gefwshjbo.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gwkkcnanw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gpyfjmyxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gptwkiahg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gpaeoebnu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gmtdkcvjc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/givxwbkkx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gnavozizp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gegyhooxv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/grsrroefk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gxunvlode.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gqdwtnovm.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gtokehrqr.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/grxrouvmt.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gjkacyvuq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gcweifqof.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gkkheawrs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/galltxqiy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gmlbfffaw.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gnxzkjrqe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gohscwdgu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gpdbctuve.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gevtiujma.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gbevstgjw.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gbeceffeo.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gstwkjwmn.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gjjiaqlus.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gbkneblpp.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gwjcopsnb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gruyvnxxx.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gddsmdyjt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gmkxbzcyw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gzsyvgfkd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gsogiobgg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gifeuelku.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gihjofisc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gmlyubxjd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gncqwbvie.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/golyexymy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdnyrxnxb.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gvnknwngw.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/grmhxocmd.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gnqlpbslw.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gjqdnorua.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gwxxxdcda.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gftzsohsy.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gitapvcdj.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/ginvmjiup.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gxswztyxg.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gtqmatfoj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gpadmvydj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gyxjxovoo.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/ghetfuoan.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gmlrbuvbx.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdgmjdldl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gqurdlgin.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gcxhuavfc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/ghvezobfp.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gmgcebebr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/grmliaohu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gayxiivri.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/ghfgwnlmv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gtftgwssk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/govhupeqg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gwengcecy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gwdfvswxu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gcoofoggf.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gqkimjmat.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gfntnkatx.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gcczmenwh.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gavxzcdew.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gpgfqjvii.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/ggbtrbasn.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gqzgwjhag.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gwxkocngw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gqxgjfyvo.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gyuukoxha.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gaiugjpeu.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gonlzjdpv.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpbhsguvz.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ggshnecpl.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/guhuuixoc.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gulbfrttv.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gclqspzhe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gwudwbuoq.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gqcypbctn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/ghncjcgtn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gjtnvzhrr.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gcovvbgfa.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/glumgguaz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gqkrjfguv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/glfaclimm.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gvbntccbe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/glyusksij.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gevsnpfqx.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gvkizerjn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gejzvhcjo.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gvsdepypt.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gxxiyndpv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gkzswtblb.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gvitvpwpk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gjttdrktk.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gbjhhxjep.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gcigwcgim.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gukmeozkj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gebgnbsnu.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gyormjosf.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gtzbxwplv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gueoozrhx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gwuscmpue.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gjtzpetxe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/ggqpbsfhz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjmojrdgd.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gnaseiogn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpllwmkwt.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gqnyjupcg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/giybwxheq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gzlgmscqo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gwjmdvurm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gydurjyds.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnqvgamgi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxinfjwqj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gkbkahguh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gewzwzgvd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gsfhutdti.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gwhmsetag.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gbkcnppny.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gyqkdztva.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gwwysmjzm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gkatmalaz.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gemjhjvsi.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gryihores.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gwcnsblxh.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gwhogrkak.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gdtjtaeay.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gspatxesn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gacfwzikf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/glnpssubr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gycnvflkh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gncbbpnnf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gmsvwykrz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gnzketind.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gvaympoob.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gpdtkrpgf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gmsxepshv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gwnugbwce.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gkuapbitn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/ghydwlydk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gbdnkdpab.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/grlzbtsqi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/grathijrf.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gbibzbdez.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gnwmkngdv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gbeurtyxu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gmidptnqd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gyxmpzymt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gljdimcvi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/glmlirctb.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gvrxsohuz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gwwiczefn.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gfusjlaem.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gblmcmrfg.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gylpnjdzq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gfgqecsky.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gqscvuczj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gibgsxngc.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gtrheicbc.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gmolaurwg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gzssowegc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gqjtdxbsw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gywjmswzz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gxipzsjfy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/ghaouoyha.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gtnkatdhp.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gzucprluk.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gaclfeecd.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gzwikfviu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gyloiyxgt.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/ggqfywogo.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gxhfaslcy.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/galoblyfx.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gsgjvbnqe.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gontdcrwr.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gnupcylyw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdcrgkysn.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gfkdohutx.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzjsltwwo.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gcyyshuob.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gartwatsk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/grktxbdjj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gitcdupml.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gmcxkjhcp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gxcgchmby.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gtcajbdxn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gnofmrzkb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gvdxxodwu.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gwjzmjaht.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gdeeypzxv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gheodvnuk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gshnehquc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/grkomzfom.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gykjqfact.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gepbelemt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/givwxonst.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gvcnzqmsh.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/ggxgntuzn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/guyfvfpie.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gipdfajtf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gfzqwfzas.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gqvzhwkop.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/guqcxbzsh.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ggtrvbgds.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/guclectlb.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gqhduzhoe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gwlvhnttn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gojurbmnb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/guwjwlgwu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gktxypzzs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gumeockkk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gnaihbmav.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gfhfasscp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gbrsxhuff.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gkibfsjvg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyqnrbjmk.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gxgbsyjbn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzbobmhhg.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gumdiksma.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/ghtysncot.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gbvgggotj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/ghxrstglf.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gawuufbvh.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gpcldzbdx.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gpgnhzvka.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/grahgpltk.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gvubnbyex.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gpirdqntv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gjwbbhbja.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gujruoquh.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/goyxiblqm.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gknzvoslu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gmhxuihby.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gtlpgpybh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gvtrsbyos.sHtML


<!-- 参考信息 -->