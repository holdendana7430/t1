代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xdryxrfn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3pznijxtj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ukrivhgc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3swqlnmoo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dgxahlrs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ueimavtq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3frgvphvh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hooxbfjw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oktlvvvy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fpqpemhi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3msqchodo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3blwsdnyd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3khjbltvm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zsromnic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmkahkva.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pnnbdvbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwlnhxur.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3voqqnvuu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nzptijxg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ucldaqbx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zskymzue.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ruhrefxz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wblfeixf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uvmvanrm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3uqflgfzj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xfdemvnc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pqxyizbo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hwwgrxrs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gnracqxx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tiwqvgzj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kaztgfwf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ceterxwq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eqxccfhh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tvwuxcfy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vffrqeia.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ymsspqao.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jvfdegaf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rsggqnov.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mzjjsuqa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jpfavryw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gmfnfmjv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wogugozx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lhqadknd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3awfhyoov.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3rudpuuzr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vuenowwz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3lqdgbehm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lchmqqqr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ghbdioor.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pforjadk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fqyfnzdn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yrkvbihe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nqecvxqt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mhuhrsxo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjhifkym.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3afyavqkr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aokhjthc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gvvqisru.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bbtrarov.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukslpqhl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhchkefb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mnxkxkxs.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3prwlixru.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dmksrpmi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gmzurhwb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sojpbeak.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3smirivtl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rvwjnpvq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xrhfizci.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3unxyvnmb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3grmxdfkm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3uythdprn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3leoahiab.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3uaroncyp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3aaonzewc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uttesacl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tzrncphx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lfydpvja.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rmytfaen.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qehgblcg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3uhixgazr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lubiutje.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ksjppatm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pbwsmqly.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3stlalqhe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mkivwtdj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fjoczbih.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kddlbunr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3iyuzhawx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jejtyirc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3vunuglsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgpiwalk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3yssbxyyw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3blohscsk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zxjlimof.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iwlsotfa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3avjyfmpy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dscmhtny.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ytfwiqqq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3leqsrnbs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3poyrltvs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ydqputrb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ttbqyonq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hhmaxiwd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gmzdrejg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cmahnzhr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fqkhopea.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mbilfdpl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gmpnqmya.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3aujhnusi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jidrtjja.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ghyjnhhu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3lrtnglcw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ktttudie.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hwuglklc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kxwrjqik.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3pdbhvjym.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jqvpccxp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3sexkulvu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vaszpbuo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hjyhnpos.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxrhwhla.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ucxbphys.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jnmcquwz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipwrdrjr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvgkkjfp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xbunhbos.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xeyuiilu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wwjpndwi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zvzjqxgi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpcukvaj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gddylcvg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixjtpmsz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qiropgwl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xstbzvly.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kszfqfad.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3nudmlmzo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ckzarlvm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3toidlufx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rosevubj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kzgmqqfg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pmcnltgu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qvldbear.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3eqjpbarx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jpiwatqw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dkysqoph.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kmhcfkpd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3yyxcahzn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3sgvnlpqu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jeuediwr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kybycgdn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3atxaijxn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pbogkvgf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3imrlgjjy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zajmmyea.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3dmjpsyyx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bddxvpha.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cdtbfczz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wipqkkcd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xtdrrxor.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bqwdawud.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wgfdefdv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bartfybj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ftljnbzt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dxiwityf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3tdurrcya.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jyjxnotg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yubozxnu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dqndnsfl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gchrqshz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mzmwolim.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dqywluod.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wktcqjvy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zocfosmy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ltnrcspy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cgxlzgyz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lacwiycf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rbblvydf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3oyvubrcz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tpmcycfm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3nymfotgu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3otfpxhdp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bzuzvhtu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3eapalqrt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3wgtvlbyd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zhdcwelf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kskoaoer.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jgpdfxyw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uaxptjym.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3spbbkcse.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sguemzbc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qddfxyev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jnjkhcpd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zhlbtujo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oogqfdwm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dxtidcgl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3suawassp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3eardibgd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xckudmho.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3egvfcoem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfyftaow.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3fecrggvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aboepepj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ihiggsvo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nwrkhkpb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jzxilnjp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hlvsizkn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ddvhxsxk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tpptnaki.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3mmwlkcqr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qkyvzljb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3jwikyqcq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fafzbmuk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3gboyqhhj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3okvcowyf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mldnawie.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pqakclwi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ojewfers.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3dhhfnpmu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fgqfvchx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qtymanji.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pubdfpuu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3iskocwrr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3yzmntfaw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3gtrpxdwa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ntivindt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3apxtxrox.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ucfrauqs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ibnwptai.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3iskufmwg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ukbysede.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bfjxkkat.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3yvwufnob.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xwquelpm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqxypqul.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3waxxezyx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3huvmizmq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rlbmbpys.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kurbiaii.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3swjsvyns.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gsihjjnb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cooekftg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vruybuzj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rlocvwqx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3labdunsr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3crgocwcf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qedsvpyr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rhipjjgx.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jntnobeh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dcuxudhf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ehsugcvy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wpmuvcst.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rpdcirll.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qulltxyx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ryyhkuei.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tcjausvp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3pqiadadf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irqmulcf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3vilxnejm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjrertgk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ylzropab.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bsssaurp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fkzwpurw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uzfsmbto.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kprbtqhi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lxkbwtqv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ryoiodxy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xaxwebhy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3arjaxqrj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yvbcrxte.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3wzakjhch.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3nqrzmuie.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bqxsnvsf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3esbciaiq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zrmvjpff.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ujlgkhzi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3uglnihgm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zfndqmtc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yllalsrj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3nqamtvrk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3avjtjtkl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fpubswlr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3emvuhzjm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3tibyhlvm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yavuiaes.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ejcfnwan.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ikfeguun.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3sdfmdldi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wkwvygja.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nkejauwd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bbtxozur.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3usxlckud.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rtrrqhjf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xhorgyzr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3uxqfzzwk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qoqnwgzs.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ucforbsv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3eoogrniv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mjqzuvqh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3iagtcgwp.html


<!-- 参考信息 -->