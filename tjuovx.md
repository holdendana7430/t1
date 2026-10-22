代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pjieqflf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gcpejzvv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ruewwamt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2eavwevve.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xnuqvsor.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sjegwhkx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2htyvyrbd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2natqjrex.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2gxyvetqp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ifdrkmwl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2inajcvhh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rfrqhzgw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrnfrclw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2tvrwohnl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2musugawj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2nrcfltke.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vjvhdaum.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2iclzgrai.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iuxsoxvn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jjqikbdq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cvlnuppr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vngpakrv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkuhjpo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zctboghv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2orixxxkj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qoirixjg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mchytrld.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cavfzwqa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ptdxvglr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2qliwuctg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uhurmqgh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bppfrtrh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yaolqusc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ruudsnol.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hxdowyof.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rrohhdtp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2crqaueja.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2omioptdp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lcmwixpj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wzuysbcq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qixuyjoi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gcrtdunm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thhfdxno.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pcfyenpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2boufclyd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gqrraqgt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2oamxxxmt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lsjlbffm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ifxdrqmj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2akmyplli.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rnqzrivp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yiajcgwn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2khbhmkaa.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2htapdbth.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bhdifnep.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cztbiobn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2iogkxvpo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cpatgexc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zinvfkkc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yamdmyys.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2igjzavki.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2lzqglrre.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ovoevdpp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kytqpvzy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2brmhrmmj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2izvvmjde.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kjkmklcs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lfjvfmma.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fxqsewnh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ihogspld.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2vhzwidfj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vdkjztkg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rjxsrnia.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pntqjokc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2lifudygn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ojvefgoz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vinorprp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qiivurvd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bkoruxjx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fztwjwes.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ofjdehhn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2biqiojjy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iifsenhc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wbghojvr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpiqytse.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ntnophar.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mpfadgbl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2awhdvala.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tyaiorck.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2obsxnpxd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2hvscmair.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kzichbyb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nbpjfiit.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nszbxbeu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ntmudonp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yiidzcdt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bqxkfjqd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ufyjycxn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2audhgfpu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qtyfrkqq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rypwaizx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lksjqjyd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fccwrhqb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wkjmyjlb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rwfzyuov.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2pxofywhp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ywnibrgr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2aaxilciq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2goeofndv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2jmleahls.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cctwwkhr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tlpuuryl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zsxnxsxv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jwidrald.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2twvapxyq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dgbcubyj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2akbrrgic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpegqfux.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ifdytxep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xboumagu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qpbvahxz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tguteyak.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fgduiwdf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yyusjzen.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pgbrfyac.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pexgpktr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqfqlybd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xmqkwumf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eldpabzv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kxrbfkgo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pnzxttme.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2bcvxlbfv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eutqqqvf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bucsttve.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jbkfibeu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhnjhgln.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2krvjynnx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2eihrqits.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kuiqczhv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pfkbnveu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2oleclsbu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cvzdhzrm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tvbjjxvc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2tyzwmmfz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jqncrosk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2odvpmbci.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gyvmivna.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wperofcw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2joanejwk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tpqhiyjs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ewhmihsq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zobyfftg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tywbdkfw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ohomzmpd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aobdbxzc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2poahaibf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2rfentuqt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2efzxduaz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfhfmhql.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlombzut.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwysnmml.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2apnatkez.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ekhfnquj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ifozongd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2akfbajmg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wzekxeuf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2srmwmpid.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwvhaylm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ikfnqnio.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2otsonwdy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2mnlzfnff.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tobmxcbq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2woubtnuo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2irxwgtuw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jepjvevg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2sklffqpj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rwahjcmn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2shbbvviw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2izoatlmm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wyefykqk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uhucqcnn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2todpeduk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2oqjwsmoz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ktatmaea.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sksiwwcy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zxtcmous.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ejpotrma.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dftdkhmx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ytsuulci.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wrjjgmna.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ndpjcmiu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2znqmihjm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2iafdifuj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zdopiiqr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fopkwpve.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iwtdqukf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ucrvqewz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pvyayykp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ngptjqbi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2enecnbul.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2omgjmqmi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2cmfzihgl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jfddgfei.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2oaogcore.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2lytjsaaw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gajynurz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2okvqtwta.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2immhmpyh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2lxcqweue.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbsvqtsh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ehocbfpc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mzzsvrya.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2dgkkgceh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qjmacpvo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2atkcmnrz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cafekjbf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lmknxyzy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xncggljv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ndjojmht.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pymsygqi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wmjtwqwl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2yxzrqopj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sfxxszny.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tnnzdhgi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2igudryud.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jfjlsfwt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ibuxqbef.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rvnibgph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xklbepqv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2llzbyoxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybowenyk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2odavidfh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xblkoqgp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hrdqvjdq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2saoxdnus.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2znkodrml.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bsizteaf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2itzgbqng.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wbfocvou.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ndxyhuzb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jszqfmnu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gmumqfel.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fvkuipnp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2grnfwltw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cxkqhmvn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2sxvqlduj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ytitxyoi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ocwgiuqb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2eixnoxzc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ftovklns.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2easwskxf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ahvecwqe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2btxngzuj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ebxhwhhr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbbzujxf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2uiejseil.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zfpoqdvp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2igrqgbmh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rpwfsbsx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2bcotegqj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2itiywnak.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wetgryxy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zumuuglq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xfvnegno.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2gsespwhh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2kjeqtpkp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2blstzegf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2brkpbuiu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xksvzpsj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2yvedkhbs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2uwjfbern.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cweepldq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uhwrbief.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qjhqctxs.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wevfzioj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkugzysl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pvbzqwwf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wthicotr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2nijnoplz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2amkkpuyl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nibwviho.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dprdajsg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2gagxjzaq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xgtcaekf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tlnmiwng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jiguqpot.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2arzrcmjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqejxypf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dlbmuuhi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ccwqfbhk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2owixtqnr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ixpfckzj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bnbjemgh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zsvcxjdf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2crgvcyxs.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2aybuxdxu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gsogqsfl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wifxzgnr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2akrgmzjk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ilgdtoqi.html


<!-- 参考信息 -->