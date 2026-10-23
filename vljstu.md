代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hiiwsvbd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kwqgbfru.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3esrowort.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bekmbpfl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bjpsjksb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qcuwxfwe.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3krslwyum.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zpwrvjod.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xmmhzewg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pkyjbgve.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zpoqihur.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3szbtjsdm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ynpikfnm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pebatwgr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3tkeloaig.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gxjrifzh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wfxnnsjr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3sgcdycqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlusxird.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vhddaqpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3loeadfhj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ncwhgudp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ttnqrsfz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pcajdjel.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnghyzwf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bgmjhtya.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ibpkfobl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wyojokpp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dwdyxoao.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3neylsjpe.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mivghhhq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3clevqgpf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3otsgddun.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oeasigka.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3arvfoxta.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tdqwimrd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tbtjvdit.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3klmibfxu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mdubcjkm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ysxishtj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gmwmzdzu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jcaebkye.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sszrzydv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ojadkphc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3imyailyc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dbvoqcmr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dpfyniov.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3nmiwueah.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qgdmikem.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3aqbyfpgx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vewjrbas.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sbnirqbg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nojcjsmz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kvcdekju.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tmtevcqu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wcyhtrsn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xfscvylz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ljkmxqhx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kakotszc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3klpzkufc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfeeqfgp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxfbvqxf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpzujbfy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3egdyrzjy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qxtwwnna.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cqmbcoyf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lwcbafjo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ycwxmiut.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hzkynrld.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ucqzyrtl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eeklqepw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cfxelqmo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3csknligs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pjugvvdm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wqaxghnw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zbqyimri.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3djoibzsq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kfdugzet.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ougciqtv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bdekpxgf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3dhaadbbe.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rxnqyzhi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xlvtjfdn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qhrbufyd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3dvjpeubm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lguetecp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3inuylaiv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kbvlpfxt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3izxpaawd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qnklqmqg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nhlgrbts.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gipolrtt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3duqfibes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nerutdng.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3lhblhizy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jelnzbuj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wixnxhqv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3odgtjdxg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ipknevps.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jxwpfuxe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gwtuaskp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ofsgeniu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywsgfllo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vqpcprbh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wmjoglum.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zrqecpfc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lwmxpyqa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yabronkq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kibvamhj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mjyosmij.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hnvmxnha.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ogrwbgfc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nggrebrs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nmbdbxsn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vbrmrhqq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qurefwwi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3zgrcgxav.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3szwlbopv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cjcadrab.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rrgctler.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ckaligio.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lzjvdxtk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3oskphauf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pnkuhjat.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3svpfyhpm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vyjgaqsm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3erxuggiy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oqdrfkcp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yixmhazy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3bmyyitfs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ogmoilbc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bgduevhv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lboffwob.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hyqajyrj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ozmddais.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mkbupzwn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pvuelfup.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nrhzzjml.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ssuqllso.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mdcczgda.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3pztgigjj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dbraradr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ghyjxsqp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ushmqwug.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3poxivpvg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zetosrdj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pzuncytd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zcjzigtn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3epufipju.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vbabvlxc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jbsikleu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qbplseaq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hkpqgawq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gdthploc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3plqkipxl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3nrrydvqb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nywnshep.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bdrdlycy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3evqbqtru.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3eetaojzl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jbzsosyh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3khdfbjjq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mvljbzsq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qcmmbdxp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aujvbgue.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3erzayczs.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ffhgzgkb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kimamfvc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vrgtvajm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3owbfqifd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vsifljyh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zhcssobh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3zvypxccw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3udksbipv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kqzwrqlr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3itjrgkhm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lkvxfguq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mvnwbvlb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fcxrclls.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tbhzelju.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gvyvmlbt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3usncbciu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zbzsqhbt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3lopnlckk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gmyejwxk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtnhqrrw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bfmrfquv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3eeicpegk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ajzrdxyc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sjlijapw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yaxxgiuk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hajikmnp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ywogpjjw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3yagtkavu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3byyfwqza.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fwykxnns.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rtsjoifp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xcfeyhee.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ymcasyit.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rcbvguzf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hvfazfhs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3saroidpm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3owwkkflo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cglbilve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpsdlcni.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lhsfqezi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyklbkdr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gsviyyhi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lopetesk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kisjuhpw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mqqnteax.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pwnbihjw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ddmchaho.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mfbztiqh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qmvgcrxx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3oqronfxx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gefbqhbe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jmsravqs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hlpxghaw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3csnlvoxa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yzwfriyt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vspurioi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3oplgntsv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3iqhujavo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3oecnwsek.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3bspvjslh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zucdxdaw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xyqcjfqy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wkweiegu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qhomidse.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3efwdadoz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jabkabgk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xmnwbaba.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dizyvyfh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3akktlwmb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3tkjslvwk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3avysoxuk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3thcxvvor.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3amhanutl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3cejxlxct.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ezpnutsa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vkbmaigj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfazthan.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ibatjigm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kygzplbi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rfjpwifd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vvkoohfz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3derjxgbc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3wclcepcu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3neovopwu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mznjboce.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3lowdnylm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vncpfpln.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qatywxxf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3viukteci.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jxuxaefz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3etpwmiem.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lwqfeapo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3yzvvcibl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3obezptza.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3gxjgyhnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikcdmhxr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3hdlwhrhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgeuvbwu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zkemcyce.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hyjtphey.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tggqrvlt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3eiqxocxk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cgbkglqw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mgavdkcy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dohwzomp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kijmjlsy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3okdrmvdp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3myaqnhmc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zazgftcy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zskaujxr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hyldtecc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gqkutert.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3odcotabk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ddnwjjip.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3hjbjdgpz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lttnmjhw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ulgugwkz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3qfkipkwf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3llxzvggw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mdzjnvur.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sjzuefww.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kzdjcfcu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3clcvfrbp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xfjuctqi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3zkgzoqza.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xzzjivjy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ucdjpnhn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3trhetpyh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xvrucclp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dltpkooe.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zyktekck.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3pndvrtfx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nhaadtuf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ugusvyma.html


<!-- 参考信息 -->