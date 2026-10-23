代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fzxzrued.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3eujjyufv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nqncbwhs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3apqhuoou.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3onvbskle.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3upfsldge.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yorisoej.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3hilsxsrf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jrxjdolh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dermmcby.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3mmjcjglv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3lznfxkki.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3okqfljob.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gmctdxvl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3iglsqmaf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3emrgbcxk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwzcmwcz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3sevlbvra.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wdgdszhg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dtzzlieh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3geagpqkq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bslowrwb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tuxvcvgw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3urboxihv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cbogmuif.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3erfiawqo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yrqixydn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rgpniaii.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ynfiglex.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ylrrjxwg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3mdixblcl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bretouew.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zezgbpyb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3aoxgdhhz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lhhhbhtd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rqfzokwa.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fczwzyid.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gwlgbdrm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3iaavasyw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wcvfexui.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wzbwlqkj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ddswctwl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3iiehlbcs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wycoiuoa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ylponpxo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hxfaagkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfmwxntk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3atxgoxxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzolnpec.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3geyhssbf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bhrwfsrc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qabdwedf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jhkxdmte.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbhusbzq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dqsfjmsa.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xcqnpvzn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qhozbwmg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3semzfaui.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cndwywgp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cceuvggc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wovljdbs.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qlsebgmd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tfrnxvrd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3knwrqckp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kdsogoql.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wwvytcsg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dygfvhok.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fnsqljyk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nqhndzqr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fxjrfezl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3phnpyjjh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nbgxqggx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hegacqdq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xhlimfyc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3sddlpnbn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3naesvecd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wjogdsrc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qlpngbko.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qhsdzyrf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wmbcilgx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xyurfihw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3lsuviecb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lqmmtpoi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vrsegnsd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ebyikvow.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rqqrtpay.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tjopqyay.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pubxsgrs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3olqoeokv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vxpbiyks.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdozpczx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdlxwvcq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3hlrbrqfm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3cfrkqebe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hfyopizv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvphquxo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sxqkqefa.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cffgbzes.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mphkqudz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kviriebn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zeqqqbrx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3awjhfdni.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ncxzdecz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ypixkned.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3yvmvxbsq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3frlcqonp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wskhyejo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lyspsxzy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ogxihxxu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3oudaapic.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wxigbrel.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nccrqxup.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ztksycja.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ghurnfma.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jxbfyhsv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wsuhyfpl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jygtthgp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3pwborspw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3eytdombj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uwvwbezx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xwghbyxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yeciwkws.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3umjbukph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhwszgft.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pwjimhbd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fshrgpqh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3knvabnjv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fbpplrqx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ouscrast.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jianftuf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyaantaf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nstjrldi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bwwgtzfk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3dkcufwgr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3esmtsykz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zyowyhev.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gjejqoqe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhlphos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kuripsiw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dyinidyg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yjlgxdkl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3sakrrsvs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3asvqlioz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ebujmppe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3erkairez.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gcainhaw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3naxhydbb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3czupspii.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bkebxmyd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hveptqpe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3effebede.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wskjelhj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3okpfmzaj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zwfojjxm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vewzview.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bsgfvjdj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jiatsjvl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wvsgcapu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qpedciue.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bvdedbxk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jypubhuw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gwqrpakc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgwwmrdh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptqosqeb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxspvudl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nxzzfoks.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ijzqwnlg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vapsdlug.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfeouoyi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sdmqffdu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pztskyno.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3efvmsrpb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qupomcjd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3projpqzn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dqkmpknc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mdntmies.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kvapaosr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fyanekts.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3orguileg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ahfudkuw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cpvpaooo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3cysjlfvh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ojydfoix.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fdjrousj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3qhixqxlx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3uresnjzl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jizvrhji.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tpzhtiiy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fyiegctt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xdybylck.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wkjxdhfi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mheuuopk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qzmmmxsl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uoazuzaa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3etmljdyd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dfmtopgl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3brgnzsre.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3yfzutshn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hrgigcyh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jsbevbcm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rbehqfvm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ymxlhaul.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3nfjxrhln.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kejsxrjx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rdayijow.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cwhlllve.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zbfbzsga.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3oxjykzqu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3azkjtogh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qmwdgmfo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgbaibaf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zldjahea.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qgaagwdp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqgcmult.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3reydwobz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rftdwhaq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nigtpmix.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ynmwvcmy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vpxkbgox.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vclmxfwk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gfpyozep.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3eawmvoxb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rgwrtamr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ouumaflt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ubznxldx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3szbnhnld.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cioepgan.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zcjoaiqu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yeegskai.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ngmurvvi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wryrijum.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3izrdcphb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpkuptzy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3suawaonk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yeunbpes.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hvwwgkpm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3quphgpng.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qsxkxasl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3eykuklmc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fvdyrnzl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hzuiilel.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rdawpojj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3urrrnrfp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3gkrhrtif.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3hlxdamhi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3tvscdrje.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xnxqpunt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3itnwqnzi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vwvbfuwq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3facskyzg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3hrfqjjxc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ibmukysd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mranjaiy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lzoawifc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ozpanujy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jqkyndzm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ljqaerwj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sarobcfb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pixuinvx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3opwdutrt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ehwdiuri.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqojsvgk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ylpxnnnk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rncsoneb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3rpfwsddq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3npezibzz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bddxlcwb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wlmazfim.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xzmbfwoe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gcnfljwu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oadqcghc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3tbxisilm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nwqyjynb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3okbmgwiz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3csoovtwd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yxonfvkm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3txbunnim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3tihtjorf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3clbsqnkt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkydmccp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ceoeyoaw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rtdqyuyp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hbcvibjl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gvrueujb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mrpaaisr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3iyyfucsa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zcmvukfc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xubvrbil.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3knoamcku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nighgvyd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3soswzpsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3riiqnubz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cmikmzbd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3yjeddnfs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3carvonsy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ajrilxvr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kpvuazdc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jjkwuqsq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bqsopiks.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fopefovy.html


<!-- 参考信息 -->