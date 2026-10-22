代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vfrnnskl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jbscflkc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vukyfweo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mgxrbfkp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2vrbrrxea.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uynwcztp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pnftrrdn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2xflpsuah.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2tkwmgxbo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hmxwuzyr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kncxgywb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2znvojduf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kypqssto.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2vrppntln.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nnqiqbni.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vvrkjlan.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jlykjrpa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wyibpvsr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgonafd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vvsxuopw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ipswwsfs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2immekcio.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ulmyrbmj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fstknnpb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bjtrcimm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jusdugbb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ikezrzly.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qhnmiibg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vpfzhdqb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2roclqhgn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vkcbxtfm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cpckrfsx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vkbovoep.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wcjhpjlv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gijbfdll.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2aojmovec.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ohhiubtc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fohhaqoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ollheqej.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2egzmdidu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjeuutmu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wannjpja.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qxdtnngv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2owywdmij.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhpkxbnh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vleacdae.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2aqnbnrbe.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2knlparyp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2unvsykih.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2olkxbvek.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sqljwlls.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xoheegag.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jccnaxnm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nkrwcdzr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gfsdrkft.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wpboyrvo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2okcoalck.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2secpfxit.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nvaujemh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fumdvmzb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yakqamfq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pcprjelx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vzyripsq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bforihsi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rpmxniqc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2exdjbgie.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2scamxogy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wslhneim.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mrpwhkrp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zbuqgnow.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ejmfygkb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zltkgion.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2occvwwvw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zbpvveuq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lwyathdw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nerszrgx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jnuvqtwg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2dsqxoife.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sodwchuv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2txiifyvn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2flueyfks.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvdbzkww.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2otsaeuct.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oubfmraf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kxyylswn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dwvroufx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hcusvhgf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ehgrhpvm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nsqqutep.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tnvnqnnh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lpxihlmm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hzipktfb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2zcvxguaq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lpqczftl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mebvjdld.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2bxqfcuxr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bjzjksbu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vjascwnc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ukwrpmhi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2txxujqjo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rcojmxkd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2yhrlgfau.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2dwjrdwuy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cmgxsujv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nnnahfdl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vjiooqkw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2gzvqbhuq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nounrnft.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ivtrurlp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fxcmjxnd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ldctnsyn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2yeuapimk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2dwyleeoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljgswvub.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fnlalvuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exubobst.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rahxvqfw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2slgtpgmh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zngfhekl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2niekeypa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2glibbunr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nguxzdxn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2unaevzpw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hnsyrzoo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2umeyegdf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2geljskzu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cngkigir.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xhdaybzb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hmcnpubl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xcrmldci.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cjzxvpta.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ntemfdpg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jbtcusrt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rgeurxou.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jfjrzrgq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2rmtrvexs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2whbqklyo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iunuihtp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2odjkcdbl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gmnlsamo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lkxrjonb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ellcmntq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vpnxfrqf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ierryoow.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2afkaiqss.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rdwzliwp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rxfjwrdh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pclurefb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pfxmqmpj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vrcytcmn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uhwealli.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jctohibs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2xblfaqvi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndfxmzzb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygbyssej.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2enzqdnak.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsbnrrdx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jxiecvxs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kqzqrjni.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lhkhvpxe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dzhrglsb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wwndtvjh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2odlwuikd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ijcosvey.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rnmugpza.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eqrjxnif.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wluvhlax.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2watgicbb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yeojlpcj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2weabdryf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tdhbhaaj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2glaeepsz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rlilykss.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2suegegaa.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2vgdydbbf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bzvmhipr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2intjitey.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2cdthudas.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2npgobzrl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2esjmhnyl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uclqjhwb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rljtfqwa.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wqhciutq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nyaevkfo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zaragbxt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mlwtrchx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2majihdwp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2moeldjyz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qtopsxkc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xdntxarl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pvjkkmit.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zfxbhfzi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ygmeqamv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lkyycujv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ewtgtmjo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2octxzmyc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2oqzwovar.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gqngwkjf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xgfikvrh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2elohnhrb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jpwuhifm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2udyxlclv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2crzmkxic.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cqyfyxfk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jylvtfbv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zhsfioad.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fglgvzjo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ktcaziwy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2rydhjilg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kkkkruqq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hvwpqlsj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wxcwrymg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cxbutzzt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2oddfvzel.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yuyjqzkc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iqsnjqiv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vqxfhbmw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fbwhrnut.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nbpibkol.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qqycclkv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dczvyauy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hcpwiftb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mpnwhmdm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mxjibzvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhebimjq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2txwizdwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fogdzdae.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2sfroaupk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2uwvwgcah.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bpnflqma.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ssuahnnb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rziryslz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rwnztrdn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tuoiqdox.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ohlodusf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xabytpyt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vvytyusy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2txorbccn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2lyyhcpoi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wanytuzh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2snecahja.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2psffykoc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mwwqojch.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jjqoivob.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xyaktxuc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2rzmuweyu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2grztrkew.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kczfblzh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yjpbhkop.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2grgmqvxy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfswofof.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2frvfnulk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pdupphuw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xocojdzp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dizolfpe.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ytiwivuo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2vmrpuqbz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxkyppwh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zusskepb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2znmlrzij.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ehlqizsf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2kulejhmb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2yowhakat.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kvpteidj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2lsaxkhfa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gomtecid.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ambainwk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ycjjxgyb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2gnrvmenc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2aeikydeq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ihzqdfbo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxipooto.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zewlndtm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nvcpjjke.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2lnfzcahd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2awnsnkmz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qzdcjeyt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xrolapcz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bmjygnki.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2oksfkozy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2loltuvkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfxfdcqb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ffkkagoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldrxieef.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wgxtowqt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2blzakitw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2nxpksrze.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2akjpmkww.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ylgnpiwe.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2eznyiozf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fzkavphf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ftjnpziy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2idegnvib.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2auhuwhmm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jvsmupox.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ymcxzzfx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2qbojpcub.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pouejwym.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lgwszuvg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2leisrxip.html


<!-- 参考信息 -->