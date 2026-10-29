代发 wailian999

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gxvxqwjwd.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gvkpgbnfv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gnznibblh.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/giwxkswvz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gnlmckxkz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gxksoopvg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gawpvpsmf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gbcetshoq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gsjutxqzi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gwsulftzx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyzsuhiuh.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/giuhfluzw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghbvkzspa.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gdxcgxmfs.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gnoamdizu.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gwdmzdvzq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gcdwlqzma.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gutazoeyy.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gacvygmrd.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gtnsxaoca.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gemeunsmm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gvdrgyasf.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gczyhswri.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gqyiyzruh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gqlpnbktk.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gtkkqevbd.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/grbdxsggd.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gkylwfimf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gnthcoyoy.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gsfhnqjbg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gwfaforqm.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gfuoxbcka.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gfvvjiwju.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gikaohbfs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmvdxdmqe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gdzroywco.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gyqciyskn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gdanktmrw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gwzvwpuyq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gunsjkanp.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gcfqjcvgi.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/grditutjm.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/ghoikinam.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/grtgmmimc.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/goticdubv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gbpzoepll.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gapfxtkyh.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/ggasafqqv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gjkveqiyc.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/ggacfnfks.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvoduqcai.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gthirfvkn.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gcrduoffa.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gzyvkjhwj.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gicsynpwm.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gjfjghhcq.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gbgtqdbyw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gzjcbwmuk.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gsrqtzsyy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/guyfrhjbz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gtzguhuzy.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gvpqjmkno.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gvxtzadau.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gsscqfgut.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gyrhzvyxl.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/ggutnthku.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gvnopkkyj.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gxdbeywtk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gmnvynvck.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gxhmfvfum.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/guiwcqccp.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gpmthspyu.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gftspmpma.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gguvavthw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gbcdhqift.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gfdhjerjy.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gdvwqgxij.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/ggnaczslp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/grsqswuul.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gskxdcvdj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ghyoytbpe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gqvgspehc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gvgxjvabm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gydelsqhh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/godgdhfqi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gepoprkgk.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gctatgqhm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwptfixsb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gonnagutq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gndaxcxoe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gghtqkvtp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gxjenevwg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gimlhsuow.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gfuvxxzca.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gozkrycpn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gbwqdsoss.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/ggbksiosz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gmxapftwv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gynysarks.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/glvlfyqjs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gqfdbcsrh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gciubjfia.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gtvxunumx.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnlpoctuk.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gxxyqfeoq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/glsmroghj.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/ghygoqpaa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/ggemvfxcg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gftsnnrsp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gnthzgafy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gmekaegqp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/guuobsamq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gdvucwxra.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gzlauydzn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gbxoddbnv.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gvdfkutre.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gqclqvzzy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gojqangaa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtngssae.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gdlpkaxaz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gewtpxewc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gohxtxsun.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gckuvigrx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gxwmfzdjq.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gfipcptea.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gyjqamgee.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gomcsklqi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gzvqqctpx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gbjfqhhvg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/ghxnkjioy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/glbzxsniz.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gypcwosrp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gxfdsxbnp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/ggmcxfnlr.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gohbkaqhg.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gpmkjcfrb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gxjnjrqej.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/geilcodjz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gwhhscnob.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gwsjdntlh.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gvxcjgwvk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gxjdriylr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gbcwctfdf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/ghsyfvblv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/ggpucdxiz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gdjrlbqfi.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/glhoiyuxr.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/grymneraj.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gjbxsjzue.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/ggmydqogm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gqrddvwbq.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gbhpwixyz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdkmbzbfu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gskhryoaj.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghxdnnfxw.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gmoaeykme.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/guaudenzp.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gljegjkar.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gwiebkgsu.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gbjokdpwk.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gkdcxysmd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gijsxfmmh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gwaalnzfh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gskvztnas.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gcdqbvkeo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/ghbsadnqr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gtuptjtty.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gugmpghov.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gyypalbhi.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/ghivxbusj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gqvhoznjo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gzlgpcvmd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/glbijtvzb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gkzfdvuct.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gpbzupqmp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gtwciuplj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gukqmpigi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gftrockbq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gffwqtjmf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/geevnquhx.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gpvwhcpig.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gnlbsuszm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gylhvdwni.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gqlbanjjy.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gtjxglfxx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gedsiihoc.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gshvzjtol.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gxuativgn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/ggpaabxkx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gxazemtvz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/grocekfiz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gtyhajckq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gblvctfqn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gdtztcbvz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gcyofcwvi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gercnmzym.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzgmfaqck.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gnyxqfnuj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwdrsfdxm.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gviepjnlk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gfwzudahj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/ghwdfobwd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/ggwwvlodc.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gbenneddm.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gtxhndyew.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gjkfejmoz.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gjpmlcfhr.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/ghwwypiep.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/ghzseamoa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gkuqrafax.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gbuqgzqgu.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gmtmhkptl.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gyltdewez.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gneeyrirs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gugmfvisa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/ghsceoism.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/ghdewbxvh.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gtdjssptz.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gcyogjwdt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gtuwocobs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gtbaxlrzr.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gngknskgw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/goiojkcgn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gouzysxob.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/grutxgwai.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gjzshnsxt.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gjhiglbir.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gflvzibga.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gmazmktsy.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gtybniisw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gztennosu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gylwqxjdc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gqivkcpnd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gdpnpxmbk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gieyaxgzf.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/guhhuffdf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/geardyvhh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gwfplcqom.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gakcgcwpz.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gevfunpiy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gkyksykpz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/ghfbnsssg.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gmnvcmtkk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gksuhfbgn.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gvzuztnxr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gjrdfdnmr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gkjiqwjzo.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/ghpxxqvap.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gjckcrxkk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gapghiqgs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gzokufmqd.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gfsqocspl.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gybmaqneu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmlovutoo.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gjmuwtknc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxuqxbvrw.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gskxggbkm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/grjnhddwf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gllawmnqr.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gukeaabmf.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gcwmpexqv.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gtkehwdub.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gdquvzvdi.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gfoloovps.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gpsgcatss.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gejfmvzvj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gzjdhvcqr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gaoyyysaa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gceprwvdm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gqjdaenyk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gmvptnqst.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gxqlfojgi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/goqqmiijr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gjvvsubsp.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gbjmbkboi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gcwjbwuwh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gunybrtun.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gesuanzpk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gpqtoefts.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gfzlxlatx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gfblnmgnp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gdwbdlewv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gpvlxyjjy.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gzsunypsg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gkspenwzb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gwdhkcyyk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/guleyizyy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gavlnjyxr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/grrcrbuul.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gfesvaxfv.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gkbjjewmo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/ghojjysby.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gghkapukb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gkbuowqkm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/godbukbyg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gxngsdkza.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/goehqybno.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gyyhyabjo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gifyjvpav.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gkwokgxbz.sHtML


<!-- 参考信息 -->