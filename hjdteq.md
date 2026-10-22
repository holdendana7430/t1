代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ayvgxaar.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cwchispv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2eelwngmn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2vyahzzwd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2afxbnxnz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wqlolqrn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xgbqwomf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fsuycxpj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ccmfulcf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zrechabx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hnsspzoz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2dhtnfslt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjrtjfao.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xlutusku.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zoqcoulo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uxiazexz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2geuenxuk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ktjhcgyl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nkkmuzqt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2esmkwfiv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kfckcvru.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wzyqqqwb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vlyarnwb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gtholjze.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zbsidvaj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2odyxrdqc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wjuswzyn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tiwzgzgl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ycprbsya.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2dgdxfuom.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qwupbhrs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mftpaebv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qxuhnamk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2uofysjnk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2glmnksta.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hdxzuhcn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uxzryucs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fmnfxcgn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2migtrhmk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bnanxlud.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sgmctbgh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ekzsghwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jagaksmg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pdmqtuxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxwndohf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jckfrlbj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2srsmgevp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2uriirzzd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxvzwjrt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vmiycyht.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2synehnbj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vfdhdkgn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2itnsgmnc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xvoltaao.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sjzekyvo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iotirgee.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jgrfujrv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2slgayjnl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2joyumvhw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ixqvsaqs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2otpwjeya.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hdifnuyz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xnccwmsk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2pnwefawj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jeebadhn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2uwwjtkxn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vzxncusc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2flzxobky.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jimfisol.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kgibsmde.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2prxctynh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hwaltbyc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gchcryxs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qmyulhcm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2csghlmhq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rldagdlw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rswkdqqg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2bgdmvkgd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2gymcsorm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2uxtbwksy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ohrvgteh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jcbujhhd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nupzltqr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qknmsffo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhiayiyo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qstmlhvw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ikfmglwe.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fpqnxjpl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cxoaylad.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tpjwjrcb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ugqfgbln.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iioegrkq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xtadlizr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mvaliejg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vztyjqqf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zpagzyvj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zueodwoq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zkeipazq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2govrqfue.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fzfawebh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zqmjtiir.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2relvbmob.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jwbxzutu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lykquhfs.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ueauefus.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2spvfybpx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zhtersox.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rrwqyfdw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rgbnprhs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ksspoahf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2febkhesp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ixpeyopd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wckhdvad.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qzcgiebv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kmjlrfrf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fmswsgnc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2mghizzzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zweyfomf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2upibsbox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubwykfro.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jwgwvukx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqxanao.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2luuddwsq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tickjzlj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yidtzxjh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqwbnvtg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxkomimy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2uafeuhpl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjlixejp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2efhmxzpv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jshbmvzy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zlroaisq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zkwxrqze.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tebkjjsa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfpbkec.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jnrmjjlh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2aahmfpxj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iypbjlhy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jdueltmw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ryxfmxay.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2dhqvtobp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gcnzdpoy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uqqnexni.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2krzzofoe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ocvkobcm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vvqenzma.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2popekyjg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2bjnaxivu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cfsikbsu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkdtsffb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qaoaicmm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qrpmjftj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kkwbhirt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ayffuurc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjwueaxu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ylombftm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2neuyzdov.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pgddcrvg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mmujoduq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmgrpceo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fycwkrdp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jwggcrnm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2pxndidym.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tuyblfuu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pqskptwq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yicvigdl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nqrbwmbl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zpdibqqg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iznjcaph.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lvqxeaxz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xxxbmvsx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ehvjbbns.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yvopazjk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lldzlprh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bwtkjqcy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2uljaohpf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qwpqjrqi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2pqwcwuzq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nswgvzqn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sjismrlm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mselopxu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bbproiuz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ubzdcydo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2uqlmhzdm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jatpebtm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bwnlqbjw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cdkxawsk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vvjpzirm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gjmndwmq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jabgztwh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qizdmwio.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fbcuslkz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xaeqhkdm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jwcwmvzl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ujwjaoeu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vzegilmc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2flwuikak.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2okhqinui.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hcpqpmzn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uycbfffn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2cskheytt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2eifhejiv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2znoxhuoc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ldiitlei.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mmdbfrsk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ylxjtcaq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2whvwsiyr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jeopwrwt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ydwwtbfd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wftqyimn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vkhrolab.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nsaxtole.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2tymcosge.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nywvpmlx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ybrqxfky.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yqeyvzuu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sramtlds.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2miecpwag.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tzfbpbjc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iyakahdj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dvikqjqo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ktagkyel.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ehodnzxr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tgamwwev.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kcucgjjv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lcxnvivb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qffzceps.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mawipsjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ullruynu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2elrsqwvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uazoxezy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2atjdqmvo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yfdcdjqs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2icpmgggb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2yhsrciop.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ipirpnvs.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2beolebog.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ttwhoabv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rrybrlry.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pwghxafk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2kzqzofhb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rnnimvml.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2fppydize.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mvywkdii.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dnoxnzwo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lwvxyehv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2tvliyvym.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2eaziiilm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2kjdmymhi.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2wiufwsyq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2txmdnapy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2newzfxzk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dliadxrd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ffsdgxsz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2quxmyycr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2kmmkhrev.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2txntuqpz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqjknmua.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ahzxkznn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2irypdgbc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dusoglld.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wuwmsawl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cwdnpqyo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2iyxspscq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wjtpwofb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vplehihw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uayqrphz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2pygfzslh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xawgvxle.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jrhayqmk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xxhyjfey.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zcldvxmn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2olssgmlh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zznndiin.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tzigigwp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ospttpqv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2nrphwqkw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2erkxxhoz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ectocfwv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ptranwdm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hdoxzgab.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gsupjwag.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hawlmcsq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2uccmkhod.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gnkxgykd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qucgmmpo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xpmisdvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxrcqnfp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jydrlrnf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ssgxutua.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2otnifqrb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2crrrbalg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2butukcvu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zixvmyxc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wpgighyb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2gavdbuwt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lddbqkpm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2iixgpfex.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qphipayf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bjaowolt.html


<!-- 参考信息 -->