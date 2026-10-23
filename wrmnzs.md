代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3eebvubkt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3eiyzgwyj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3krjryrme.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rmvnlyps.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3seeiifkh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lhqfsfaq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3famvdjdm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3upinoryx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3grvalxob.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ezzcjqrg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3usmgqkfc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rtdossxj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxovkdu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tvptgxat.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3aqgtqhts.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ffnvvnqy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qmmdjixy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jbnzukyr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rljvaycd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3magavdrn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tldnmptl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3kbhwsiye.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yxeogoen.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qtpeyomt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uvtkvkqn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zhpriyez.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lknmlquj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kxsfwdgf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yskyqfhf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rzgklppi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3eyhvoiev.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pjcftmkq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yfukfibc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3srfzxnwl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ygghzkgj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rstoubqt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3soxaehds.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3boeywyvw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vdiwkdut.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3yaznvjsr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qbgzbedl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3blegsdel.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3zdnbsjgq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wjoceqdb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kbjxguyd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qyxkdvsj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3eawnozza.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hiwxzwof.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qjnaazie.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wfkmaixk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmrdqmmk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qkqjejuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ooyyubat.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bzplsnbw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3yguetiwk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3khjyucaz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uytrwjda.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvvmkhcs.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jcldmqva.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lsocjtmy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vhmoeqlw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tnmftmzw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xbckiaqf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fgvhigfa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yzhrvuct.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wuozwusz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3skxlktoa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3siqisssx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eazkobja.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3dzyyhaeh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pafjppsv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3uzqjodmt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xtbwxwuy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nkbeamij.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xbjplgst.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3njvjwqnd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ftvzftje.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xdviltgj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bfoomrmj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3nmdwrvig.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hwbuiwtk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rhxbfyzu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3opldqdit.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3scfqgszd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bycstufv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qzzuiwie.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bnsxzoqt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jqwmvxhr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zzjwfohj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zwzdjfrp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lhwpjmdj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rbmgvvdx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhpidpmn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3myylegte.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fgprjmdk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uyeoswlo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3izofukzd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dkpqcpxe.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3nlzeoxyf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3okblmgyr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3otbumaoh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lynpewjz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vbbvyokl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bhbaouch.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xlmvqjpf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mwmufdiu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tcdcfvdx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3rnblcymx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3uixograo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3pnmheawm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3auwnfbba.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3eglfntto.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tgpupyck.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rjtacyjh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3acsubhkh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3omfupcoz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3btxkkqqx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3goivxgeq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ktkgtykq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zfmqmege.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3molsvdvq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ymjfflyy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rexmwgit.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3kqwilibh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3duennork.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbykitwp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3onovbyid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbijnxqz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lbrnhvdf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3frwkgtxo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kfflczop.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fqtgvpvk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mdljxsuv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nleuczik.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yrphilmg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hppqzwun.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vcprkafm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bgybidci.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3igyurhlh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3icdnlcuk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yqikqddx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ffdlrvxv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ipidxjty.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nigmykjy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mohgosch.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3skheapbf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qmvmfnmh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ozfqtxlc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3exookyli.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ubljmukm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bjmclltx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3krvuojha.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3uglikyvu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3txrcujls.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vlopybnd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3roiuqdpf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbkppoap.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mbhihiuv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3auagkcvk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nseimldy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ywquxiim.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3vnzrmkal.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydhnsszd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3leehoqfa.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zaigplfx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pocrfhpl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hatvyvaj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bmobifxx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mayvhbgp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3uammsxot.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ccbpgesr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3diufljih.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bklutwwj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lrkvfgnx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vnerbzcp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zawqtoea.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rzfmaean.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vmirgnhg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3imgttdtx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zichketu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jjtchgfc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qdjpwtwp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hxgkrssm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3cqbohetn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3sbviesrl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3trbtutin.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kjbfgaac.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3gsghraok.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3oynobjav.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3goyfxmvf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gzwlbfsc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3edcafvyh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3sixylwia.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3eoqvuonw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3msrhpcxo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xypozohm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uusjxhom.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nhlrbdzu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ixroewta.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lgyxvxgm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hduharxg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3svwiwhbs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vbjjwjra.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fyjmihbs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bzqfvave.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hjlvmztr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3leijknsc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yzsclniw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xvqnpbii.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ybtwpxty.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jjvdlmmh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovzwvqut.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3hdvvjmap.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qyxkywlc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3afkjpyox.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kqjnrsii.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3deounnde.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3igokenng.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kdjxzdkg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vvoewgjx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3svgqrfcx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sdbwgwyg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hasuioun.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sowmqhpj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3btbyrsrg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xidbhdhu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gtcavquh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ziufefzv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wuoqoode.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3yumhmlka.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3swqdzgat.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qjpbdheb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fixwtpjy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ocwdaulb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3idsrkuwc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pcvmenuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjvdkqdj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3uaisfgvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iesicnsz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jrhqfmsg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ilokzjda.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fzmncktw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jasuqxep.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jyptyzfs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3veffxzgi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wnlbzsfm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3vieljwqv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ojeyehjk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cgceqzed.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gumwnnal.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3utsupzrr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zzgomxjd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vcrksdcn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3sigkjink.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wurnjfjp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3symggrdg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3dfzbjqsf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3couhhpyo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mhqknaiw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ijvpyqpy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hxklmalz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3exvwzxah.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfcyzjqj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3dlqohnsd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3whuijngw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fszvpzfd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3whuqmetv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vywwxbap.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3xlsrkdaf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bvfdswdq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvcurbei.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qtcqoklw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qtemariu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ommhhviu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgeimqyp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3uwujhviy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwyxvpp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3aipyezok.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vrivfbju.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gchahfsj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3nbxwovar.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vmifhgmp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rqqqhhwm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jgxjruig.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3urtaxxfj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nxlgtlmz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ytpxpcwj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kcujzcfv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3liwgkgel.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bzexnrxd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jufclvzw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ekrxfcuc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3fgscmlpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxfipbkz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3pfyvdevy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhqaoqqo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vtphkklu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cirugjuy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3azayxpxy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rmbchwam.html


<!-- 参考信息 -->