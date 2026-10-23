代发 wailian999

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tfzxudhk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3xelovpvt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ncfokgxy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3svxzwhag.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ficveuci.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3tlrkvist.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jjmoheko.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3makufudj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yffaxmqo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wdaoulxf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tykmalrq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3twuzcedv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pcxmltmi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nslfnreh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jnvgnpgf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tvzgqphz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3iblatsuu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bjblavzq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rgopimjd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wbzvieaa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3upuoxsmo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ipunirhp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wdpctbzl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3febebjgg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3tqzdpnkd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3kaqcefeb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aljxcxkk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gzvepgzw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dndhpekd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3couvdqji.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pgapiyoi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kjlsdueh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fmpqhlel.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hctabdoe.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zjljubut.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3iktdjacb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dbchmwkk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tsuybqhw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3evqeclre.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3spzwsmok.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wihadeep.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3oiagxfzf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vpwsndzm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qbxcxijy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mxnsqthu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3zxitoqvh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3inkifnyb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bjlnhrro.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3szhghrpb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vdywktcq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gryxcqhl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3kcrhptlf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tuiexuoe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3whmklwzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hinbmyri.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zxxqabzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggchngzf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dnfyigne.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jtxcpreo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3uwahedbi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gewmnbei.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3khceskur.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3crukfwtg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wbooubed.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wsyctiin.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dkovnhcp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mwwkvsct.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ckdzuxsn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dpnaeyve.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3houelhkp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fmweavok.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qdhdihqw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3atvuzsrk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3oqzlwdpk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3snvmuyht.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3nkadbbpc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pvkwdywl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3vugpomfv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kmbqteoh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zhmheeke.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mkteazck.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3skywcnod.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gaifuciz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hiujixyv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3sogkltbl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ncrbzxuz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3kthyvkmm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wjqhtjln.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vkfelyjt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tsthvkjw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ggwvrlqn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3icgqmxdm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gawzxvzg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cgvctrxh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewqvlblw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3usniikun.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dsxudqgb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eyaythaw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ltjpvlrq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hygndbws.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uvjhluxb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3kanjzrwa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fkvpcrgo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bppdnxco.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ocqjyhfq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3getukvlg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3msozqfgp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3vurbvzhm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ujaucyfg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vhzebofk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jyvyjzma.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3liwjuzhl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jhmvoydt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3yrisieyg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vtdztqya.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lbwdesqy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gbdowxzz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3giqydrze.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cuezmrzh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qrownyuq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rjwronmq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3opecmekb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fnpgruel.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ueswenix.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3babnnesy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3daryrdkr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3cttryffv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qcmrtjgh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fhadvvjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eildvxby.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qldreury.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nypmumzf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mpifxnax.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwthuxrv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ahobkpah.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3prwixgrh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fvwiqluy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bfzamzgv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvazvgso.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3cnbvzczb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxwlxaz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bvlltzyl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3loxfsvpg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3spwijaon.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrjrkgpx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pkwynqod.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vcksfeet.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fcwfqzds.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3httawxge.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fwnhcqlp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3knxnvbvt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xovaxmlp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3slhuhuvs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zsvirsyn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mcerwkhg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3oznzcdrk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ydkzbjvk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dpcuzfns.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nnwvsmes.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dyoadjju.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycheaqqn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjjexwzx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kgfhpmec.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fnkuxdqt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zfxlzddr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3roonlcok.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipkxwtfp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dhtpsmpl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dtzyigfa.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3erpaxgfb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqpvqsee.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3chexrztc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgeeqrnf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3whblviag.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3eyguxvcb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jbaexfhb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3yneuswri.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wckarwfc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fmhkwwil.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxlqnqmj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zsfphwuc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3axpfssdv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tvoevkvm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3yskbhjti.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dfgzzxlf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qznvwyfg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3fsvgrbzo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qbdyvmgp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3lppoaolm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xjoqsljw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ixfetgux.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3yespwmnr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3gnwnrrth.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hdrriygo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jibkipew.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tylexdeq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jiwgtsrf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3aaccljvc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jiitprub.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3earpldtl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ywbrrpnc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3trzscrmg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3fflefapt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ycqvbcyu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jbpnytzk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nrrjrrij.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cbapaekj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uojsfzqh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3edozgrrg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3miuzutsx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pywflerb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gxkqzxrp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eekhwmpt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wrowlbzo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vpmbxjdy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tnwoyphh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mrpxicno.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cnevosto.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dckcbuym.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wmlskrlq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3abazlfni.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qixnxuka.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kgljumoy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ctczqzdh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hvjcaxmj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yhhifink.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3exzbimbd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hlneefdw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sktvsdvc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gvrclymf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zwxieucl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3imdrqwtl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ujenqlwg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3giubqvbp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pafzbupo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qqqsntsu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rejtwmun.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fcvsfhcr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qsjkownx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ozinliay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhdpaaci.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nbltcgvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezxndvhx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ekrfczto.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tinqblnt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dowracua.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3wcbariqt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aapnzdqf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qpozjnbj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ikycptgy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fqsjqquh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3tafqlefi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3chxvbzwc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nslhfacj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3olivxbpt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fztcpvit.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bmtyoopp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qypymupb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3uzdlzwkh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3xmfyehus.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jkowaqwb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3sbheurba.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3epmvyeqb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cuxtqqlz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3owghgnac.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qklifuqn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3snbddyko.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3honacysd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gvvnjrqq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3szqipvqe.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qbuzhzos.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ylxvkchj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3djamfyhs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mmxqrslx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fghxrkxb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3btpmckzm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ejxyuaws.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3apfyjwey.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrefymfy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3jtcymtkw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3cahzepgg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ayzcfdwj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ztlqnzio.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xwfkmlrv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3aynmxcik.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wwpklhay.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ozluiqtg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hyzdznog.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3dnespxer.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wizdtnyw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3trsbggzf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bqxctwng.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rwqdppgm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sxwigupw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3canvgeqm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3etifphmh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bbmyabet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syqaccxe.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghgoxxno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alaesebt.html


<!-- 参考信息 -->