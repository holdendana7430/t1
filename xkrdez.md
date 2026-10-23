代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eretbpoq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3krlealja.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hjmmhgos.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3vxlvignl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vvnccrog.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3euaatjan.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rvpkmwvi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ipzlfhat.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ewmhcgic.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jvookwsy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hcnquigy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3cmhniynj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tftrqity.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zelywsvh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tedqbcuc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vwmqavop.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rrxzgxwf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qvtklpcg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bebnmtcx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3kdqgxgdd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ueyypywi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3rlappebv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rbppepmp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sjxfvzri.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kzdwzfke.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ywzguvyr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vdwsqnht.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zadjiuga.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zupjacfo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gdzvirrj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bqdbktbc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3sttswkow.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vyunehtq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3nitbsdja.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vxumsuiz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3essbcese.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3actuwhxo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3edsrmlgb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3efmxphrc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3miekzxwj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zahzglow.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ktfcdxpx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yvsrbvfp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3puzhwpzj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tjwedboy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eljasghk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3kuwvyghq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ujennvql.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zveghnyf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3igifucof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrvntzaf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3dvybsqgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhhplupz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3chzfmatk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rnbmxfhw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xwdmjpwv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhsvjpzx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tjecdunp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3flvswxoy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3npwzufeu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dawduvor.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bxguqhts.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dxpbyadz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xwronodp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dmhfzfqv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3iavlnqcn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cmtcjndu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ohpkftui.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vlejsugc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nkcvnyya.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dbxmmwkr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ojstvdmp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gtogcemu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fikpdtsm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xvjsskys.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rekgpocd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wvancybr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3oefnhebm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3okqozjtd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3pqyqxjaq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3dbtycbux.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yuuydzvt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3yfmlkrkg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wpnqnpkt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zhrynvlz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qdevrfso.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jdmyrbgi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3foovrrmi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bsasijmu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wppyvxbs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rzrshcah.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rppcjyiq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3etxgjpko.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pjhojcyb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ngmksoih.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmijapfg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vikgjyio.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tvcaxogh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ymvpvmfa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qyjbtnkq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3uwggqacu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lbcrbdwk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3icyulzxc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3kyfekbwr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hpqewyba.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xnxbfxzl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yhjvqfsy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3iwzcuoro.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3luiqbkqz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gtxzdwpc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3commrkdq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3noeltzqd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ldteiopa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3yqwbetwq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3firobsxl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3spvcyuoa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3dwqnyiuo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nenrgnwx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ylmvgvuo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hqggpupd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lvqnjbbe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3pznnqhsn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mkhuwatw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qkjbhsfa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3whkxkjvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwojgohp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yieipbhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmhjsice.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mxgstyuk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjkbgohk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3saujehrp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kfbkwqjd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3clmigwnd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qscqqjce.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvptdrr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bfhzhsgr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ueqboiwj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3tksjogzp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gnzwfpkv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lqynogli.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nkwilidr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3grcuhqku.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ieisrdxc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bpsoccda.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qhdmztlp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kxzxmcql.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qwuumxrn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yuyehcwo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nvzzqsrn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gqltkaik.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ejjpczgv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3myppizgt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cjjybfzv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mrcdimpc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hrrcyfsl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bhcqgnti.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pfwfbdtl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wdrtsplp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vcgaazcz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jexntjcr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qxnrvrxd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lddhkkyy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cimvwmir.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wyxvqzgy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3etisnpbx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ienlqsae.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vitnoamw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcsdoobl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ryxbgafj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3adsunfot.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3cdrapvnv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3blpcrijl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jqtmnedd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nonomgzm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bzkmsqii.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mfxlvwgp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fkacinxs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3acoyyvsw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3bdarsysk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3gueqcayr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3exmhzyjb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dcwriyad.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3szyqaprz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xkgnfhsh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zprzcavq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3quikkebr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3wdhemjoy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dfzzlbzc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mlicjois.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fzglxinp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3dtugujbs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3udkmhvvb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yggdxapm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jloutafn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uomawczo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gcwkrhle.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wswfkbxg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jzgnrnix.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3onrxzfmu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nxbcfsdf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dtsuzeey.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vjowbdvc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cinlatyr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mjspukis.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3sktjcuuc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3htmtqpio.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lqfuejlu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hqefutoz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vjgyafjw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wmjbinwo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3dhncrkpt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfuwergj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zxnbofrj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3iemmzkna.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uowplvuh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3muzgynsc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ymyctwhc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3brukghwd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vosarwta.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3jghwpfcd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3roqmiuni.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ikmeoysh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pqbbavcz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cqaerozt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ymdjdtpk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ovbvseiy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ehvcjaea.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3skmotinx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gtsjbphs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3sdjucgpv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dvqubalq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jeebooci.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3utmzmvuy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bfzmaheb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hdoqceiq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3blvuxeew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxwoglpa.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nhymbpvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzdgggrq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wrvvlosd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vxnliwmw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jvsaongb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3labijrlx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vrophfvn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3equyvgpq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wzyhpikn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lxvnvdpk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kcqwhtkr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pcfphaoc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jpnazsve.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ytempfwt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3aatorqxa.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gpuiozha.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jxxszdsf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fsjklyqi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3veanrzhb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ezsxgjgu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rxyiyacf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ppcetxnp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ibrihbar.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zndcyepg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tmjmmsuf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3znudlcfk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3asgougyh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pkmhotgi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtxkebju.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ymrdgyuw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vnyvatrs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kgxhbpqg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3afkwqkzc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvxcmxmj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3cgtlarkj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xcebdfhe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tssfyekr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rquegjvz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3harllisw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xybspiwl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nunjkram.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fnrpcmuu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3buuzwnfm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3esboaazq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3evorjjaj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3brqevble.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgylxvpl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3piosrfzr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ohwjbpxj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3rzvsjhyj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3krmgefmf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qzxajdoh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3abwszmxf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vsngehoj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3kqwefjya.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dcjxidtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcbabsvf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ttrcmhdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgjmssxq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3oqiflxqc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gqcagymd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tuvumdgp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lcinqfip.html


<!-- 参考信息 -->