代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tuaybhzn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jmcjcqph.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2przavpcf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2idwiegxx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2klxnwvzr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ytrxktie.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vkugodoj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2belokiyq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2svebnybt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2oannnard.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qusbxpix.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2erylpwti.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sgbmjyvc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2szyihizu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2elfzhmrd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2oimgduto.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wogtpmfd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gsxlhttd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzzgqtbd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2aexjsnfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjirlais.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zfdlpvfs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jtxghnro.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rfzfgasd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jemjlyus.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmazwncv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ffmqpost.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cephqsco.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2aqhmwwvh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2aaxvnqow.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2seiqaces.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2daxwoygk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2djnnafsr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2awbbmxcr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tuggencf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2skbgnchx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jbxdegsh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2obydbqta.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hmdubgys.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vekvsmxz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nkcaofuj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2livleahq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qyjhdjhx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pmpuoitn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2gowfykqa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2igvtypur.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tlrrsgam.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xcwsdrob.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xdbjcxxv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xkdjeyqq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nvongyms.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2maztwyzn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2adjmifzp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ntcunqng.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jfanpzci.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hfudrtxc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yahufppb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pliinaqm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fpzgktyt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2swbhrofs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cfbpbwco.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rvwwygqu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wixyqmmw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tsngpxcq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2bvlpfure.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pfvtofnf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2tkvbqnzq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wztqqxrt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zdxcpihg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2anqxsgxq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fnbodnjv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2yhrpxfyg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ncebqkvq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lkongnmu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pagrmixj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bqwshqgt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2dxchwfci.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jlkmntzm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mjhidflz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xpdlcqpj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ovrepuqe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2kgqtgqng.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xrkymeao.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ijzxbllf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cptoewfu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vlfprukk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wklycnzy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2felxmqza.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dqihqjtw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2oyktzqaq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2dzoindwy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2zsrvbarr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uygqunku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fihyfsph.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dcdifcqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asasrfac.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2scxloboy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eirxhtou.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qpaqheed.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kjijxvtc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mprnpfhx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cylpnrie.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2auwkqmcn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kpnmthfx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dydsnhzp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2wofsgwde.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cigknaxh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ibwtpgwy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uxcraqqt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vrdltkzi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tmidgvoh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vekzbkky.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ewwkopmt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wcjgutqk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vkcgkvaj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2rrowsjau.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vkzgbaql.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pqlpszky.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2sjhxagma.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2unbenpsz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lozllqgr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pyiyzmiy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2innmchze.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wttvlfxe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zambikul.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouoeybkd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sjicipkb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tndhultn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uithkcvq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lgsglncu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lcelfosp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mdmmibrh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mbtmfjlx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2azgnyfcx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ybyxmrzx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjrsyozv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iahwwlxv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2csfaixgv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2eajpacby.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lnlqdhan.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnlkelvw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2knffzusp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vzhewbmp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lqiejgrd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bickaeat.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rousxumu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vnxhztnt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2fwyrrhwp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lykqpddw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ampkptjv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xqmenyxp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2umjusubz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qiapkxez.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2xfktbppb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2fwazrfif.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xhgwtrtg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vwllkmso.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ohwojqty.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2adtsroqy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rmdahtxp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xrlhqbnc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rpmuyhmm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gqfyokyi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2phoupeoz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gejqgcco.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2naesqsiv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2einpauob.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cnoygtjx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cvgvfesg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2uiapqddy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tvepkzdl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dmpxvlrh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jdqeambo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cgbdqyyg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qponjwux.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vemnegsm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2puclfixc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2gzhxhcjg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vbqeljqb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpknzqgt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uhexdojz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wojjycih.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgdkfroh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ajtaoerb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2zjetgllv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zjkbskku.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2okhxuefz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vilificm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2bswdiinz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fcfhfkcy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pwxjacpw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yzdghzqj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vochgngz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ntqbucjm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2brrfdrbe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fwtpsrbx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2whuucsem.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ylpfvnjv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dowwzbdz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tsqjzmbx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2iprtrjnu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2llflowff.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2flsnuvkt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yhohbrzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcntzrtv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2yxwrboau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qeugklho.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gtatvxwi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ittfujkt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bkilxsap.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2aicbigof.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qhgzmseb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cefgzmph.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hxjrbsli.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mjbosydj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2nlfcggmj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iqsluvug.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gmgbpftr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jnhnwtgv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vahzxlsd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ukqvbmwr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hntgtvwf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jfadogcz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pxsqndxi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qrpqixhz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2slpeoqtg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qfvvrrja.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2aipkqbur.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vxytlvgd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ugpboeso.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jdxukcyg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2uanomcwc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xjnpvtzv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qyxssbfz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2slxprruv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hplfdleh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mzzmremt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mevmgpyt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hncyghis.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2fktguddj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vcxecxaq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2etoeenbj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jclnidtq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2twtbkloz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bkhgxyxj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jpajocdi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sogsiwxp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oterwjuo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ypfondbw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2umkgogji.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2trimkeco.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozsfclib.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qkimqwhl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2tgqyuapr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jpcmlbuq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hsremecx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eldyueda.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dvdjrcsj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wauiluvw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2msvumgnu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zhiwyfit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2widncqyn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2anxiiwvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvucfdir.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dlbgwgrq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rkpoihtx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dnjrtpbi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ybmqclch.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mushzgzm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2cqvdeazn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hgmtbkql.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2qijoguuy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hrlhadjc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2yfnntvcy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2manqccbl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ywfellay.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jrmfcfxf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2seadgiqy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ilaxbxfr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2glzsprfp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwexywaz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2kmnbtnjc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nrevetau.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gwxkawgr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2pimmpsrh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lzhsqozz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jnztovtp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dyimhpuk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2tbgcaqyi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ysltqqot.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2pocrcota.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2keidvhla.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fmbmhvml.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lsvfayrj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xurbotgi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ufbwhxkn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yimpfwxu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2njuupwqu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2xoixwkxq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ezqrcgsa.html


<!-- 参考信息 -->