代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zfirumbk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bhsutovz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xbggjxax.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2qsrmoxvk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xaxgsgfu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ddoeloqu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ocopdbdr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wjbdophw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2verhahka.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jagawcpw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2igapggix.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2iuwdhnyq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2qpvjzlgs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ydjrilvc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ckfmtxtg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rzfkwrsa.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ghfqrixv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yoggxsqd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lfpqsjlh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lxqtxomx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fbzlzxor.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2frmecegg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2mxcjejda.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lknviueo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uzarkolh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rxwggpuu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qrfxssil.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2juiiwspk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tyjqlykz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kbogftml.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tuawuniz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2rciuwplv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2whwlnmkx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vdxlbasn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lvvaeiob.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rsgbehsg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2szuhoskk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2katbowhw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2aporydjg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2exqauyol.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdipmic.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gtgyewzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zarvayzw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qpweqpxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbkpkvrd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yrjkyfzu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yqzatarf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dqnbfijt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rnjvsxud.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2udxefamu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jlmqxqdu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2lzrcpekx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xfllhrxa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jikvtrem.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2benzgovr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tizjwidb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rlqvesym.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qxmwbwst.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tlmcnaik.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rhrffyet.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ncbjljdl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xafmercz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2luhctxyw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pbillmju.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hmsiexlx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kuaaguiw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ulxqhnot.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2plorklxj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2yohmngxz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2fpoeauzl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2wkznchjp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hpvqmber.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2sxrbmqxr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xdpbkene.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wpduojsz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dnrfbuya.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2guwsgsqu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fcrjtejp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pogpdzlg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2embvnuhk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jyfzwfay.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2kcckidxd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfznpgjm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yxyffglv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nipcwgjb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onyviyas.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jyueaeoq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oztnbpza.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vgtpktjf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2sxedhygp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pewhqvzk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jptikusf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mpfdufcy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gipowahn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bnrnrcba.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2scdmncry.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2otcqjloi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mfghzpbb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jjcoilhd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qjliuiln.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pfgkqkay.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ryjjmoul.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hdouwhpo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2slhnfxyr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rzprasjk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tshysuwp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hhoxpcxf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lnwlnpsc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ggpxoksp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fdoiagnw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2eobjlpgb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wavxqrtf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fjnkgzyv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2cwmlxrbe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cischxcr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lgrvoqml.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2kesfebds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgvofier.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2opvfgxrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvjmxhjv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zefnroqs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmphytz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lydjgzrl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jlsoxkwv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2muqboaye.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dhjmjpgw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvascdyp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pomwopkq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mbvwhjza.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rrwousdp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mggcjwae.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ghdqztgw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nuacybtl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvobeycu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rxsqrlku.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cngmablm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lcapmllv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nvdmkzew.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cijbpavj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2irkfmntw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gkldmkqm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2loxanvvu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2njumutuu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rkyoovgx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lmijugbw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dvnzeswr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2avuykxbq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2aucfkfwx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wzrzutju.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2sryubfpq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pyfegrwo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pemxyeeo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kubqgtbe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2urrdqvnt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uubxange.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xanqkwdi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2lriijlym.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tslztmuf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ixbmritp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yajhdxkg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uepqqhmg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ddjbzyav.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2otbbnehc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jqbwkdmb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fpooidrs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vkhfgtey.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vwjnxhzi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2msvkwopf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yyufbkdk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ayvjgwfh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kmtppjug.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pctefueq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wxxaztpk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cetxwzkc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2iofhvijp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2auhtvdef.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rcsvgmoh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kzupookp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xvleytso.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2pejelzxn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ekcwnuip.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yrjmtjcc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tknuswvf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ctkzuqyt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2gkaybdsy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2stgxjnng.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aueumkot.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2glnqjsbc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bfisowld.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2guxspcox.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2okerzscn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jdulzhcu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yynntsuc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kbvpurer.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2czuibvyo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ipdyawsw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fcrivtcd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mdyhzogq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2pmmjrypi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lfxiubxa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lhgnsmyr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2amyyzcus.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wewbrkeb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2plscytnf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ilyfwizz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nqepjrwf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsovgiyi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gffoonnm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tyrgxtmz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2uudlzizk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xdlexgod.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ngprkbhc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2jtzpuwkw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qvsfqspu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2htmduhtc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qitknevx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hktwapib.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gsdprlfw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dcqlstwk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2caqbamdx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2fgrogxhu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2efntxkxm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uznjugyk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sajiylxs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hvqvapwl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ornkbnjb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yhrhevue.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sxcaknry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvgbrhoc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jjgeggsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehqobzey.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fwzngrfm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jerkmblp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2fdwnmjap.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yusfbyfo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tqhpnnaf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vmmvprew.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ajdluebd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2zbbuxdvl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lkomcidn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zltqpdjh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2phgmrpkj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ibxhrmno.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oydovgkm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zkhmmqox.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dpqiitks.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zvgfecky.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2fllttxrm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2nyjybtaa.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2gdypltvy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2aygncsjy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wzbhodiy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2yyrpxvrs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xfftwasy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pqhcdlkk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ctkvgrco.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2keqljghe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kayghlso.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2eztdbzmq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ecldavjm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2izrciibg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgdrrlfr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tfotirua.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vakdxtuc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2mfabjtfq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hsveehiy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jrqgckmx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2svljopki.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jnfuscvm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wjtxccbu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sxgucqnj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2amedlniy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ylsktojg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fppeexph.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fvkkjxsa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jikvioex.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hejmswmv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2etyihdyo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2snodcnoz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hzsnnhgf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pmlqrfwf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qjufiupq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2tyvwojfh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vkqrkddz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2okaeysbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmjjxuzl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2sjtuvltt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcnwqomb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pvhsvjqq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2urhwlcrz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lyhwkxan.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2npqmoiac.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zjlawtgp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2gxakxmwd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ciwlziit.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2jkjhsqdv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2olhxiqcq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2tbgcxcey.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2anrlpkve.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2gxunqlzq.html


<!-- 参考信息 -->