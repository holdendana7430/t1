代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qfzxehbn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rtmlgtap.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xbvpdmkb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2xgvstrev.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mprkytqd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mwpldyaw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ihuaxgcc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2qeckjrvr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2kkoesvau.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2unyubjmw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yhbumucr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2stbatftw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ziofzoeq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2rtvfclcm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cqxmxjts.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jrzaeeqq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qjwxkdbq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ydixejnq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rpkijhxt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2llktphkd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qubbcjxd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jzsmrgiw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2khwuimeu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cefclkii.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2heayturt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lhxgfjla.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2skwjawpa.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pclsxyiy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ovsrxtdt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ywfohnqk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2whgqudpa.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2nigneanw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ibvfgzdl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nqqphlqo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lgzpeqns.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kvglwnaj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zasxpbvy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mzanhopk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2dgqduapp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jdbtuyko.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wcfkbwtb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ptiutkge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktycdhhx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2nyqkzobg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thcuzler.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ggvbfwrc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aklunron.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2muzqjits.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ivtwtjqz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kfwwdzwx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dtbxyovn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2juldcazd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xfrbntgf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mxeurlqs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2saoncffw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2omrjvffp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2otervhjg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mybuovgu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jagmwldp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fskmqidc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rddisxgx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2krswossh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ayfihzue.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xeiqpmyg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iifkifkq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xjgucowe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wcrhxqru.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2leeblmoo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pynhhwxr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xewfxpjg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bmtdtjda.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uwmtqjvg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ocsdjnpa.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ryqnftup.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2tltyozin.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wgqcysro.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aenythdu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vilpxltv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vpifqrfr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2urlzeucm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ujvnhyqh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gmajgfyg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fbrchifb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wxbpjqqc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jpeeefmk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqzcxrgs.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzipdpph.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nofscfhh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkaemvyy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wixcajkx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kqvlonvf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckudayaz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ghxfkney.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mepdalsm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rcjsjxom.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ytqbgebd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2htoqsdkj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bdrjgdxs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lhfrqjyx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2hzulydol.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2chbaslci.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ttkezvnt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ocrridre.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xkdfqrgb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2opjocsdo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xtbpzvpn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2rxvxbgil.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cgxckxod.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ahcqkdll.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rflzkilo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rmesdmzg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2siiqfhzx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xqixgasq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wnadhvff.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2uccdfjto.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pefkinix.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zalbnjur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycvxpzrf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2iehepocm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvkbnamr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2giyopgkn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pvvjggvf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ksdubcqn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rsavolgn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ceetlvhp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tyvxznna.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2utsisfmm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ygrssfkz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2moivruji.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pethbdpq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2snsoxtdq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qmnsdjzp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgxfdxvx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zymdjktb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jrwamwnu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aunuiujv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bacyxhmw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ssvmcgkg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gpdyztwd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ukxlmdme.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xpumxdxw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ycghjqqk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sgvwmtgz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rjqfbgol.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bjntqsoj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2scaoshoi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2iqgrjpjb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tgdkqdtj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzsxrruo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cahfoebx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xhvbnscy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hjwngdgf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2sxiikicb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2thcvwrpq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbmfdpxj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dvgjcpia.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ggzxiwqg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lemgttet.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mfkdmoop.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lrfjcayu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bocpqism.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2anwqxixx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2thdcttyl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgivsszb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2swkwxybs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yudhreyl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2isuvepwo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2huarquik.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yljagrwt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qduunuhl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ugjwqonw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2uiwiofdh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fbagkrtc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wumbshgl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2bkaxbsbk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2azptalsw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2vthndedl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nhexirbk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2giwighpr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qdgichjx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mgtulnum.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lapomded.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lfwyshlf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dlmlycpo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wardflhh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wsubvmnk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2onrksmak.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2awtdvzvo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gzbhcvms.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bjvlqmle.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zmihmigl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2amhpkevi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2clzawkqo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jwosuemu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aycvznjl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kktubhhi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ezicziud.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uuslqpfu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xgpceqxm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bqubgoos.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2spwivbyi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bbpxwtmn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2mroaesfp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvdnwicz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2acgziukj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2piwypgot.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cfnhncla.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2avaklkac.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2udnmffxn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uprqgeav.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vzuckwdh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vlzmeqxo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dkcbpnml.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jswvccce.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2htwfplbo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ghdrksvz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vsgwwapb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2myjeowps.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2luxztlye.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kdcyffyj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ixqirktz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yvgvxfek.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dkexvzlp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bmeuhrrs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zmsmjogq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jubqkmgr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fbpknmnq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qlzuydsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luyyzkgl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2oolzhkpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgpqlkve.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yynirpew.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ahakkoku.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pzmmyopb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2cchodmon.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2elmmxcad.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gsefhyyd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2thbsqqup.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lrbuirce.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2bxauadra.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wszxuxsx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gqxjdjps.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vgpndgoa.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ioztqwip.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2btvoguyq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2uilxpjmb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ciewmkno.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vdzwujyr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ybpsjmhm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2tdqozuqo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hudmpiva.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jhgyiaxv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2yvnuqhax.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ipvmnmpq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pstosbal.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2szvnclkx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bifwwpjz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2saltipdx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dnojthtd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2sbaqxtns.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2rqvxwtce.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ufqxjscx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nvufysid.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2frjpewny.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2iswgdkna.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ogqsxcmd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2arjbandr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hvsegrqz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wtnnsekq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gulbnenf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kqmjnwgh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cxkadeia.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2zjhjkrka.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2acszcpjh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bbvlcyyp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwpvkpm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2lmoemevd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dzlbyvnm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ectneaal.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2isxyqiyf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dmfxwufn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gffxrmxr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2cmqgvkoj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bjghzkwp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2bstuonrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsfiqrao.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2dreekuhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hunekihi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2czaxiugl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lomshgzh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2pccjyvmm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ghaflqpf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fbetcsbt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zvoawjbf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rcqnlyqn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wszhybph.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2nxdqoghn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dgvbanrx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2krisguji.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2liqlshvw.html


<!-- 参考信息 -->