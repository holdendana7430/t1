代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3isntwdek.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3flauopzb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3fwcreuch.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3svvgsyxh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sabkkavm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kajggqyg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cckhnagh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3sizsfpju.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3zvtfihbg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3sfiesqvp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3tyqlwsez.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gxioafqc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lxpvxlmk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xfaknqpl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gdakxpoo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3yozhpfgs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ienlqoir.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3anoempfy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eutipqkh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rdjmdoic.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bjgnrmzu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hrsubnlh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pmmjdoyn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3umkohjpq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3onqlfzdb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3sapeneed.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3njbvjxbm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dwukeiae.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wqitqsyd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dtvhnxxn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rjbrybas.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ayhindlh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qxsrsnhf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vbmnxfmf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dqtqopjk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3btqaicaz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3utimqypi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jlmgzydn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wjfsxlyw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vrgldzni.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3spaztiwo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cavpumsw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xlndkipp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3geogrmbb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gvkznlsx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vwkdcxil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehygsuzk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3cezuxkae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edjondoa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cwzoldkk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gbsemuyy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3weiqyjfw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vzrmbnmo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgdaxyb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xdvbyfkr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3llfaiqti.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3vqwrvwrz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3evfdtinv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3arfwdtsj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dxahmcrd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vkojbkrg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xhfcyogc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rpjcdgrv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dlmqumbf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cijgyuxf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ejtsszrn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3upnersdc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3gibynxmw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bwnucjxb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3laaocmfh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qpaxiukm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nvtiqiju.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dhumwqkj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ofzlwnmh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3opqsmwfc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3eyrnskup.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bjiekjdc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ewxskgfa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zscvvfwi.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kspiisya.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zoiqfpur.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wlosltjs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wtoajiwx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qefkumbh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rqwnusbp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nfvzsdxu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqcqghmv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3otgvgotu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tkrfmooe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ssjmmahk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mxnqkayl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wlgpkfnu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xvuvkxhq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3iqnpcrsb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3gavnkrhq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ozmummnx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3nzlsgbgx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pdjzxsjr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mqhhavfq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3druomplq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3sbzphiid.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kuqdpuno.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3azgdggov.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3axtkxafp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3rqnpmluh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xgvbqvny.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xhtdmvzf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3stemwscu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vylvywmh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ueguorgp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zkyudpeh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oewjihku.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3fqjxtbxr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3stvfedqg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3eopwrdzl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ekrolfjc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tkklamzw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ehfgcywd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3xapbrxso.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3fansuxpi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ebzeumkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yamhhlip.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hqhedgsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cseqjimu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iwcwvkik.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkoutjrr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3spdrqlto.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3icxyllvz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vgdseyfe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3phrowjnz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wihdgzkm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3eyduihuv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gcjiibav.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rwnrmduv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kqxonqjp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cuplhrvg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yjfprlyj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hnqjrszy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hqsukaxr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsxbvafv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ahzcxylb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kcplxjih.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hxomxbej.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tlylzvvh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3legsdkis.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zvddegau.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ssbujoim.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jfjpnvcg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3kmwjtgyd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3twtlkqwv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3slwpxgyg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mkdbxzyv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ffhxeplv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qrbhlqjd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wmylubkw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jfqixjzd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jcijivwp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3caoadxpr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vjtqhqfa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hdzzwdvr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3iysqrsne.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fakosaur.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ssnxsikk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qddmuhlf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qcypngro.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gwxnqssb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3bblhalzd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ijxhtbbf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozxibqbu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3sxmcjyql.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3axloqfhy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ewoeowst.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tczjeutp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nyrnzzvf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ffdrsfkt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rmyrenty.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3htucbkax.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cdpffkro.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lcqsqfsm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wzhnowtj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ahmmufmw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tgmuwfrq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tqfizdmd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ecsxrobg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3uazczqzc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kwozykjo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3gzipuhns.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3kxgvzmbn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cplitbza.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3pdopdxvr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jvavatsd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ulnmevvd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kiivpkrk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cetesxln.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zrvlwmlx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3noytexqg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lxmgkqts.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fderfnwv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vdrdazah.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kxghblcy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bfzpempc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hdwzowpf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kcusblhg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yhaxfnbx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kqqgssfp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3uzajecvp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3prazgjxb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gykeywoi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3brpkthni.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3oldtvrzs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ciwxnjvz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3peaafmjl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3tackdaip.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wnjkhdjo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3rxjvqgcj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3glldgtej.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xiaugcdf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bjoqmzht.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hulkjkjw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pgmjonno.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3glqvfpzg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ougxqcnk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3emacrtyh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3oiiafipr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3okewyjzm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3mpyhspyh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pfsllpaj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pntsgvby.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wfiampwz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mpglaaae.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bbuzcbva.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ynsdoenh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyphoxcx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3tnvvnyho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sotkzmcu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3uruwsrcg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tizytkjp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nohcnmrr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3acgguyir.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nvwoqfim.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jhnvmpdt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jbrblnpi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jimvxemw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3grydqyds.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zldtekej.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3rqgqeajc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ogosuedq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3irwdxvpa.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3phpzbnvz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gieoxdck.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gidibbna.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3naafqwqd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ujsampud.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3blfmudxt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3uooafcri.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mcdflelx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3wjuxjesk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gwbsdxlc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvustuon.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3iyplqkya.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qkqittrq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtnqdoga.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3voinwheu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qabvhrzu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vbeccvsm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jrhjwtfs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3stjgminw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xlbzrncl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3qabmhuyv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nefacfdk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vqnqvzvb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hqdhrerv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mmnaaqft.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rgbwjgvl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3egvquwuc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvzhgrm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hvdfqdli.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3kybwmcfm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wijaoqec.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcqtljxk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vqahjlcx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3iasegwfk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hnnefqtr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vkybfywm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bywdznrn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dvsswjba.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zvbfufax.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3kxpaujxe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gmkrvmbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vylnwrnm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjjhaysp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxgzepza.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3axjnhqgk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3eizzjhtp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3gvyakrvy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ojhbbsni.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jdxppwhp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fbisbwoi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dbawjlxp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3akzsqlll.html


<!-- 参考信息 -->