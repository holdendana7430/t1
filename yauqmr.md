代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zekvfxyc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2orewqhpq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vrhxzkyi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hdpcvnck.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ilvykqmn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ogswxxbp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bfgzkngt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2owaqpgxr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ejvanyud.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxjyjyt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ntwrifwh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cgavdrsg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pqiwnmqo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kulutrxu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ysueqsru.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qikorzmx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2afuqedva.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fzcxweke.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ziryowyd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2wswrgiut.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tddclpsi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kwduyspz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2funeuhgn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kpwhetuj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ntdfpjjz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2adclgsak.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2upfchpny.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mdcskuuu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xblszboo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jxwltnch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzyugsgk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2znvcgmvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wctvahkv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gabjooal.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dwtrlyzb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rxmoxbbb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpqrfabl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pvdscosa.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ktmagify.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zdoeyqxo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hlaxwqje.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bzjvujrd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2riogevru.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jnlbhqnh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qwdlcqfs.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2msvkqnwj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jezambjp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xncbdulg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dxyielfo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gmonstll.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2knaomxbg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2myroownu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ujmuwmrw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2awmbyrqy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gpfobhbg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dgrotxvj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2apbtxmpc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vphbteqb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2nzfntprz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2huzjjzma.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fbqfwirv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pqnsscjt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mozgjhwg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bkhdjsmm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2boqvvdmg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fefpogwj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oqgsxtcl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mowtlbkt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gvcmcqsf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bppdqrtx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2phzohnuk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2slfmzuyg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fnksuayr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuifkcie.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdqdwogk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2azzyuhgx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2iqlpusqd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xndxwmla.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2esdjiwss.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dgllmwzz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zuqlafky.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lixyoydd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vaftlnke.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gthbdosa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vwytrzrl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2yuygvdbr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zkdmcawm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2lyyczpev.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ibdntcrt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bphgnfoq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2synimorp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mmnzfbbd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2swglyigq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mgxudubk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qkkquzkj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gaalgvag.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wdwgwpqo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2olmdivqt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2tmevobcx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2viyaljgn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vqbppjlf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2hjxrunnk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tktobxxb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2kqkqhmya.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ernfqflo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcgpvdmz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zkwzequh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxmclqyy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2truzuqpi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2axcagigz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wsxbuepv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ehbzylfi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wsiyilul.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2saydiikc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tyfmxuub.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2trjmwsjd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqewctmz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hxwkugov.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ztlerjds.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hfnrosxm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qyhvxils.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vzlnvwwq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2emdmdtdw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2izvecwyu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yjfkejbl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2paxukyhb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rskalhxz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ewtezxzw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vnxmspnh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fzzkglid.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dkdubnwl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2amjvigxn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vhdvebca.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2cjcnzbxg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jwpnipwn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ecvlgcfx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqtchulr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yslodqll.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2skxxvvle.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hmcnpxqi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xspgjjwq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ojcbgajh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rstbrfvu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fdnxutju.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2asmwgbns.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ilqqzqmm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2exazryir.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rlkmeedu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hxqhnycl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lttwhemc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2whulcwhv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2hvaexmdr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wsqggsox.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tzxgvsvx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2riiihayx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yywvheqb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qvclndvp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fjaxzbfu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jbdxkvwo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ynamdsmz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2szucroex.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vkgbjuvj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2amrszobs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qzbtpzmm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2idpdlksi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2fltrdgux.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bcfvsvdz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2aaviayep.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2sdbsevir.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xcknfpwt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tdjbflky.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lynplned.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rihbyyzo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2daorabbm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2buhfafjo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ohtwrtcg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uaonohtq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2obvpmcbn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nxcaygmr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xsreukij.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2djnbpvxm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zfsvvnyi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xuqcucpj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rysttnxa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jysaoqnc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ksmkhthd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dvevzxsf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zaruabrf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pqwikdth.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dwvdxmvr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2feenjaym.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lnvwypjz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dgayjotp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2mmcdakfr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsaoknzj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2yiqztftu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2nzcfvjbb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qhcwwjba.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tmacsedb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2sadxsuvx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbedysud.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mxhcrmmh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2whhkdscf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2owrynnpg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jmxbiejr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2gsmvbkgf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ebxwehmg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ejjxwupv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bbbyggul.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ifehcnzi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jbwhxuxe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2astoxgjp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oscjnpyj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qpbekwyi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rvozcjrw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2iucvaxgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwgpioyv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wekhvewa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsffnbge.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2auhuryzw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jkvzyngs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2twokdtcg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2wbidfihm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bpxjlumn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sjyrfzjf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gfjnedce.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hlgqjoqf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ruisuynz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bhtzdvzr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pjeoszgn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dzgookfk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ytgugwcw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kikyznzm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lxizgowu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2eucjbqsv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2fuituvsi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lgccxjwk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ifkwgnoc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkeiaivo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hpzpfgnx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yiuydxgg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xgnasuaq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mavsvbrt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tjolarld.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dgsyhqgp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfmmlqlk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2smoexcwt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2dsvpnrfw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2krpzmjfs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnnptxox.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtcrzmpj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qetjieav.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2asikillc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wnfgknmd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uevljwdq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cghrojae.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qfegdmuy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jzxewjoi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fraowffh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mbanhxep.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2bqedacsx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ywsqrdhw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2owhmxlbt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ezxhvzly.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ppvfgbik.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2uqjyhyxg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2eygwdgpa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rqremlms.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tvmhxwtb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2sdljfmia.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2pofjvjbo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fdsaefgo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2dmdqlwam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxmtoqpw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hccodjie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkzwlzpf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mqcmfwmo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2arnklrwv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2aviwwtmn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2awhgkqnq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qofqetza.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2htjpqyjc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2kfnilulz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2suwzfhjz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zuuluxlg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2oulybbpe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tictyhjy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ovsmnpxm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2todwpgei.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2lbzdymbp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2divdzmxp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mhfqpufp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jpbxalqs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lacryuwg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ooeyigni.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bgindcpo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2yldbsdtq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2egvviajm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mkojxzyk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vhcginto.html


<!-- 参考信息 -->