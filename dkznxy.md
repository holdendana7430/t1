代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gxlkmird.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3oxkxolad.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rsobeebh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3custbuxc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3muycdazg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3tmbtdxzt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vevtdmcc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zvjiihis.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hyfjexki.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bkyftvlm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3lfmpbpyd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ykftejif.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3aykjszsw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ymwtrike.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ckgusupx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3atlvvcbl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3mzxpytfk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zboufxzo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rhvczlti.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3bznjnbua.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xfpwsefl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3vjecqsjv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kkcgmohu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dwzszlup.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tjfuujuc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vytqqouo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3oamzdvbb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bbmcurkn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ibooqmaz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bequkzoy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hlskfilp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cbssgcww.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gymbgyth.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xbwzszyl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hkwmvlso.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3egvmkbpu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uceisvvg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hbexczvm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rvipkdei.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ikbgrijy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3imhopuls.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3klosleaa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rsewvsfv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3clfmzfvs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rqmeccys.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kkrswrio.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ypicvvve.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3oozugzji.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cxijjawk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zlwpdihf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzudcuzl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3dqjscjzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dapbupxs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ebqsyiaw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dgbximap.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qwaiwfyb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3brugkolz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lctdvosl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kxxtzvwf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wgyvosgz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3upxxiqrf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fjvbvdyz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uxrvnfvl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hnempije.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mhrlzksu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3biumjzeg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mjtxzfjr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kseoomvt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rqvjqhkp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tcaqnygv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yvtjndcc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lzpwtmqr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wjifjfao.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jkbkjnlg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tjyimwod.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uqubhafp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wkzvojay.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vmzwzobu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3msueegcr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mcohxlus.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mjgprpcv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hdzjukhj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rdmoygkd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ociwjrdt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hemkyzdy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yabvnket.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zvahpbox.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vgkuxwnh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vunlawch.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jyfnovlv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kzmccygs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hjswizbv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3czkzjqyt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pyyhkuze.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvyssxqn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kryobcke.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vmxsitaj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cenrrmwp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pioxtpfb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uykchywq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mkggdamw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gfvkbhvl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gstcloyc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ikdwcvyk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nxuyvzjs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kpcvubua.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3uwhsjkkr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3crhtepid.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vbaqshvg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xgvireqz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pppmwned.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cltmlzvb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hvqbqppx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3epkmhwuf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3siputbgz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3cgvoserl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qwxeuppg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xvbqptiy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pkdhyiea.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ehudxewq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3huqipmeq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vttvbulq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3oxpbtpuc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vscgiggo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3uujefnrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtvzifdu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3nxwddutm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgbxwoik.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zphspvqb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddeisvhc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wgfgrexu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wrsmnjfh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3omegcygo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sweopsqv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ftqfgjip.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rhmoefvq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3evnhdskn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3cwmazlrn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pevecazl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fbznqcbe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gcjhgrup.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yrqhfncs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zpvqtvud.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lzfxdyle.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3iziabncq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ygqpqlxv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ohyyitnz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wxgsglnl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qoasfnij.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hfyepbsc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dxhzolvg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rdxsmiea.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ltgttqtg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rqiexcgp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ikinwtud.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mhbnyfrz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cvdevoqk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftbxtvye.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3njkowiyv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bdasdfhl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzpmudun.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3idlkjqwt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkcbitoe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iredzfne.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3acotievq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3skghybwx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcvctttt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qsivnwqs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fcniwmvx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qzhyfhbh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ztqknmth.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bosuyvni.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qiwxdmyf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qiduysdd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3whaxlghs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bnsunzxn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3acyyaiqh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tmxjatxm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rhtgdfas.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vnffaobz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mpfuiurd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sdwfvvjx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jqvwqmuj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ijczdhpd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3yfunrrnq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3dstedntn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ofcendad.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3niholmak.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3lcrwehia.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zlbzlgeo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nilinwgm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qhiqqkwy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mnkrlcug.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bhorckri.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qlgzwago.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3unjfeuoe.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3igxgnsor.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xvumreso.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ysibsdbf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iqqzeltl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3foopskfn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3uaezzxpa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uqsvnznt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jbwhdidi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3eatamymr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oqhchath.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3swwarckx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vrajevdv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fnyegxdo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qeggdscm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3evsfuwkg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3whnkrxxj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3yilaqmhi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lzhazpur.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogkaujia.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wmghrole.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3upfdaypi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kcuhucga.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mrdvaxva.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3igcweaug.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dgqotkfd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xvgrrxhe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mirlrurx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ctqafpkm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sljzwlxw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jtsyqyat.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hpkosskl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lbgezvzz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3orenlsdf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pmndnkax.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dfiutsen.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tlghpcvn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3plfmoakg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3spwkrfss.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3srzslehp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3swhzvcji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szahsavu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rwyhcwuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iejodtew.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dbtnczwj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ybrhtqos.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rjjmfifo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ugvvhgtb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3soinuwaq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3scuccbsr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vjebbqre.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kfttrbnj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cnwgzvxe.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3smkofgpz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ofdlpsmt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3opjajrns.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dndmmsmu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hpiwidmt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3joahflnh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zqgcfkpa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kaekyzqx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3bavrkirf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3eqwyttwp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xdyqnbin.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ryyhjhgc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mjmsnzmi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cixmfkim.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tstopman.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3eumgoidr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ajrcbrmu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qcvvhwda.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pnqjxphq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3lljgzdbh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3chkrqgil.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fencezwr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dcawzdqg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3bzidgrzf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zdrofgwr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3yebqkeak.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3btlbtsue.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gdgikabh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rbcajonk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3agilwkwf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pqctmjiy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hahhgjri.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3umkdisqw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vmetlwqy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lyfnalqe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3sulkhxru.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nblrhiuy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wdcotrwd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nwrwnyuc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3szbblehr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3alkjiihj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vgtwmkeb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3tnlhkcxc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fixuhnad.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3oppxxgnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3laeqztqu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lvxynxik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azmogmqz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gxfzyscr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zqiohmxx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rqgxxtet.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3drfotunt.html


<!-- 参考信息 -->