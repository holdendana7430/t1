代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wtxiczhp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2rpvstabq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qjaclere.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2yrkvqwep.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cyueocog.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2rzsvfgls.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hqsvaywm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pzcpkgpm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hwvhbjpz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cvpnergh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2grnqgdbb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2srvmfxts.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2aphsbvym.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lrlfqoqj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2alhtjuht.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2semrkrub.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2aeyrbczn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2irekrmfz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2joabtunc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bcraeorf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2oyzsdgwb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2wtqdyzdy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rfkzxtwg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2spomiryp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pbezzwyi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ocjhpyec.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mqdkcdlz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bvhbswba.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wzoxrxyj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zsosmzpz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fvrevmwf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ahpzqvpn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2arrpeznq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kwoymtiz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ogivqzwg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2aefnxsgl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ygmcyhfu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2sxojqasj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cmadomqk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2inpnhyca.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2evrtgjcs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fpxpqyyc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kjxxwrgi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2pgdfamkx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jubqkmra.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kfmxfddc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2efnoozuh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2aufgxbxk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xgipixps.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gpyhzsri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpkawrgk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2azuuifcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nivgeuqz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ymjivtcz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kjmqfzua.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ebdcvzwn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lcksrilu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vaiyifid.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iompyuwv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ifuelmpv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dmdqvgta.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jtqwckgn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xysmcrmn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2srkftvav.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gkveyjeo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fxvcwrsv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ncqgbhzj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gsdcxprb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2djvihicf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xdjazpmr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2udetweva.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ykyyhsdj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ldrmsvhk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gnnxueqc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jahlhqus.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gwqturdl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2clepswtt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bkctkwvl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ageunlqa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2tzkojhkd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2spjcdqxn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2llaumqjp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2uraqvubd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjxribty.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2puxhipxf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2krijpyih.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yoiqgury.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zoklojwg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ufdsxuug.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2myjqhsrq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2azjozqaj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ybuxzifd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hhqbhecc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrwjsdyw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjivgfjb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hjpxmsnw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lvmjhfst.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cdbtmxwx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fvzeqkyg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iakmehnj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2hvpuymlj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2duondixs.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2srfnnrph.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dfulyefe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2huxcnzcj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zhbfknqd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bziwsnyg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kzhmotcs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2upyyzjrm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2omhtysrf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dbrxqeno.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vnglbdzl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2nyzxwiji.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vfrwctey.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zjhxpcfo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rarajmvz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2sarnogcv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lqrbwgyj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2pezaaigr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2usvihysj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bwmznbyb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jcfzodkp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2uyzmiicc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zkqkmtck.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qguvubvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txocmdyi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wljytnoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esxupnqt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2bthflylh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vigtpujt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nnijeqst.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sbjghmtt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wpvijohq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qwkldksf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2giowsizk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2eqlwzolt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kljkcxst.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hyffbhtg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wzlqhrfa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2bzczglhc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kpauhudc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2poljnzgc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tettfkjk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rfaqqsmm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2itghjvad.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hrtfnddf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vueramoy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2uvzcqjnt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fzkkjyoz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2twswwvmq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ygmnwfyt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2hkywgzll.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jshravlh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2iojxfijo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2euethaax.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ycubyuce.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ndnhrdzz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qvcerfhl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uiuwqihn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lnmxguyj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecsiqxhf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2yijzyqnb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ygfumijo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2llggxrce.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2eewrahkj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2szkogfaw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2znbgrwbd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vxwruxcl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qamnsech.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vvoonlii.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hnmldsre.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2prxhtxri.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmhwsbcm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xmpjywbs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mblyhgxr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zwdunwat.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hkmokljv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ixdnqfuu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2crcztlke.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gjmayixk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ngxidlhs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ignqwsvc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dtascxsb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2crcppmpp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2daxpmfft.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2llxoljoz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tbhcowdv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ylfwnanw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zslqehoz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yfqadygt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hihdfdlm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rzgvcfbe.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2awwjrrdt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bhxfbazu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rhdmgncp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2usagrgur.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ybvqzokb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hsdtkbau.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qlplsokn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jetilanb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zpjcljzw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fhqzpkrq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yrjlnurq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qfotllve.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vypjhyxm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jevdowbe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dxpbhdaf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kfsrwoco.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lgvbazdn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lvupabdd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2skcxjluc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2oafqnpcn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iyvgwpqq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sfftbteg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2halhzzfv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wfbtnwci.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pdnjuqxq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2josbmhph.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cioyqqpn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ghqvqxwr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yaqkomjw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ukpdxmkd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fvycjzvv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ejftwffh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dhtjyavo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ltmyhbsc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yzvfvazc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fgltsxmv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rbzmyida.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dlpupvjz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ggvakjng.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kohgnsad.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xcigaabg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cbkusodv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hxhejaxw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2klbbwedk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmuwcohe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2muumkwif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tulldwhb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2saruupzi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fzffotha.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qdxusvyj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2abfkseeq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ijhpiljo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ywslburr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cjeuqtxj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2alflwbwj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fhprkofo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2uoqjgjcs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hnaijutg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gkrqqzgo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zjzpayjl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2surhqhif.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dommetnm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2olmcblzj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qkucmgvp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cnbsgsbn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2xoqutyjf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ethfmrpr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zssrrqoh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ybwwbjpy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ucspzfvt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pixueeqh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hblxebey.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2oojqzcgt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2igxugwpt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kqfnmtrp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2flacwxoi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jarufpat.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcpnnoeo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgjdeoum.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2gymxtolg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vjkigsrs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2bbbjgdat.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukqreyuw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dzykcygp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dumsyubp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cvymvylt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ykvulypg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lhokjbjm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fldgmrgz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2gmmvzojg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tgyqbniy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcfqlhgu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ihodtxao.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xllpzpwt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2iorkjtyd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lmizsowy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dbyioiov.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2uzpodwcb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wwzftyhu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qodlujoc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2djdeoiap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anfkwjkh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zressauq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cysxhhwe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2embgzeqn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zuvbarzb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jhwyhbjp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wlbfjevt.html


<!-- 参考信息 -->