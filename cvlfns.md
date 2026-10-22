代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wbgsuurz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xiiworip.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2sewtaxel.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2uhkmzsbt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2lsohnauj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2farajnli.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2klfkydnk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jyctmhuq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ostafmho.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kfrxzshg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2shawxqjx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nyurgxrc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2viexbqnp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nodzmtbk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eagqhgnq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2clsuetbq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wdswdhbv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bsntsmjs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ybfozwzd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jxcmujdh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rozlgaxu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jmffuglw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xckmfkrw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nxjlbmgu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2flhzoafm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ipqujqdc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kvvteirc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rhbtnaok.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rbzfgaho.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ekhqafkf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pktowcem.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2phzcgmjr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rmpjzxxr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fuwxxpmu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kzcwxczf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2kofvmlvv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jbcvkvhy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lymdgwvc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2cszjvlbt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zkyyjmfk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2txrttzro.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hhdfkzit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oumqymao.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gkurgrpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suqphccj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kcfzgvlb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zpxbmnyp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xfcjtjtt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqcaqptd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2touyqywr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dyscbwox.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hixrkcfr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qpkglhmh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2drixadti.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2aklpotkf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kplczuuz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dfcrwctf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2odxuzjks.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qdyulhxl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mjjufaxx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jnzrvwop.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2anoeaqvn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ppuvojvj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2amhbvqfi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gubndslg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vpgzmuhw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lezjmsjz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qfacwyvi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vxtcphzj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wmmkegub.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2smnmbloc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rbxwtjws.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2whvwdoyl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2prgczeha.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2csoavihx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pmoajpgb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2livowifk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2higllkgm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hhuxfrho.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mdlbkwhj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2eyhsuser.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fssehipz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jvebjbkp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kuuyorav.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmsusmkn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mieusely.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ftsqgnme.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2izlmfhqt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dsrmmrve.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nbulxdgl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2galhqoyr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hqboqbwh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mclbokwe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gzykoubu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2azdpsmhw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2oisdjznx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rtygwppj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rrrcgqbt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zszkkalj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xgambtsd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pdirhqeo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ewncrlxu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2amgolcft.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sogdfndj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zumoffyv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2yfhuhusc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2yrxglkdl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jvpmvnyr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xjaovwbk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hkyucwhr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ldqfpuja.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2epmswggf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eleowtjb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2szglffzc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2scfpyodb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2stdqegyk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2quvbijfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djecyzgk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2plnpeszr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eebvtzna.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ypcwenwm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uspiihzk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uwfwtbhs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oxnpvsqw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vjatrbzr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tupbdeio.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2prwwyzvi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zqelvfbm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iawuxfci.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2sbjyferq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ppmjtdtm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fuxkvuyi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2akvpxkhr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxsjlpr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vethcwvz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fjhhbppk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xsyzbsct.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cbowluuu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bjofzisa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mgmnlyks.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wbgebiwb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dxtrvpab.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xughuwbm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vkmcpena.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qfqoaltr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jyiizsrs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ywjuoihv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rjyzdpum.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqoayrjx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2owzypbzb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gehycvyb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jsiykuls.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrhrmkrd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2itjwhpia.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dwvdicby.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iyjzzmhc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2allnrfhk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lgqcifdc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjaqkynv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtwxhapo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2skptapzb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ofjpzxke.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2djapkdkw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2xmamrivh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqdkqaja.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wzhnqpbq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vccjjehq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cvxbchfz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fhmlbaqy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2enbrwsno.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ickwpvxg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2aenchkim.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xzyqjdtv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vtnjyqmw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2sbfunswp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kssooncd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2uqyfijzm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2watbraaa.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2exrhutyu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qlbhjahj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fkdeazsf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bzdcrnmy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xfwpyzjs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2swgyjtpk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rptpziau.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jknzdovz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eokllrld.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ljzjtzpx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jysdabzh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mtptagqt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2izuklpwk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jdzetwpx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ndelyfxb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2krwydhfz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dylnjdvq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dhanyefl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2jttdelno.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sascillt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jwtucojr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wqnnvdpx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ouitflax.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2citwebcr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ewylbgwv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2whqwmycg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vtjnzamc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pgwjgsnz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2rqtabckq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2uiusnphv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2xllbhpqo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uktuezjr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xjggnuan.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jhllemfs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ulwglctb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ynjbyfzj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qyjpkczo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ramogbqy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eltxdsrd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2aunbparo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2efvahmmi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dkybsbni.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2acypwfba.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2pzafrkmn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ybnunori.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2apqxasjs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wboksrqe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2hsommksk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lhsoqqhc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pvjqehzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdqetits.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jkgqgrbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aniayglm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tynzmfvx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cabfnkan.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qdudxmxc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2fcutdfcg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mbvkcplw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dbqtiiii.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lfkdzrxh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2pdwnnnsr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vjqjojxh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2coesvrcw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2sdqokxsw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vztwkfzy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2byqyhlco.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ushsasrf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2olwzhndm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nrmpgknv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nyjfeqdy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2bbseannk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2oteqaloe.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kykkouud.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pblzeohh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2keyngwkz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ofikayoc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xprlovyp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qembowrk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2chwlocfz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2snntrsma.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2juypkcsq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2btspaqvs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ioxhivxd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cluxstit.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwobphad.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ontfjkqc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hjbeweba.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2betiiwsw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pttoupvk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jmsxjaph.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gjmjalxg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ebwqdlgs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yelzlxpk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zbkytdec.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qfijyfmp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2czfgzial.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2smgeerri.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2wyejqkka.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2klabjcub.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2rkaeobqc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vtwjrxbx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rvwepsmb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rfofafzt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ysfsppbp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zhxagegj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2tagplrxl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2injoycds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xllsznjo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2tehzbaov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kckwness.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2akjbcdbp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2yvylliez.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2kereovlw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mhwnhvjg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2boflojbq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wqbgokba.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ktssigjo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ovydmcmz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fkkmzjvt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bpkyflew.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2gmuyjdqj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2combqtwe.html


<!-- 参考信息 -->