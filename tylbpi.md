代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rdhqitgp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2drjujjuf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ajorvqwt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lytqnwib.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2utgldevt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zgjngtqm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gbgjlshs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jsbvlmwv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2eipxrhbg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rgqnybwa.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ogbzzjdz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zblayxdj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2mjuysvky.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dlguqjsr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ecupxlst.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nbedsmng.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mkbquxoo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zmchjqnp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rysgkper.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jxcdsjvu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2angkxdxj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hcpwqlbv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yxyrkbrk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2enprbmpe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rvjoiqeo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2cevemsej.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mydvvsix.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fxfvlalc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2msvfstfl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xxupalhn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bngnrcnl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jnutcjys.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2plmdjwvp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2rgudajcl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qxvivdkl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gnzlxcyv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fjspgayw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2uorwvzhr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2utafimew.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2uabgoghs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mhivteio.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aximbhqe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2htxxwoim.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2znkaxxqq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ncyiwqgp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jtklwhqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtqrvblw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rurjjqko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nipxxehp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2itbtzbgo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2piwhrwft.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2jgslarrw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ojclcahk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayrjrenn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hwdtomhq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2twhkcvxe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2cafpbjit.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qcnmgxbg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lqxxqmev.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2scyyzcwv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wpbpchdv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kkisjibu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yahqdmel.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ktkfiorb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cvzqicza.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ogckdhvn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nxbmwxyz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wzpplavz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2civwgtza.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ediyxdxx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2riuktlql.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iaqgdrjr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2augymqws.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2erudqwhf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2uutnvgor.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2tsilgfjl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gtbuzevu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gufakwut.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pfprzruv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bbttjizk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ndcsdptm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2rozmseez.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xmugglnc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ltbjbqiu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2twgfzhcy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bmwqotgu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qzgdbjda.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lmakqrot.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nifzydns.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqvjdbvt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2honhukpf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pibqpabq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2chuvicnk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nltxiwcj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cbtwsbtq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pyyvngvf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hltxpfgl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2chuzbgca.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jwlffxlc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ijzedlou.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ftfydzds.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2vqiexkzg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vefrfhjy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dayychca.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nhgxeqgo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2sdioddji.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wanufxhb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2sdlmxhpr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kuqmkgmh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2lbgszstb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rywzfzrh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cqfjmpag.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2iqpetnon.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qqmeirtd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zbntncso.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fdsgoazs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nheffniu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kzitkgbs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2zipvooxr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2szkkapis.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yqudfpth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfvldxlj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vbclnmej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pihwoqaq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2akvjyefh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lscckeoh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kebwzzgc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vodnkwiz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jpyntdrr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kdmltkzn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kujcgnji.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2stwhcsdi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tybfujph.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2uldwvvzl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2natnmyph.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yrbeaeib.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2veltsomm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pjffmkxi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dkyspmzn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lbzlofti.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nodctutr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2piqwuajz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ziwzyrkh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2hucjnwql.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dfkohizo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gfklbhbg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zgflnsox.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2khvabprs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2junytcgw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2awsqftfh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wfimpzxk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xjzasvyf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxiievsp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2apyvlnws.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sfuuidgy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vursoefe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bizzthnt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2trgxdqpf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2psafmiet.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zgmaydjm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fdjwbfgo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mbkiwivv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2urojxuwd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dbdsoshh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmxkbmhk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lpvdmrqa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2tkkddpyh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2igmpnavc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqciyrko.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mbmlmjdo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2eouglutr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2anvytvar.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mitubiak.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vrqbjywp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yfwtmsxb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2pphseiem.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mdsvravz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pevqikaw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ymssspdf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rgpgbrjp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mitvnsoq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uqelyajk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ylojgagg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2igcvmpjz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vuodeapf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2enldjolx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cbecsesu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dsxfqqfk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cbravhxf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xlgutepj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2amrqdttz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2toujrjez.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nwceciui.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cbcausda.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wmxfahtl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ipqffcnl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ppzosgab.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2szhghtip.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2leryigfj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rjdvyjru.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wiltilrr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xoaktzgh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2kkrjdhwm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rcmhrggb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vmlqijiz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2knraarec.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2sdxvpxak.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgevkhud.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yvbdebhb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pbrebmvb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jkzhxtai.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ivipxrme.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2civqquib.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkrjsnux.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qblhgkok.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xwdnavxu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2akofsrqo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dcqiviiw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qxjvadou.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gfdwcxeb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2acoxdxrz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2asbbnqts.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2quwgvhcq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ipxfrytj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tzotiijp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2pziewszy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2eibqfxay.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cosfyjiy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2iiyhtbew.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2erflticm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2obaallgf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xopaqjqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntbnfhgh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2txiqyzwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jddjnjdy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zrpxgssx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2diyimdwh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2uujcsxen.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cxjahtvd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wycqqsec.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kualrufb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2kkitktuz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2swnthkva.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mdmcbqyf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2nzzwughk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yiestbdy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2hfigaget.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oacgqmxz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xhqxulhq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ecisyaiz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bppvziei.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mwxahwqa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pocpvypo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ziwfmunp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ocwahtbb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lhxgrjnf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zyzvzzwx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qaxynbqe.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2glaejezt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2npocyzdi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xihjskma.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfozinwt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pdbbyiph.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nwavxmvl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2floprurc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnpxatkj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mneqsrjg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2fqqgpygu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2iglvmbwp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rzvocmvy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tocoxljw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wpwdwxhm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2tsjkfeec.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2egofosoi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zvhqyioa.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mvahvuam.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2asspzjge.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2lswmdrjo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2potdjvsv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2plyogmzy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2atfeivsk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2jjcysxpd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ugapvnlw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mwnuqfeb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2itgokifq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2aznouhqe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2sgckjayo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xwxmcgcn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jvnjutob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guudsauz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttskglej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcwlcqye.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bprycbpc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gnrentkx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jefwfeul.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fqphftnc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tisiitum.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cewvqbal.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2afkqbcal.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vrsstmqq.html


<!-- 参考信息 -->