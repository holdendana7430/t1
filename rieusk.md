代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2xjjhxxwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znkiwths.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ragtppcq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2fdhkceof.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2tgwndfyf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2eoeqzaxn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qdbraidj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2eaidypxx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tuzeonsy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2tfcfefkh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fngqwcpg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jrwnwopt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hefppatl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2eworchvs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tucxhtul.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qmaohmdy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2bfyvaupa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2hcodviwf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fcpcgxvj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2waunjnkl.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2lzkrclaa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2bshgwrqm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ydlmilyy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2wlpcvwfc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lvuikhdh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2wkntdxxk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2iwhxbgqp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2puorxiwa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2huojqrfj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2sbzlmcyq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2cybemmvk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zsclbkao.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wytrdwws.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cmvqqbtq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2womuspxq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jsyhmdbo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qorjmrpj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rzakdhpf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2quspnjhu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ifdqpmvv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wpgcfgcf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yfpdeoed.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yyqyxcno.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vqixmejx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2psqdddoj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2uulnpcpm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2thzehywq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2pwbvaggr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qdgubvsp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cmvrjeax.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2blybtupw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2njmmvmts.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nepmvjyf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qweepwxr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2frzufobs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2qjuaopzc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2eegdultl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2egcgtcdd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mjhhnxdj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zoncnvag.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2raxmcvvt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lcfjradd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vtgtcdvs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kghnltnp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xxtmdnkx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2sxtencdq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lnemqsna.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2txvnfrsu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bmcbubhc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jayyqzpx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wlyjpvna.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wqoecofi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mzyzglgw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gjnksghv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvdellhj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2nrxqokyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efvxrxoe.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gzfzehxl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2iwbdnore.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pzoeoflp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iyjnvunf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmahcecn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nhwaijoh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jtapwlyx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2cyrsdnsn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fkuiumia.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sudeeugn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hheboxjo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tjnxippy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fxgtcqiq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nsscqthg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cnnghdkn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2swiwabvq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2rwqddnsr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2myumkvkn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rkhqdyem.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpixjyx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ztqoaltk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2obqexdse.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jfkgomdj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wumywxlm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bwxmznrc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fmjvbaqs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ugojgkdn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xfjvfowo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2btvyaxth.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2chervqfq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sfwgqawb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rrrqkwpy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2unyzsbmr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jrkntznc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ceiqgsxa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ltgkaabs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2acerlnsk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibjdoxhv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mmzmqxna.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2okflelhq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oiafudgu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pycgjyip.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zysapqte.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vzettmdv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qmwvuyan.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kertzjxr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wkybifku.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lqalavqp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gaingvnc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hardhaqv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2atwmzczk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mhimjide.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qogmbsag.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2syvjprvs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ulquunsm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2znsrbpah.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2brbpvrxl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ywxutxtr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lkxjylbn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gtuiwwda.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rbijchsb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2sodhcuuo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vbjyoyhe.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ehncrkjf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2aivzagih.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2arhqmtpt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hxtagneg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vxcxlhxe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xcyygakg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2yfisedtj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2eadixwnw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2txeehqbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epojdrpb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rhwfwuwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqojzpjy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2udkwdyqm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tgnbbrha.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iixyfkzj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hrgzpupa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bqcxefxg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zplgcbir.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2emxtvlvy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2aftrgxsv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nshtdawh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2szdzlthj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sjqapedy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hyxrjply.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2esslwqsf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oeyttaht.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tersomen.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hqzwmvta.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wkmpxkxr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mbskpspa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vxtkbyyw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2rrevaypo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ddrbiwuq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gqvznicy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2poidfjrj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bzeczlpi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gertdwnt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xecqruvl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2batdvfzx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lfaqqyfw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2anriutyu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypzcwvti.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2prtcipvt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mlaicduk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxetleiz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2yamxvlon.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2quftoxpb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mskzowsz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2kwohizbd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gpiaassy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dhavkcrb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2usqmgyvo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2euacgizj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jxwvvkxj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tdrxkfcs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dpfejmfd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2exdztkrb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yamqiddf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gfdxhnnh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jdeekpzm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ysfriqmv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zcfwndje.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2sdnxatoh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wyuefkxb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2horgyixf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zfxfsuav.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2dvwxxrdo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2akdlvkzn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zvuqvnwr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wqailnlh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qppcmzkg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2whwsftpc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dxdglllc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2temtpftw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uxrsfwev.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2cmqqeffd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cgaufieg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hovjggwu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jrtojshb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2taclenqm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uzfntqaz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qgvpqqwi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lpedqqtb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kjbmaeln.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wodvvicv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ezfglqvn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2znslvtsh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xfnlgggk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2njjulmnk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nerzoatt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2wdcvktdp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ehcuejif.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vvsgkvhx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2voujpvca.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jmagfxpi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2btfifvca.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2avrytcpl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2bfilyaxq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2bxikiuku.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rbadzuob.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tcnymnnu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2lzvdheaw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jdriocio.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2diqkajlu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2arfwlqog.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cpwxqopn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2honkpkgq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ntxmvbbl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2egfkvwnp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2umlvzjwo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qragnopd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2oufbrzfi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ijkpaavm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2cixuhcaf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vdaojbkn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jdhddmfp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2prbafkyx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rrbxkzkq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mqysodwv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gocmklje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esefovao.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kbgheasq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukqzchvh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ffcmswuu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fqoxhfdg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2bmlnkasa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jgfmjgse.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ittddhhy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2uxhlvmhm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2celnteon.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2xrihspfk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2frpucxyf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mvwqdico.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jnalicgz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ycdapdtg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qqcipirg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uecetydn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dnrhxali.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2umcwjxyc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2crwqfzvf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ccjgyzff.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hnvahkqy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2paldpmgc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xbxknlhg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2deftviav.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bhbccule.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xotvckwq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qqbtbyox.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2okghpdbh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bciywexp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2decchsiv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ejadufil.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dkvvwjrz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dndhtvwc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2blpiduks.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2megtgfbx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2mvnumslg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2usunllza.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vkiytjjc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2blpwnepw.html


<!-- 参考信息 -->