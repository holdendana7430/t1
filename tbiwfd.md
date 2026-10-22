代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qwuggigm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sflkneby.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2edbeagjv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jmpbmxsl.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hudfnysi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2lklsernz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jaxdstgx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jgpayuza.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zeldguff.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2cqnkuvew.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lshocksd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hprhwnor.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wpkcdkkl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xeuvocvj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xouhdsew.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2avlpsktx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pnlvqfcx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zqbcnsps.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xcdwdacs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nfribjtd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xzpuvanc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2cluauezn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tfagvrfj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ljinakbi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bwuiphfm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2aegftorn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jedmwxaf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nmlfeqfg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mhymitdu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cupgvons.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eizwiifl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2agoabqnw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gvjrhekc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2mlsmvflq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2mpjuckhp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2cedfvuwg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hylrfhir.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2navklwiv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fblejqei.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2fxjeremv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2twbcrydu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2dqmrelqb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rxhpfknn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ukjcwzxa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xjvdmgqs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zlvcisxx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xmxjevjq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ruvqrlvm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jtqpewof.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tdckcnzf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2perbpopk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zvrjsuho.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2djonipsg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2enyysbqx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cbltqill.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xtrqdcxy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zwajdact.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gzudjtsv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lvhpcdkt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xuzxmtwn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nyzmlsnf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jhogpfde.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wapwlokt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2dcdepqbe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fxjikpyt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ihepxbgq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bakzzzkx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2agmdqqps.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uqhsbdan.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qgdozcay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzcjitur.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qnlngmtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygdivrsq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lgqgodqm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cqrpuhzj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kyjnldas.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bhzklall.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uogeiapc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fbncxkwd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2kuxxghjg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2feybcjpm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2eltythwm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2adqvlqvx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iqhtvnen.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cnfrgtxa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rxtkgtop.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rizoovgs.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wgifgauf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vsnhpnra.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2dkyugyku.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jtawkmqu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zjqngapf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jcujnxwk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ejfmwbfp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qzqzqppu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uodpcwto.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gasefhex.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pziqmrdh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2txcrgzaz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fedtroez.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2pzbxfegj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kbudsxha.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pdkawtxp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pdqzkbpe.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2paejhpgl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jhbzotnc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yuzbhhed.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vynfwrgr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2odanxhhm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xhziubvm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkbcrbbl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hnbwyhyw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hjzrdnsr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2exmtwrit.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cabtfpqo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pymefhpa.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2aiaztasn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kankyuye.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zdcrfrbq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xeosszpg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yakccohb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2iirsucdn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kbnygysb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ihvlaxhf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2duzimfgg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lqffpezw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gyonofic.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2iqumvnfn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rondljin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2wrctvwpm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ckczdsyl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mxufrxhk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rgptnajj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2oyjouzza.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2wfwwysgh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2evcrfaax.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vfgoddlc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mmrtkpbb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kvvzaqyf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nwljbeos.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rmtztxll.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2yocycqqh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gepftvif.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gmauspst.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2myieanzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpbdtqpa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2yulcttlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjoqubdz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vwxjddqs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hjzezgcz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2soyxnlhn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bnbninuu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xzxghkur.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjhnoqdh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqobyrvx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2eiiwaocz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fewjyafx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2alwobzqp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2osvboqka.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wnvjgftb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rtgngzho.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2keqgrktz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kkhdfowi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sigfywsq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ycdfkiqs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2newugzpn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eujwiofr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2oydunpbz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2azmnxtmr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dwbtbtbo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2sovzgmbl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aggsxcum.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ikgccfsq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lvlpywtl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tvsrxieb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bvcbxhrk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sdtwuxmg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hlrhahse.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cyelrcgz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fcwanrwm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gthiskdo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ihorrwzn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2luqfwpoo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jzgopftl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2neeujrds.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nhjghnbn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2znzxdvha.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rmyfcoqj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksnpimut.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ieddeykh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ybrlupyk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yvadxpnn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2yvuwiore.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bwkiolkt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2brnqvqco.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ugedjucl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aretihno.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dfasxxgn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gpvfnugp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2aczcbtxn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2afrmbgpa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ujorueiy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yesmothl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2juwrtsiz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zcpswfyp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2oeiqtpha.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2azlmfixt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2niuecgrf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2aitykdcu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dprwppxx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2uzmgdqpy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bdmqtaag.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wgstqmlq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zbcnyfdo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2feqxdwxk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wejlhpfu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mcstnwxu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ocluoltt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nzuzppxl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2daipklyc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2odyqhvbq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xyyvssnx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yocuhljc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fjrmacuy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tnbcscgs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ksrdolpo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2sfpndicz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yhgurpih.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tpnjvguu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2elfjlbus.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2twcnwlck.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaalggbf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2thknplkt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sosbezxf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksouslbj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xquitxgt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zyaxcprz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivjbocox.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2knxogtuj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2chhmpllr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2fwsnzjhh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rmawreco.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vwgdiojp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2spjaccaw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iamzjvgj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rraghmjl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kqkhshpr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2yyvyjgfs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rnxweypy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qncoubss.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xlegultg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yiybihfg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yutyoial.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ylssdqfa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ejvfaepf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2febebwxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dorcinkt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dndexplm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxgmzavs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2llneqhkf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kuxlrfwv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2cqztsrai.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ngumhdvd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xpknannj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2spxsjptm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2drclagsn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mllgnqhm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2dqrhtnzb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2avxdktzm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qbgqlbzi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gbtawkdu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fuxklrwt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wqyiaqrh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2klorbnti.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yikjscsg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2noycdgbn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ypftdpcf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lmgzmixh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hfjxjpyj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zykmgslf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zylviixz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yjjbhvem.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jwyzznet.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2txnsqvkt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2slyxjfjz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhiuweqm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zwhvewvf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2iaqvvwse.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fbdhhdqo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwpwlnui.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xnshcurj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bprdmqyd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lsdxowzv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tycburbg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppdcdcwq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hcgfkfiq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2taawdnaj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ppihkzme.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uxjmucmu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2iurcibti.html


<!-- 参考信息 -->