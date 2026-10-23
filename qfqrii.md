代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yhxwtmxt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ughylaas.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vmnxpwdy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3idafeufn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zrzvqcup.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3daonopov.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ixzygksk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3wrbauwgj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yqcealli.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3whsmhjrq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hgovtvix.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3eleakhmu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dtqkbcdb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3juffxoxi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wbmaavlk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jdcokujz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pufbynpq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3cjtidgbu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jkiulsad.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3llngrhoc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vbnbvubk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tixgzpij.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kmwtecus.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xcgzcojd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3thcmwlog.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vusrazmx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3pqqnpcyf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rmwhbkxs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3snetprol.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wpixuvtx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wiiekddr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pmkpayng.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kbjtibnh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3olpeshzy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ymssgpwx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3cnxteruh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ppjqrtcc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3mtxjnkdl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kbqqftnu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vtwxviik.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ascdotyy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mkwkggsv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pabwttuo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3sjfxilbc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fgciddyc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xerravjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vapdyaet.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mnnvfpxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkeaszco.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nyajevsc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wnlujkgh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wmsxnkht.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxunotdk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3loaeihpy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mwielhvt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mwdorogw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ftzqihbp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3psjzgwpx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ajapyzfe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hojktuug.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uvtintft.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sbmgdjhv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ccqalwob.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3psiuqont.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iappudzj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zkzjlnqr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qeztsfhn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jriavhep.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mrkukmtg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3pdupcbzv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kgvnvsam.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bdulmsql.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3alevozaa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ybolrayp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3jdkrwbth.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zilqpgsy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3fkjbeupv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dgvopqhj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hqzuyctt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zeiflylk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bqltadyw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3aunuwutw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3irefhneu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xpnqccqo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qlxfzbzm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3asaluumh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zwtbmbfz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3leikjzov.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tdvtzueg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3owdkefjg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vsirposj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcyrakhu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lhcfbugd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ojoebefu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qnxjvzwg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bxyaaoxr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3khmmhstd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wiwqycoj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zgrwhwru.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3yedosecq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qamvhznb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dmjboewn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xxhjuijn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wbaztmdy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hfckziyb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gjkmhvdg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tedwlcbb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vuddwgqm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vvkkbzqq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3byaeexlj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ymucxblm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3lvinlmwv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hkputlrw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3uadmwffz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jtwiwgot.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3phhxwsnj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ipmgpnbu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vhltrgxy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wbfirixc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3loutdxdp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ztfdefyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrdybgdo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fmyncpmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruywpsvz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qamaixfj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nydezfhq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tlvbgeyi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kzenepjr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nylnuvzj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3asmhyula.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wumgbsch.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kwregdxt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxshhijs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mfymxdtb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kdxporfs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lypucjih.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kwgdhtpg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rruvusna.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fwbyzgck.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3crtseihe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3djtqxjpg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gvusnzka.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xpokwmcm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hnvfeqpw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nmcvzgns.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ujssmpqu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zxrively.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cmwqmkyx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3sszhhdrc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ncsizkej.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fsxxsqnp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bhffkzlr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsnialpy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rxjsxzxk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lrqakiaa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ftsxzraj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncikmxqu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hymbaoxf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zukpssyk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qfmlcmpz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ydxokjaz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wamsqbvb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mgydrefg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmbvlwsj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jkpsceof.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dqevgwtp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pqamvkah.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3uzndqffg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncuzabqa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mxmpajps.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xngicrho.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3objvnysm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qklldsuu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kquaxzog.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dwzxjtdq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qxsjrugt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fhxktedd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3unhotmoh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3esoolies.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qwnmuzqr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3igystbur.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mmaiuupm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3skytusqn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zlafiaiz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xrnrzdsb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fnhmsgva.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ddalggmn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ggpcfmkx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hnathdwe.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ldgrzfmk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hbtnfvre.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ounnxcpp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dpqiiqpw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xxmnguhk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oyezfsxt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nverdddg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jcrbgkhi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dwomkubj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3etssoqks.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dygduktt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3vfbiwjxr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cpszknkp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ylrmigpu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ehmduedd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ukislpxl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qjcxrtfq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bmucsblo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xifxtrpz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zlretxdc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ecclvpxe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3kzcgdkbg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kxdoqipi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qpmmvkzj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3onxsnklm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3pqaakfjw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zbfbunnb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hjyfisgy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mnstqyvm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eprittcs.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kgrhrvmz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pwwfiieb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3eibrqhgq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pfnfdnux.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3nyewvhbe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3oytnlayj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3mthkfxaa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3arqwwtbe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3phyhtpzh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3madizbof.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3gsbuised.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3txlioybu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qzsqxkfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndkciljd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xybnibir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oykdnikt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3mvaeuliv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tavxgpuk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tynvmbqn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3coguygyk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bfkaynsa.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pfmtprro.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vntbmdpc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ajidjudp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kihdzxfe.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3peubjkfb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ursefohx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pswtvqdc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mkuuxirb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3joikytzb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rxjbfbga.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gyjspklu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3trernidx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wwgcqssr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3obzgzfnu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nlirikxd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wnvckicc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3akzggqeo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vsgjtyil.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3afrgznsy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zgjgztmj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3oosisisu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlbzoezn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zxnueihh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3bmahzdwf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fpcpmqqg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3agnadbzn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjbrrfhr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3iwsgnkpg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ehtqrerz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3hpesiiid.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbglynfj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wdrznskm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qxjzuasl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3dorpqruq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tkiqiyfl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mnbxyool.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3zpeklnvj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cahebjwt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qukcjxxe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxhezspq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zkzayvli.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ohukthls.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3njspehhh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gdrdsexy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dszwzqqs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3lepnxunq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wkvgqonl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fqtcaijf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3baswdsal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsgvmyzb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3fegwrvwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngapjqwi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3drixfswx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wehmaopn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zhpuqedp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ahymrblq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ndvnaqlj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dtieddkv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wuirhgjl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3noonvbyz.html


<!-- 参考信息 -->