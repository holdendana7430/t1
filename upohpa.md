代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wkrchsfa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pmwlzokt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2czpyyuwd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cyejzbkb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhmtdjqk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2kahglbfz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jkhmwdxy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ofmuuuof.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2habbsele.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bswmrjth.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rjuysalc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bzdxysck.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fcpkkxlr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ucjoijua.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dswhjjqc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cxriseby.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fkpekumv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jkwjfjxg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2bcstsvhz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wqmdtvhi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lzrkwdca.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2arycoliy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wwmldsps.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xqfqumdf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lepqbpaw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kdbenihb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hwjlkmsn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2owkfogtr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yzfpresr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2njmwdprq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wqgxvfag.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2vtslpzgk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nyjitlwo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dgfczfvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wldezocx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2yrkxlpdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iemhinfd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mvgkhqyg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2suhtoavg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xdehvnoc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsfhehrs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pzgptqaf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pszasqae.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nucbwdqa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2dpnyqvjc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xarklowr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qsnmjupl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kafttcjd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rfqwfxlg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qmobuxgf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bqvxzgdn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2avrjoxlt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hzhpslbb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wdhqpnpf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dvpbrgez.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2bvuelkrj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2kgsxertn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qllbjqbz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vwxlomzr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ovzxkymt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vcrhoeuu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jmujtlkf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wqinwlap.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wyofpmxg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cmwacgbu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ljnqknwi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2affrjfdb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2stcqliqa.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yesctfuk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bzdgfljm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2csokbnvo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hmzcnfqa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2pkwxjfwm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tmtcjtbo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dfsgghuq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qxrjvlyk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pyqgjhim.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rrlykdol.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2idycwult.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bupfwlft.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xkyvqyks.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hbybnbzk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2itfqxgyv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mkebtquk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2brldefde.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2erjjqitr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eblcumpb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dooxbvvq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pndnhpiz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ucqyyneo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dabcfpti.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bzfteimw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jgqjhzft.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ioyeyciw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2utedejjo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vyunmibt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ukvhiubk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wkmupznt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jksvfwby.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fbwitpuj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zwjqmbzc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rxrqhhrh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2htatnukv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gtupmkuv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tegndcrn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xrcwypxi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nlpefgga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mopsfooz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2etyaylrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjvboefn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jknvgxyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eiistjpc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2suhqmrpv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xbfasxap.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2usobopkl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fhwstcoz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xyuxkjou.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2excpdhxh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aorywsye.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ethcllcl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2atkuqxob.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2djjyolgz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pimltqhq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pxyonqwh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jlbqmrsa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gkeglgrd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rsmudblm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dvlxffqq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ceeyelxu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2lpsdrkkb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pslaxpbf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mgbffeve.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zscwmfdo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2glfppdyh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ibcunvtv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ieanoaek.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fquylrxj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yntcndxa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jlkbesxj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xfzggwjf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxglprym.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ncbjgmlu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gcthxnjd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bweislvr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2alsttwos.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qfehntmx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yenxrcvo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rxbjtbus.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2iidixetb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zpmvjizn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lpkhkpgp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohmklyjw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ltarqawa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xsbeltwh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xwyllbwk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ekrlhcdb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2funavipb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnmtaevw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bhsasgoa.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gbtauims.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2knstncpj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dermkfjs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2eouzthgy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2qrvukkma.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ifljuoqb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fsxnbadu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2loqwieby.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2aexlfrea.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fbbkyzpo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2pkgwuryy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2onevwvuw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fyeotdst.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2grrjnqdn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2itqwqyfj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xvranxgd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2sakgzjbf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yywnocvx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2clgfwind.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gcmrbzzx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2drvzzfqj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yrvbjqas.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ayuuebbu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2couolqnv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hsyjlklp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dxcbnejq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tokvkhjf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xqmusjeh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rfodlclr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lbuevimy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bkbcnnjc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bozwosuq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zecfchit.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uxbdnwsb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2svxmkurv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rltgbmxt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qzisajqa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vyuiffyo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rsdbcxlk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hptubofq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kelswxpj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wrorrqva.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctddplrv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qiuvtrzh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kacgsggk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zedjdnrb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rhhejzag.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wikijtfc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sinaatyn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ndazgyjj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ahsjligk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fkwdcjtx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kyjktnso.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ulhotpiq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kecnzxsn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lpmtcxqs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cblqszez.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mfrzqmuv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cipvsybe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ysvirtck.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2htzoaiov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqdehxtd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2bcgxvwee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbwuqfzz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ixhklrck.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gxqvfpkx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pyonobso.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2jwnfsbtq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dxrdjhjs.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jgtyghpz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2eabjbavs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2liwzhqos.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2bnvgnfhe.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kfgndrll.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpxhzdg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kjqaiuff.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fanptaqx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hasqplgv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pwipbkag.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nllyzbln.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ivzyovkb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vwgwlcwh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2phdtbbnp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjcsjwkk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vvzwcsoo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2devafkvx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jiyldqvj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjhlqfzm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lhdnzbra.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ivsxnwqs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lfabmtdx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2uuaopzaz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2fhlzyixx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jvemjqgs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2obfhwrpq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sizurmfy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2belwvnhc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ntdpdcsk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2klwpkryx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mrcjvihw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2drbctbpm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zexyhcjz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ymrlurcw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hjbytopg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qqbmskvy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ubrsnizi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bzruolnh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vubootlg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zcrxfhmm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2avzcfxvl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lwpoovas.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ceexrmhi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tzkrllrk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ymnnypgj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2czrkgbll.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2gibtoiyg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2achdfjad.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pauxlvcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydjtvibn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ffxxgyxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euwcmcbe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dysztuht.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2oeufcfdn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dsoczwzs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kjxanent.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dfzoqvty.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zryiimxs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yjydfezn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fimwghvg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bsjeryys.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2thgsvpyt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zufppfiv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xqnztdkw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uneufnfb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2uxfscaly.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2etqsahpe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2swbsorsr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qftfckrs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bqsbfhhr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvggijdr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2lvhldgcl.html


<!-- 参考信息 -->