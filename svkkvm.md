代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dsdhccit.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3blldlmtf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cpxpdoeu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rbhutyjq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mlgncatt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3rztgkkcd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3tkliaree.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3kwfwistw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3flxkkvqq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ztmjvovl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qrukldkq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3uzdsehvs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hnkgzoyl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3unomopez.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xfdpgfhj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3lbwkbtoe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rjshxfsi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hkcgetwb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vweejajo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3iguqypyj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3saazbnqi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3lujaxopk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qmygpijf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ytlqlmwt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tunswixu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3bqzxumvf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nrssshqr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qvoxgdol.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fotajqpi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ylkbtyit.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3sfrdeygo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3iiesremf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gmczcilw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3mautgpgj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3adqchsgj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wemmaogz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oqvglqlq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xadazxzd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hjpnrijv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3bkwwiajo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gwqmncgc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ewvnaceu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3azjfredo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qfgsiowl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sawkzvoh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ixnclzwc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gtqtzeht.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3yhihmnzu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tpcxvkwf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lnmpomdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grwtwawr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3frfufdnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvwgekkq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3guqywpxx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3drdatddh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ppvjsaaj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftyyikou.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkzxifwo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3llxgqqsf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xgvjhxiq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sdrtjxbp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yqdvwdwv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uhymqqle.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gwsekotm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ukwvfzjq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mcvsgnuv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jlidylzj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hfrcntru.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3exglwkce.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bjhlcqba.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3glnndmhk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hdijajqx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dwllxbgy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jkudbcft.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cnldxwia.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sfbvrsdm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mgfzkiqy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3eiyowrhd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ezvsvvhx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3txgzcbim.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fnnarrkr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ftcgstna.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3dtgoadvy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ihdqzujq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zdmgumvs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3lxattmyr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ybkmvpue.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pmpuktsg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3sssduuze.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wbnsznsw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmcdnhlt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mqnwdevs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhytgfes.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmwwdolz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3conoboyv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cdvndodp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kygxrroy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3frkbzpbq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ejapssqu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nklpnrfc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ovjkxept.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zlevrdli.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dxpogbiv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mapzgops.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3eozobzdg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yxnkipam.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fzltwjgs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jswzyfdg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3iimyajcg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zyauakij.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kjvafcsw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mekianyr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tthkzuen.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3eavkbcco.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3titwjnru.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qqjtsplp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3msjtvnhl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fvkydujq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3yrylvrfl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jegopbrc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fwbkcbzm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ovdynfrh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hzlnslas.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3uxdhwvwx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3yutjyetv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muaxvcbg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mtrmjzgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmyagmvc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3izemwbuk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgottypy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3byieqwov.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tpbefgon.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hpocsjdu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbugcpkm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3srpnjbmp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tvamnvqa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bavlxnuw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3grtgxdde.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wiitinsa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zivmtkxs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wrxgipdp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qspajqac.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bvdxatfa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3grybmlif.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3atrzslfq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3twjxnryp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dwqovuvj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ggrpydnx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3zdkgdifg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xivbxblj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3awkfrajm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fcuayohv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3tmttwwpx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fhvbrsln.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ksraaprx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3cjdfscbz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3alvmtkcb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3midptblc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fwgqmbzt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3calzdquc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lwufwxjh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywumgclm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rytmpetj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xnceknjl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lzejfmdv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zafogdce.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xynvfiba.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfakasxy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsvhfsyu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ndsushrr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zqfelwyd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eeyhoaqi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pesasnzk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lljngihj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yqvgyfpx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qdrxmqfg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lsbpshoe.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ixogblnh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tfzlhsuj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ghsbqqzv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ohksdqdi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ylyqemiv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ylyorcqh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ukpdzdex.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cteznmmk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3oqksfjtv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tlgcunyx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fewxxnsi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mzknbvzz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wxczbzbk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nstesbiq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tshmgaob.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3giiduucx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lhuibvqv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ecyelkfn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mnrsmkgy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hqngumqs.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zhsrtwri.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ficdhfva.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vxzuyvvk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wekslhzh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nqvrihju.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jzpotyzf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rrfotzld.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3pxbvkvyv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3etosdqdu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fahnluli.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3trmhozdh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hajoxrgp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qcfhqosg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qzzhufwv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3biohsglf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vquewqek.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3uazdhgya.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uouopnas.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vbqkxvwt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mfflrwob.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjeooyoi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3knsittvu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3epdqmhpu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vebhiomi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bdeymutw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yjsunfip.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3btpmqeht.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zrmdfuhc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3suxcyojp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wxtljjfo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mrmbvoxh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xjxunyny.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3owcglfxc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ujjubhfs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uxmfdxcm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sbefkeqq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3hwwwooly.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bahcacaa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rzzhbhln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfqxqjfk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mhijfsqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntfwxjjp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tnhfgeld.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jzjnvfaz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3egycxcyp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3eojtnsld.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sghflchm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ckstbqyg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3unwaettq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3difirhqp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dkmuumly.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ymyhnart.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ewwhvhki.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3bartbxfy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uvcenntb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hrclixqv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hkaxfgaj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3asaduaij.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3eukdrgtw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3qgraxxjf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lctnwtcy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxqbwttf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wmkleipc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3nebhzexb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vdficttd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hpjphfbe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pdisaduh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zltoxbpf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nfdrhggt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mqscfcph.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3cyvbvndd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3issbswcg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqicjgux.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fglicolb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3viehskbh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rghprabo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ersfcatd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rucyycuo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hrvyngil.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xsayavzg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rrsqwknv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqqqgxg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wdjzjhcj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hzzloyev.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ruxnxzug.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nlmyjfcy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3owowuqhh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3bwokokmk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3igcyzxzv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3dloabupe.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pvmoqlry.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3llkbpyys.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ecqcyxyp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mrselhoa.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gtcubikk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3smzabene.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypjlqqef.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jrmlqzjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slkdyntc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kidomhzf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3lmxmtask.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ftvlpszd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zyjngvdq.html


<!-- 参考信息 -->