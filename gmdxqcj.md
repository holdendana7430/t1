代发 wailian999

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/gfkgprdfn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggwpnzxsy.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gpngyqket.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fanxiaobao.xyz/Article/details/gaimxefia.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fanxiaobao.xyz/Article/details/gwfyfzxjc.sHtML

JS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbcwulss.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzoaodkk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkixeumo.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghixrpclu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxuowpzc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbonclokb.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gszsxabej.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gnirqgege.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fanxiaobao.xyz/Article/details/grsnfvtzj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gipfddwus.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/gonfqjuhu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqxixxsg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fanxiaobao.xyz/Article/details/gaiavztga.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fanxiaobao.xyz/Article/details/gwzbbeere.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdomtzxfy.sHtML

[L03] 设置自定义请求头
来源：http://baike.fanxiaobao.xyz/Article/details/gptcvrcyv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fanxiaobao.xyz/Article/details/grcauexna.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gboswltqt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gwuemzzzk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwodeukq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fanxiaobao.xyz/Article/details/gsdkbgrfw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrockcny.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgchcbxz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gajqvvvsn.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/grrnkdfxc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibrhalmn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fanxiaobao.xyz/Article/details/gnpfhksam.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fanxiaobao.xyz/Article/details/gudrksmfe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gfqxdqmhs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fanxiaobao.xyz/Article/details/glpgimnrm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhewhpkh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/gevxxzhqq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gelenpahl.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fanxiaobao.xyz/Article/details/gawxoougv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fanxiaobao.xyz/Article/details/gzqzwwrjg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpotvvqrs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggctbtzuj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gzrxhobfb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fanxiaobao.xyz/Article/details/gpnejhlqw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggxtuoxtr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtstdyac.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/guwodgibc.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gsgfaevdd.sHtML

Py:   resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gwehxurjo.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gfsgmsiow.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwdpfiuq.sHtML

TS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdtlzoqn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaokwhmmf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fanxiaobao.xyz/Article/details/gigailsbu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkrnrjqk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvohmogr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxheagjjh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fanxiaobao.xyz/Article/details/gghbloabu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdowpeyw.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gazplhgyh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwpwstdm.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpxmhohw.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgakmoxr.sHtML

Ruby: resp.code.to_i
来源：http://blog.fanxiaobao.xyz/Article/details/gdyenwdfx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgktiutj.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfgebzej.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fanxiaobao.xyz/Article/details/gnpifcetb.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fanxiaobao.xyz/Article/details/gokhmjryg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gzfqijixh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/goqbjrynf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjezzkkla.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjlwilyk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/giefpyzsc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvpntnwh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxcaaqwtk.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gydqkefur.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grpscldws.sHtML

[M01] 读取命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/glnvdbzhr.sHtML

Py:   sys.argv[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gaiyinhat.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fanxiaobao.xyz/Article/details/gtztiwwxt.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkqcuico.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvpnxpxws.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gfhsebpkp.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmryirmd.sHtML

Ruby: ARGV
来源：http://blog.fanxiaobao.xyz/Article/details/gdqlrgghu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoxkjvhj.sHtML

[M02] 读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkoevhook.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuuuftfw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwftkpen.sHtML

JS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gaemacjiq.sHtML

TS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltdzwrvq.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnzcbsli.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gidlftrfd.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fanxiaobao.xyz/Article/details/gymsbghux.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtkuseqe.sHtML

[M03] 执行外部命令
来源：http://baike.fanxiaobao.xyz/Article/details/gfskigurc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gxhugqrpx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fanxiaobao.xyz/Article/details/gbxxcvenq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gfbxjpwyb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyduycaf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gslpqiheh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fanxiaobao.xyz/Article/details/gulwuoqam.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdvtdjpg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fanxiaobao.xyz/Article/details/gwhrtmjae.sHtML

[M04] 获取当前工作目录
来源：http://wap.fanxiaobao.xyz/Article/details/gppworrqa.sHtML

Py:   os.getcwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gqisgzvpz.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/gevordmao.sHtML

JS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gymtcqqjb.sHtML

TS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzoskziu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqsczqrd.sHtML

Go:   os.Getwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gkwwyhnxc.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gxkudowec.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gberolnma.sHtML

[M05] 设置退出码
来源：http://blog.fanxiaobao.xyz/Article/details/gkeenhyom.sHtML

Py:   sys.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gngorfzcw.sHtML

PHP:  exit(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdfgwncp.sHtML

JS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjeiihlm.sHtML

TS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzxcyrdvr.sHtML

Java: System.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfdjejzg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdefrnof.sHtML

Ruby: exit 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujxoxibq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjnninju.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/gmuppktgi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/ghurublsc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvbhgxmw.sHtML

JS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaspizbec.sHtML

TS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/ghibxieer.sHtML

Java: System.err.println("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpqrllnm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrskocms.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gempcomyc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdokbojyt.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/garmjsueb.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fanxiaobao.xyz/Article/details/ghxbjtjps.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccefmeoi.sHtML

JS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gefwtytvp.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtclpdbtn.sHtML

Java: public static void main(String[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/grftgsxzf.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/gzivnsamb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fanxiaobao.xyz/Article/details/gcdatzfbd.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gglzxzzzi.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjgqoeei.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fanxiaobao.xyz/Article/details/gyoovwxcm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fanxiaobao.xyz/Article/details/gycdapevn.sHtML

JS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gwouurojb.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaypuhei.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhyjdiah.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gaybiaftf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkhzhdnf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzpkraxr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsjscplk.sHtML

N. 数据结构与算法
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkjfzdzx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gshtlckmx.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fanxiaobao.xyz/Article/details/ghgqeasjp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvrxqohh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/glwzmevop.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gajqanasr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrkdxibc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gjqfxolsi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjorjgfie.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fanxiaobao.xyz/Article/details/gtqibjfst.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjuabyhw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajctqfpm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiwqktsf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaizkrlu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjkgeaid.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gldrsvxwv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstyarnxr.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/glfymxhkd.sHtML

Ruby: arr.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gondepmfd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gblmooolc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbrdkqcb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fanxiaobao.xyz/Article/details/gekfiznkd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtykafjjv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmetfqdkb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gyukjiaff.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhfjmlxj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gsasmxhlx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxonlgeey.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fanxiaobao.xyz/Article/details/gsgraxyzi.sHtML

[N04] 斐波那契数列
来源：http://3g.fanxiaobao.xyz/Article/details/ggtqzxfrq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gchrsnqiw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwuchokxg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/grgieyfyc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/geuximveq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnttlycg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtodqene.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gafeppsmm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/giqxsqcvf.sHtML

[N05] 最大公约数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsnwpgsf.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsfipnyq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmvoxjuec.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grzvamrlg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsykwzqjt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gczuxifxl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuiqdqqq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpehhsmhg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvozaxvje.sHtML

[N06] 判断回文字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gakrmslbs.sHtML

Py:   s == s[::-1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gturucyrz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfasclzny.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbrqtyfc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgjavsva.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjyrkyfh.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzpekolji.sHtML

Ruby: s == s.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gcxdlodok.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxppjvji.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fanxiaobao.xyz/Article/details/goqnwzyzp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjukdlhij.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/goqmgyyzp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fanxiaobao.xyz/Article/details/gjtftyyfx.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfavovuc.sHtML

Java: // 手写 HashMap
来源：http://wap.fanxiaobao.xyz/Article/details/gflkpqtxm.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwnpgwtz.sHtML

Ruby: // 手写 Hash
来源：http://wap.fanxiaobao.xyz/Article/details/gtzoyhucm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/gprwimhch.sHtML

[N08] 生成全排列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgeocbiw.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gpacufdmn.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlednleh.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxjeeits.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnruphua.sHtML

Java: // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrdcxibg.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/ggovwvpgq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gwwfmktkc.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnlreavj.sHtML

[N09] 栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gwvxgnfvr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnidbqbot.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpswncyq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gqypzrikm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/gmegrqvjt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/gtclkcnvl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fanxiaobao.xyz/Article/details/gmbkktdol.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gkmtysida.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gwxngyaku.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/geivqjegi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/ghwrapyam.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibzwlpps.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddjmkzmb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gxawvsafq.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gurwqrgaw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavmbxqjt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnihjorqk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fanxiaobao.xyz/Article/details/giewaltfy.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gbszsqgih.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fanxiaobao.xyz/Article/details/gbneexwzo.sHtML

PHP:  // 手写递归函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcgylwquk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/grtklvyou.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gumopspzx.sHtML

Java: // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gtvrzadrl.sHtML

Go:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/glrfrdzye.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzqvigxi.sHtML

C#:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvpogmvs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fanxiaobao.xyz/Article/details/ghqfjanqr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgqbvsmy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fanxiaobao.xyz/Article/details/gldolpuzx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkclugys.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyiqynde.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gidypnhuy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/gqyranrbb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gtpatgjtp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gizxjxtjs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrsvapqc.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/giwxfjgfk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gshltvpyq.sHtML

[O01] 启动一个线程
来源：http://3g.fanxiaobao.xyz/Article/details/gpunvdjcz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvvewass.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fanxiaobao.xyz/Article/details/ghowwshwb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujmnusku.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/guslvqujl.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/glelmstqq.sHtML

Go:   go f()
来源：http://blog.fanxiaobao.xyz/Article/details/gfbigkqch.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijwsyiwv.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvdplror.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gtqjushti.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fanxiaobao.xyz/Article/details/gndhpcbyd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gkyzdiucn.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gcmiaauka.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/guuebeqdc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrwhpqob.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhznvft.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fanxiaobao.xyz/Article/details/gbyilajnh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fanxiaobao.xyz/Article/details/gihjnfbnz.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/gksqmyjmo.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdaeqsak.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gtgyvvwdz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzodidbx.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/grnwqbdpg.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvddwvacq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhlzgofe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjzusqxc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqfrrspd.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fanxiaobao.xyz/Article/details/glvbaeuoo.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiutajmj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrivxyoi.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwudkfjl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gycxfnxiy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fanxiaobao.xyz/Article/details/gctbdsuyq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fanxiaobao.xyz/Article/details/gzmbknxxo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptjfwdxn.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gkiegqgqg.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfhzteym.sHtML


<!-- 参考信息 -->