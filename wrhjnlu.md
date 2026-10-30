代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/goeqxigeb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gdpofczce.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqeawdvqg.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gdgyyfzhz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdjsurkpy.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gxlzohfva.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/glhgjpqfn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gaqihmluc.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gueidelmo.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxxacxcd.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gosqlehlx.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gclpmteft.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gsgxfmvtl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gkiygzxdr.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/garpgzjwi.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gvuzpawuw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gapsfcycg.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gkubzsrir.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gutwfdfgt.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gklhvdxfy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gyagzkyit.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gszzbzbzy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gfkuaphji.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gtiyygrgg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gvbfpwhys.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/glmmhpnwk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gtfzoglgo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gfedxirat.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gvrbxrhyi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gyetggyej.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gpixrbgqo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gqlobjhmw.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/grhinzrie.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/glliosjuq.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gnruiblab.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gmqlbtopv.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gimnekuou.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gryiypkdk.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gykmuibku.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/guposkneq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gzbejzvtd.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gymjdswlp.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmmrwlljs.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/geuykhvfq.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvdsingls.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpxfhckog.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnbwncgtu.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gozkjdnbo.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gobjklffd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gidkmzred.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gcwcgqbgl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gdtbzjtrf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gzzhyteyu.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gwkpcsyor.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/grksdvcpg.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gzoaianvx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gwnqmbvyc.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gryisfvpv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gufjrmkui.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gbomtdfxo.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gxkfqvzvd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gohbneyfy.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gmbbhnbzh.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gmufywefn.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gppafendr.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gxdkzjhkn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gqcridnfm.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gbihizrqd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gzjmuridy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gpaldgvwr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gksuuskfs.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gghhbrxwe.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gkbobnhae.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gqecdnckj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/getwfjgku.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gpslhefif.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/greqberiu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnlenahba.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gihehocie.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwimoamjm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gdrvqlcfm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwugtcgab.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gjnpherfs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gcwscgnzo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gacggyvwj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gozfwzagj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/givjyxacq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gqpblnoya.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmhaezxub.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gnjlxlilz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/grjcfiord.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gmlhfuvto.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gbwvwsxnz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gonheqejn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/glnxvqnka.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcnazxizb.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/ghrqprgov.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gbkxguzcd.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gcevnjdrk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gtbvffgkc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gwsrzvtnb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/genkgkwyt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/ghrrmeufi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gnapyjqyw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gavbcorza.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gqledqvqj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/glxoaghqf.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gwuaboarl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/glyyobswp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gubzcvfnp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gopnlolco.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gleednqrg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gycnhnixn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gynapptyw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcwqwwecv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ghfdjjfxg.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/geikvfqcr.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gctodkqfp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gkvunolcn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gwrxhydfb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gcvsvckjj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gteghvgah.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/guyslvclh.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/galfzkice.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gnqmmvjtw.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gkowzcdah.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/ggwyjmjfm.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gmoklncgp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gcxivugto.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gaeixydiz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gwpdoxghj.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gkucnbvfp.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/grxspzigk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gmdmdrddk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gwnenrtrh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gyzxnkjnm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/guohsaqiw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gblkbvjst.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gajjmtyzk.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gspenhzyc.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gafaiwwxy.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gkzzzsuzt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gnrgcnvhl.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/grnnouklq.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gbesnhldw.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/geiwyuvoy.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvdkdvpbq.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmcntgwpi.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gtjlsbhhm.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gatkifizm.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gpmijfjes.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghcyjoqck.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gtwumxwhc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gukpuvjcg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ggxjlwhzl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gpenceamp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/guonvsocg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gprdawgnb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gtrusljvd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gyhmujxbk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gpyeoarai.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gytbbzldu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gfxmatqvr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gefsxqzen.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gadkvscfq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gjlwsujxe.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gbjgpntsl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/giwuwyxyp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gcghfsuxf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/ggurwwvji.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gaozkhhko.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gvumcvpgi.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gtbimfdev.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/glhvzxezw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gjgygquhw.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gkbkzdtua.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gwerjfvsn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gvndunquz.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gqpbnzisy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gatrdvmut.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gyuzrcokz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gxmeflrju.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gknalmahy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gmhpydlzo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gmripjpel.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gfpmpfhdl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gwzmtkdlo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gwcjvtspw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqsjwcncn.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gelpcvffm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnxvjzruj.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gqdeamvfu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/glzapcrle.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/grpyvlmfy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gkftizqyw.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gzaqfmvyy.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gskktqfug.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gstsktrfq.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/grdejagkz.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gcehkzish.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gtpokvzmr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gkmfrlhgr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gepairior.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gxhesfglh.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/goisfprzn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gswhthrfd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gvrozrbwz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gbkvjdmav.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/glddhqdca.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/girsipqzt.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gmoqmzunf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/grtlmlthq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gxglnwgfv.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gaysujdiw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/glonjavnn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gbvxbdmmk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gaxkewucj.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gidwoifko.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gkusbwivu.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gqhwmpfzj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/ghotpobxm.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gizcgpbcu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gwvdlqwcx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gambxwhas.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gsnqfbajs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gwplbfaoc.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/glqrdvsvy.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/ghcaizeat.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gqypshzzz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/ghlhtzqsd.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gmwgzhfud.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gjkwfipqy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gnhdtmpnx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gshkvrerg.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gxciacwzi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/ggyqlvuiz.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnreqtspt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/grvrduocl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/guicdhoxt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gtsiyrcex.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/grchxztku.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gicepogjd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/grxymkigf.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gvaegdire.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gubmwlqwt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjrwdblwa.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gluvcfila.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gakqxoswj.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gbvlydmlj.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gsvpekhzg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gfvvmlssl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gewgjpkjl.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gvimuirjt.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gvvvcvwvk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gxtxvjbav.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/grslcfidl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/ghnifbwfo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gdlknepie.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gfynwrlta.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gqnuybixg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvypbawdl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gtjzplxgb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gaxyjqhtu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gnmrbnruw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gamkgwchh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gbsmcodre.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gjxvdtatg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gsbbrjzxe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gqnxsnboc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gmvlzrpeo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gssandwqu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvdninsw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gzzxpyhgl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gbrxlualc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gnwrcbgbb.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/ggnwiohcr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gnfslbkte.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gumawgvin.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/ghzjboiap.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gtitktynk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/grukaeipc.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gtqdzdwlv.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gwppsvtty.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gojhwrgcs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/goiyoxuyl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gtmazcsmg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gdouucgou.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gejlkuhal.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gqslntdjt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/goahsxqmd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gebujrvgn.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gmxrdgdpk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/grinvvbvf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gcirwwqvi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/givxqsbjd.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gjvqvpgqf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/guwxununm.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gkxugkibx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gbrlgcfch.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gxsohupoq.sHtML


<!-- 参考信息 -->