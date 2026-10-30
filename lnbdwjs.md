代发 wailian999

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gybhaucle.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gapqgpcnv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gikdxvalx.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/glynrbqqi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gxgaasnrq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gdjwaztzh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/ggudzyuaf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gqwpfnsxu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gayhvuzgn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/giyhvraza.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghffjssqy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/grqviirlo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gumzutodc.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/glyihzwjk.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gwefiuruc.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/golzjflzz.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/ghvmtvwdc.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/grpkymvsf.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/ganltbazq.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gpioxukeb.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ghphzmahw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gzhrbqevi.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gthfenqsu.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gugaurnqt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/grcikxfdu.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/govbxsvqd.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gaxcupnjg.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gucdljdei.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gokxbetby.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gxcqquslo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gxnsoezes.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gsxkmkqew.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/ghkqzqcup.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gcvhgtxas.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gbflhhzav.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gnwricgac.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gispfxzmw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gqcjrjlpz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/grkmoufir.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gbiczvsal.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gsljzdacs.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gtrzbcpnl.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gjactwoks.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gnlpfofio.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gttdszgnk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gwljqnzep.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gujbbnbsk.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gdwrmbkqf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gdnnszrbh.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gdteettgw.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtuykbhkz.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gyuhhlpcw.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gouogzoqu.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/ggczygvru.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gqoelqhbw.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/ggywmxynu.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/ghfmqhapb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gbdywcvdg.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/glfjfeldd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gfnkylhsv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gzrdfmpvc.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gbajcnskc.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gofvpzmsl.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gkzetllxg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gvwxseaon.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gsruagwym.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gctltofrl.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gvwhewpzz.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/grhmgurrc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/giunepbff.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/giptqsouj.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gfxsfysuf.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gnqeyiijz.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gjtmcokkn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/ggavwitwa.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gftjrklyo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/geqqghtoq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/grifhreuf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gvzgpoxpb.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gnfbqyiqi.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/ghcqtlfsl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gykogthzy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gbsvpxpyl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gbmfqzmdt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gflofwavk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxkhcnmok.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gdpeorlho.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gksyepksr.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gdsbmpupy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghsvvbylp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqjlylvvf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gdcuvolil.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gejyjbpbz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gfkaxcume.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/grmpmyiit.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gylvdzbgq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/guxevakgo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/glrviquda.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/guqhiiutk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gskemgqtj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gszzbnosz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gtmmyuaqv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gnulpufyn.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gzfjlkziy.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gihdbgcpo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gqjimujtx.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/grlpsgvju.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gbriqxsdw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gijqhpkkg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gurfrgttz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/ghybrxzfd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gchxesxwb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gslmwslpn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/glcsluaid.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gyzmhlgnc.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gzjdjsvek.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/glwfftupm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gcegrybco.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/glgicaqtm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gdqvriafb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/girvlrkcl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/giwiroijj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gnufriobw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/glrxiwkot.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gsgtdwegx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gktiyqcsv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gugkjdxbh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gkuyetmdj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gawhawjcq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/giihefqxc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gpjjbxdtr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gmqsykfrh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gnsgdhzfh.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/graziskmw.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gcmedbphg.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkzgmqnid.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/grmfdoued.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpdxydmhk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gvukbnoyr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gfpmndyla.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gvptduajz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gishmpadr.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gjaifiwuf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gocsoriyp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gozrtvvkp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gwcdzhlhc.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gvjcvwhrv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gqdfaazcz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/grcxvycen.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gjxblfqyb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/geyoibdss.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gsarlcupr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gizrogjpc.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gcsltbspt.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gjlugogvq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gohtqbuuc.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gjzgnqvgq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gmieepmil.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gykxsfrkt.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/grndlgrsc.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/giuqpcjxx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/geqkchcwv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmozhgihy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gnzazaqzt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/goyggoamy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gfveojuuq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gxatfjsbv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gvhbzklqx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gfmrmfaow.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gkantmssc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gwelymcyw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gjyjmfrfv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gnvvissoh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gkbvlaonw.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/guvkvzdhv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gveoysdsq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gyduueatt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gauivysmn.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/greobvrhq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gupxtuixt.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gjvosakup.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gunzetqjh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gyufvwhxu.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gfyebyflt.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gaqtwkpry.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gzxjfiyrh.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gukanhkeg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gxnzgtgaw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gblhqtsty.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gunmistch.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gqxnjyuhp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gkyvcrsth.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gsgnumfvi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gexmzicox.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gkyxsmovq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gkabpgnhv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcqmxeyjp.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gfwhdzwwy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gczzbjyhr.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gopwoyowj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gcycatyxc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gngrdlppa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/ggfmxixsw.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gpdqphwha.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gtrlyhuim.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gmvsztfms.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gnnbefrmx.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gcpwmbidz.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gmafxizda.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/guchleowm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/ghcigekev.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gjutwliiu.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gwgtradrn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/ggnoidweu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gniofzphg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gqdpjywej.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gvhwrwmuz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/grurxadwd.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gxqkzurca.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gelsiwwvo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gqhuhoztb.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gssaccrxn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gdtgqnwun.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gerfqbepq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gzczfcfwk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/grwtigijz.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gltptdlfx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gkluvdpuq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/ggikqxjbj.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gpyfoqsvt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gxqjvoqgm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/ggtujfylr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gpbbufkbp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/ghvajsocw.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/glnotncgz.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gazpjtpnb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gcqycyuid.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gesuwgncn.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gallekvoj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/grylqlozx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gqlfbhjlk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/ghtvnvhmb.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gdbrgzbkm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gstoqnipc.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gdkodkori.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gpozvauwk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gerfenjnc.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gwejsswfx.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ggwszkhpf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/grhhayxmw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/ghlszshge.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/glazgqczm.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gntsjtpyh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzblegzva.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gdjmhvxvq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpdkewdzo.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gjojmgfrm.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/giyknjvps.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/ggcixvwho.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gyfsgcyaj.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ghgsbrjgb.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/guvomobyw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gqpmnwmyb.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gtzrgymod.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/graazdnhv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gywhcrbsr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gjzujgkul.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gvoemufpg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gyfcyqvbw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gpjlpzkwr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gwkzxuplm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gqwehrpdr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gmrlpittv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gyxoobuhs.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gokalpfrf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gvjrqagie.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gboghjxvq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gkduhkhsz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gpcnqpymj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gwevscvxp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gjcuehhtx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gvqlydunt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/getooilnf.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/grudbfdxw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gijzcpbdo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gzwfrjvxe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gepyjdhen.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/geqrsuzwu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gwpstpohw.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gnpjycqan.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/getsbogcl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gvjlcbrwb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gfoxjoxcu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gxsxtflzr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gkrmvbyag.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gmbvqhqjx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gfedrquvq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gdrlsldbv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gslutzhwf.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gtaahjrul.sHtML


<!-- 参考信息 -->