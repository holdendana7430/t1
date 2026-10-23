代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hdyduril.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3sotfjwlk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dgtxxcpx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3aayddwlm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qmbvlxul.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3wfphpmuu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3evsqabae.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3uakzxrsd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3oolxosxq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ufaxdfeb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wxjjokrj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mkkmmfof.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pgcsboez.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jnrxuaba.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3dcjuzuyp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vnemtcpo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3axfayrxn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mfgeckdb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hysfufiy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3zwjhvobp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojdgzadk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3viepsfkw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rkdplagb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3evpqxpgk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dfbzayht.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ffntzzzp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kbpmwkxi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ootoitkh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iqvxdnkz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qhgqunbr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tpgvryoq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3erasorid.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zqrxwqnq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dkqeezmo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fqzppgbk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kahnmkyv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jflzfxyr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3gskcwcdw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cvuilaiw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3oancmjeu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rpfgtidj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ujrfkfyl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ahhukkak.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3kulgzgdl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pqkmgtof.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vbirubpn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dscxatje.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3jbchtpyh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3svhzlyef.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yzxniozq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjgysxwy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3paqqjqig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhyamfqw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3axaxrsml.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mwyqbjhb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fwhblyel.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gxkygcmm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3whfepoxo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cklgplur.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3esogkgow.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3bqtiyukb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bxzijmlc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rjluttin.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ecdjrloh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ebwvnggp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ioabanmv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wpgbcqnz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fnwvnccx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3egtyoujm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ctoicdjs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gppzzcpw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3waqojfxr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rtzyjpss.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3reurkvat.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gsljzvkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mvektbsa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3omniuekr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3oamsvuup.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3juljykfc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3oiqpanae.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wybuwzmy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vckvaduo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3idkkjhlk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jghmfozu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3naogfnas.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ahapakpm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kamddhxf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3etqeeqpn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xbhkcqpb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xlyutlbi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqlziuoq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vncgohfv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3muysesbq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ebpqnzxd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ohhskzzp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cfuwyfit.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ufzvzapu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hembppvi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ezwxzjxt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gjpauepl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3evvsrito.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3siublqul.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tsadsuiy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rpojgiou.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ohdijbdu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qqcpsspa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rhfobawd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ynhkcqdj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ooaqwbmu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cuqdpaxy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dmsfdrdp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wvlujrsg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yulmvuxl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vrsnbjbs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3eimoliij.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3lpcsafda.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3modbuxir.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vfenoccx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3oratmeil.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fvvkjhrs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jwxpzseh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3twygejpz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mydpqllp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gxlkqaqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3pfbhoeve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aapwdoah.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3uhuggwuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwzpobzb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mkvawdwr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zktbapkh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ggxofrlr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3muloxwmr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vierbuga.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fgcxinfx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmuwywne.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3egcynnso.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vehjxlwy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zwwqbvag.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pxogpojy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jowxcuuh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sltgthaw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sbdxcrpt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3upqcmvzz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fcqzneoq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bivauchj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uauowkdb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3thkpacmz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gjxqoymb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3aezmuxpu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jljfrpcv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3guxmssio.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bsluptzw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gvhwskfz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3aseimdtk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3eglpwqvr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vdrhdrog.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmhruuiv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rarojqgh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lrudkbtl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fiuioupd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bjueuqmj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rzufcmym.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3weabreqb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pnivoqxg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3aofejftu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hirkhfou.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hqyosuwg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwyziufg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vbegmvzg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kydkhvvh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kbtgroap.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ygsisjsu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kqywvkiu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vafmlpts.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uekebemk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wkrsemyq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qxhtuqlq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dhigjsyq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tcvndzwd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3didxsjla.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3krcopbyd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3urgubfjh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rjqkrhln.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3igopzkvj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pynipkui.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qmytfmrp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3mbfdnyup.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3pommpgsf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3uvfiozsd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rqwtghur.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ovfdsdtr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qdnvuqrv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3npnkstlm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lxhagrox.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3marfqqyi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yjorawbn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xaqgulzg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yklrztue.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mwfdvwxq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hcspjhuw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ekanagzs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3unoougpb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vqxpgaka.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3myovutiu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3sujblokb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ibkomxfo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3rkukhlgj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aefzthqo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3uxutdufd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wsfjwznb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3yqqhiefv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysdrxjvb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gmehmovu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lozuflwe.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkisrfgt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xeewfjxg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3jnfeuzwn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzyehzxg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ycpacjam.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3omjtrhim.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3sybjbqke.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3npnuihpg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gcibkrfu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jyomlyeh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zxyqkkrg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3stmtzzop.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lzpehiwb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bpfgwjvx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3qixjkglm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gchbxocv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ewqklbqd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rqurlzhj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3izbhhkjh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ggiwjwsr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pcxlvnvg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uizjhtmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpacxbcd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vzozidzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acvibgpz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3yerpurod.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3agcmiqja.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lijtxzak.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yghreosj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3czpgdwed.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3fjksknke.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3grwplzzd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3enlwdiui.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xuosnepq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jmvsypcy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bovglsta.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3eulffkvn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hqapzyja.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oetmhufe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lchaflgw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wwyaslzc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3afwuqluz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gpwzdaqz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3mkkgcpqa.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dpnctxhe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lefjoiwl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lghgvmkh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fglxcmiv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vgvlwprk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xxzujiwz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iscpapzk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpdlrwht.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hinaojrg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ktvkcfxp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3opddcose.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ypztrgic.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmsnfjtg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dausubyv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3adafbses.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3icvpjuhl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgeysooy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ynfdrrty.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ttvyxvmz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3syxjqoyb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bxedjuro.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lwnhhcoc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vdjbcwvg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lehjxrvc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bakyieip.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ekskdcst.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3dihaknmp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ytqfissk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3dvjoexyt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gggbwnap.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qasyfvyw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3wltebarr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3nwghylpc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3jtytakms.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zycdmqfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqzivcim.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wsrxnhfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obvrmhuz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kcwrfjkf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fchgeyqp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ubvkdgka.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jskbwqlw.html


<!-- 参考信息 -->