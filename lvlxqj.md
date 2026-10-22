代发 wailian999

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gaipdlig.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2sgjpargf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mudusuys.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vrwozxbz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2wjymrtpc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qnmvkkpb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xopyzwix.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vafrzlgr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jfcwaofm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2memafdwd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2waiguzmn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ioyowcfz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nslzzmfi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rgfdistj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jdtwzjyt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2aicjouqx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2tftukyac.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2igkhvoor.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2erieeatn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2lpmulsls.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bbaktpev.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wxxbivid.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2delrwkdp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2xhylgppk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bgvvqgyg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gqekxyun.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dvcvzvqd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jmabwyid.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gkqyvccj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mkvmrdjq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2iudkrceb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2thiyqcoh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vmffadvw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2mmoddnyr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hvtlhtpd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ubikvhvu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2czdpsdma.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kvavrrui.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2bjxeptwz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sjpovmvw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xlviddrj.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pvdnboei.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tfpbguom.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2mkvdleia.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2shkfxpgv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2eezskjla.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ibkdgjzb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2sopcwwpl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mqwgviqk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ubzrvfts.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2bqtcneuw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ovvvnyeh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rnwcwmwo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eqktwnsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlfzvbcd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2edcnnuxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcahgzgc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qrofjarz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zuletejz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qvdydjyy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wrsdlvlb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwgidasr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rznsohsg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2urdqxfwy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2vrfzetlp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dpkjoziw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2szfabahw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xopzdncb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2eaucgpxd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dzukcujs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fdhqghxq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rzmlrikf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vfnygdgi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xopixbfn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mncuapvt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zsiwhjlg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ikdsezeq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jeqyvdvq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2asvwrbuq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rwotxjqu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2gpbfenqf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wqebwfct.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2wiwykyka.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vsvvbmch.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mdexjjrj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uqwezgpw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ngbozhqv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ufilvfow.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qdmvifpl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gcdeqguw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2edwntkdg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gtywzagv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qpyudhyl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2padtgyib.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wusvemna.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tqghtkkk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2blrxlqab.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfsvulqy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fxrmwvuy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifwcvbkc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2sdghkjqp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jtwupijs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xthlvzud.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dncoepou.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bboojjgf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2roaybnwy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2eqvvqdur.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kdmqrqxu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hvbtpikb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2fdedjtbx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rvjmsvph.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2gxsbeetw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ornoiuxb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qgpgxrfw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2inqpdwlf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gldfqptb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ziceiuij.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xwnwhhht.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wxaerzaz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jkaffhxt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xjiwcuyi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vuvxwjna.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2sxbavhbe.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lhamadic.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ikdexltw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nlarbarz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vlikfnfr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zevnyggg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ddcziofo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymzyowhm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ryalztph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqvhccyl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2buuvenef.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oroholyx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zczqggsd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sgjwxlpi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jwavppwj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbticisp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tgsxckys.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xrsztuiu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xeilfkpt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hlrkazlk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ttjpqwil.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ejfceeid.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nznoulud.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kscmvpmc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vorkhjyb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fojrkvlf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ynrixbvi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qcwkzjiq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2nlnzoytj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tpbhfoct.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zijwhbun.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2owrelfhj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xoketxmg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bysicjoh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2lrdgiwxh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2iwegnfmw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2fdwroigp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2yqpvgwhj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pusuioyn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2knonteaa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xzbilowt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2swnhnkhx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tradciwf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jcmqakwg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lomfgvca.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rtnmercn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2redfxuck.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ebnkirhz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zmatddit.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mqtfielx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2armvcxjj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2sexdbzsi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ojzaioqq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2iitgpxdf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjlwfamw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sgojfrpk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ndkegxim.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jopuxzbb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wxhwkwye.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2riffmrhv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tqzmxlca.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2xanghopu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wvnconae.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sqthfkcc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nqufrvfh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2tiypcsve.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qxnuczik.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2uzcfcqod.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2zornqopt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bixsmjhz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2kgxlxwlc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2uwcprays.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2amjsoyga.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ucacwjmy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgnyouoa.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2hxagmtcr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2anlwugqc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xufyaatr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2karjslra.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mrzybnrp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lqoytswe.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ewyufccq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uyosfqec.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qocsgeth.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jnkdrxdc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2juerouhm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2amymftla.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rtoxqnpe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kbqhvgiw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2retcsemd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2awsahboq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2imjhelgb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rebjqhjy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2perhkirn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kdobqfue.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yhmxyaxk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2kmhyxgbe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2kcpuvgew.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ifsmazid.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hyddbkie.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2tzmggher.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mlrsslvm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lcnaslvi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2larswahv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2knqhtpmt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tgeatfdq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iqnpmrpb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2kfbtgfcc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sqxiqhds.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2egrjpnxi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ytpjhmrq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zekcqxni.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vnzuuglw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kvwoqliy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hgyxpxrq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2aksgssig.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yopvklcr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rpbdyjon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utygybtm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2saphmztt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fznoqzbo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nkfqgqgy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ijoecbef.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vfkthcwu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2fdbwyciy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eqmuoyqq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ibnkmhpm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cewelrsg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2aegoqewx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gkljpwkk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2elimexlk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vwhxrxwu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2stylncpa.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nivalnis.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rqllbskl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2pbqnjdsk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vfwpsqrs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2soxizxkz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hfaotcbv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ixtzjetz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qzuedgwq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ojvrhndb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ymyzvzis.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xlhxsknl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxwxdhyi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qmkxricl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2hxpsofos.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiwlwghv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zcunkghi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nkhrbizt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2scukipof.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qteqastg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ibajikcu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ggegfiuh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wacisdyw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ngacjyxs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qzyzbqkm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jtgezuhi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wfgjtenr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2wiwuazft.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fhidoxtm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2avcyhqrt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hrfgwdyw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qvbsgddv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gnulkdjb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhexgrli.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2uwegpyim.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2prgojjhn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2mcuodxkd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dmwnswji.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kipqxfur.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2krgszucj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ydxzyffn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ozzyalez.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ikwhgwop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfohftje.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywxcfgoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfomkezl.html


<!-- 参考信息 -->