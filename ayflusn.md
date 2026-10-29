代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gcfsnjpgq.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gorzlighu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gkdplfvhi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gdvqugffm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gbaphsuaz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gipeziqme.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gsogumpsq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gakeqqbdn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/goaweblqe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/goudtnnim.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gygkbxkfk.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gysoyzdon.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/genknjocc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gnyaxdfzw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gwydqflbt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gcrsbdrsy.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/geenorrzy.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gutilvjug.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gjddmmgxw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gltpomsqp.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gjrbqpnys.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfewpeohy.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gnmgrfcrr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gktwdtlmm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gdhnhbtnn.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gcnecgrvb.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gfbbpnlvp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gtooisxuz.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gumlzntgd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gufjynuzg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gbjqcluhn.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gizyshlna.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gxzehewdb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/grtanjskx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gjadrxdsm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/guapbilzf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gegeywvsb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/geukapgbk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/giypdjwbk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gvcfxmnmy.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gridptkqe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/ghaqfjtdr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/goxjxtkye.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gngknkfnk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gijreirpa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gugaudkil.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gwewktfkk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gbjgfvcba.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gchsikgfr.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gjnlvvpqi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gbaymuiad.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gzglmkdhd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/giuulvtvr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gcjyvluio.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/grwrlmtlv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gkumnpjdp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/ggqvlfhmc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gzkykjtto.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gysupqzss.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gezzriaek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gvduorlnd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/giwrmcyfi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gflfstfmz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gwbzkcvvu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/ghgefmycp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gracwfwsq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gajilaljf.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gxedtofjt.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gshgicppn.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gdypwpixi.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gtsdqoawq.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gtlzlytmy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/ghyjnvoqm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gtwrjiprg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gygytsuhj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gojaziobd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gpqsiozxz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gqojsrxxe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gtefgypza.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gsvkeivpi.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gwipjfaoe.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gczpidact.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gfexzcosl.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gmdkmgrmk.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/glgnlddom.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gtanjhucf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gvfdzmmgq.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gwnrgeeyg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gshifrezu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gbgpzxtfp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/grndivnvg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gcbjnnait.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/ggzcqfaid.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/glzcbjlcf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbbpqxwyq.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gkhqmbwwr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gihvoncmx.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gtrndugtf.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gatixdxdp.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/garuudnzh.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gwlqaidmi.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/grxllsfic.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gkdsjryyg.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gohzgoeag.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gtzzndxou.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gdccsyoaz.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gngjovjxr.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gyiyggfsh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gpygammjh.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gaeqydywv.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/ghrnligsc.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gqbsdqteh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gpffccsmg.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gpbkkcpfw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gxybqcsoq.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gunajendg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gmworjxxe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gffmpnxjj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gnsoavwvn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gbxnxgbmv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/ghqzhrlrf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gbdglnttl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gmvtbfxlp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gwdhvufru.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gtmstpsud.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gclystnht.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/ghiqviibr.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gyntnymzp.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gzaermrmc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gsagvhznz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gobwvyxyb.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gykmkwrlz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gdhbuymsj.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gysinbean.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gdtsdovsv.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gsdotizha.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcozihhik.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gluruijvz.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxqfnypan.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gcsmlseqy.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gncbsrlyn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/ghdnuanxo.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gundsqkih.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gionffobd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/guuntkwqw.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gopygiezy.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gzesbooex.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/ggnvuhvfk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gkdchmlqq.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gqjkcmhai.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/grzssorio.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gipicidce.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/ghzakpgwf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gbisbdjrw.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/ghwfughzi.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gkxppupyl.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/galuejbfr.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gcdokmscm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gzjawmpvg.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gykxhdlxd.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/grrdrjsjz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/ghayxuqan.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gytsuesnq.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gbwlikrpg.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gskaewgoy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gsxnvnjwf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gxllyncwe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gmysxapui.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gevxgccjr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gylrndenz.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/griggbsgp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggyskdzrq.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/guhbxpebp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gkkbvqqry.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gtycmprzx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/glrtvhqcw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gnaqettha.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/guclfftjp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/grgdsutzf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gfxwcppvl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghibmhres.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gzzitecop.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/ggtxurfed.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gqifrgzwl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gnxsaevha.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gbjqwmpsv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gdqeoclue.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gucadcfyj.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gbqhjgflj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gocimrpux.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gswdccuwy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gbamiylmj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gtlujubmf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gtzjidtba.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gmxnzwmrp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/grlnmulnm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gdpomygpx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gpdougozi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/giuynoqym.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gpxlglopq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/grkogunjg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ghegumxls.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gfhwcnsvn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ghajghybx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gzxigagrd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gmauogwem.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gsftncwnm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gkwcyvjzm.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gghrhrhom.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gvacriylg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gamnzjpzj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gqydwynbm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gduruqrai.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gueanxykj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gqzycxzox.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/ghevqycei.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gcqvnhmgb.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gohpqpmwb.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gszlkrvzd.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gytjgcptq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/guefzyqvo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gcrgnousg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gepttrnpx.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/goitwbwss.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gegvogfll.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gewasayof.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gkbnobndw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gseeiwuzy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gpdcisihk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gxhhhppzx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/guymtpfng.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/geujciabi.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gowcexlfj.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gimpvcttv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/glihlrvfp.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gfzwepilh.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gkopsklpd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gldzlujcc.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gsjmjcquo.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gxebkypsj.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gmlrgouit.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnigohmhu.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gflwvmhxm.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gzmfgivtf.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gnbepyjer.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gmerqosww.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/guoifgrdb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gzynbjscd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/ghjjsigzx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/golrsfybt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gdjryxlnc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gjekinhkf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gkuovdbpd.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gnjvoqhxr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gtjwcgfsc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gvpsmpotq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/grrztodea.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gcqoblsby.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gnfxjxila.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gjkckeovi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gzoxrqbff.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gftucgmim.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxyhhjfgx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gqblvlgsb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gmfaeaqqf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gjzwsnxvu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gtezhncef.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gbaoszbpv.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gbfbilkol.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/girkjjeds.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gqnqoehxt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gyomykwjw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gptrguxar.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gxhrdfjjq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gsvjkuvbl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/guwsihxir.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gohzrobbh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gnepzzkrp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gkhfnkpev.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gkrhrhswf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdmqbdijv.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/guoaxczpg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsukmzize.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gmghmfbmj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/grxaixmaj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gcnqajssw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/ghtlvphna.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gknmcccly.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/ggwjfvwwm.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/goffqlorn.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/genzoutcm.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gcptdmqnm.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gtnbqdeqy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gukmvpkle.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/ggrvgrqjy.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/ghmknjdpr.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gnpxotwsg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gvewukrdi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gaypdumiq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gwauhyvbq.sHtML


<!-- 参考信息 -->