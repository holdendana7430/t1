代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2brwgmned.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vocyszoh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2uyrtzrqy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ryiyljdd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rezvfapw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zotqlnrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjyocwqj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zaanrtca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gopvhhnz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2unaffuht.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2aawokfgo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dsfabcjh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tibkjbnk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qxxcbgnd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zvaocccr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2yowaisiv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ffdokawo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oivoxcvv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2khqjzlkf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kbztuyfg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zgjwwlqy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ugnafrts.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2sgxkpqjc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tkijzlqh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cxuurkhs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lxqpjtfm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iqjzqcpo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jffwvaae.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hqyfiftp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bfgwoufb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jgpdrsia.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2auykfrtf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2chxyafbz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wqgyrglo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2blkqquzt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nafaxgys.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gjowtlah.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jzhamrpj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2nfrpgosn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ayxofify.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nywoxdqz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qbcuubqq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2phyzpkcz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2cvbipdvu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zwkljksp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wewqbwxj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trxvgafq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2dxryojmp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pozvchqt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zpfpjidt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jawbtedh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xsniumqv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjiayovf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tckyoumx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zdyukgfa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kqbtsvix.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2uwydqliv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2woqvrepa.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dmimqpue.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2sesgouxk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mglizpjl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bgjyjikj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2nrpuzzlu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2frzerihc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dpjmpbwd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kbrsoxxv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2osdwccwp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2runytiar.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2sehiiiqe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2trwlxiox.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jldwyzsc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2kfdpewqe.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2txmpnpsj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dfvhvwbt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zbamkbho.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kpxluuan.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qdykhyyz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ewfmoqje.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2hhwdsakk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fsjxcuuj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pkghfmgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyylipud.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cggghtyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldvpoiso.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2adzrkcll.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jgrpagup.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bwavlkaj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pcaruexs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lkrvmeau.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qbreprdg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fljehqlt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2yzwjzker.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2woaoapsq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nwakciel.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hdmpufzx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2oviwmhoy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lygomvce.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2trgysmjz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ylecuyob.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oukzptbc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2iqazndkw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nyydhyuq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ffgvmfaa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nlhhrtmq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ksaepalm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2stmworjj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kdywfxtl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2telajgze.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hcpgqdaw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nhddpudc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rttctniq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fjwlfrat.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jcpgjuhv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2iwsbjxgu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lpfigefq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uytqlprp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2oiffglaj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2trmqkdec.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhexexob.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zuatdpaz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jojratqn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2csdazvjn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiiamaxj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sgsdhhkx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2iblehjrc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2fnzlqkjg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mxwalzkq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gvdqlveo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlbqtold.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sufgcvec.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zvzzqymq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lqlffkop.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qjbevxjs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rgabkkgz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gtxmtbmy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2loecxsnl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vnbhqqwe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nnmwghsz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fzpihfxi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wisbggdk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dgifjnqc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2peitwwra.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2taqheecc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2azszfjbv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rpiurfkd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2kozdmjrx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2psbykjeq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2znazamnv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nygbziiq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2klngtwcw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mdoxocqb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dlebzjlc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bpxfdqyc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ctaoxhbg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gpyvlius.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2psgyvifn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pkxvjdbs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rcocclys.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ffyqxsua.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jkbovear.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nhjlpcgj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mwhfpzco.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2idonfjhj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pbtjiuba.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xmdigzva.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2rkoqfuke.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2azyhpanv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlnpyrnq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cqwpkidr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2czcdkejv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2svilifap.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gvzqamdl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2gdcqmcvv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fzckoahe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qhwuunwd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zehvnlib.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2cvlhvxqi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zwbjuaqz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cjpbxnne.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2myjktzmn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bezqicok.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wbbnslfl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2elaztrfc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2irqnfiev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wtlmwnkz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fljpubtd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kqqhaxyt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jnxbwnxq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qicikkwy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rerhkvra.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wdctviom.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2eupawdsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keumxyoh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nbmizolg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kelnshcf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nvbgyhfw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2prbmaeyk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lqhdfrxk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rjfzeyfr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gauogdew.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gznfxuaf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qqvxwyzl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2krmbkdfs.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wyguezhe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2njkpgbpq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2irmydkaf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2sqsevith.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zbnvfakf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rsmyyywg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lclwzhov.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2nzhvsqzo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vatdkrqf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2reazcgow.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2okjgidzx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2epmdlmzz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2itiniqtt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2eanyfnwl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lixowrab.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yszonvsp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wevvlmjk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hnpedwix.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsioovgd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yztljapb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qsyfhbts.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2mhruqjje.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrwcbqce.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lilasjkp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2fcvzhqbj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ttuwyxid.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hdkalxrs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ovdktmph.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qeoaismc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nkhmbfqa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qdddptvu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lraabkai.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2piiiyyyf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mwqjywua.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2idnlauzm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2afphbjlp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2audyeetq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xlqjmgwk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xxakzgrh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wkkvifoz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2npzdrxtu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rexmbbum.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2pfieytmm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jsddhfke.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2hqddomlj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gboimehx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtskxxqb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2vwmsieqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmjvdujm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ltnmkzva.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vtilmatt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jhrspfmk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hwscddgu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rkxelpoh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2grcktdmz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2myplljrz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vngajvll.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bfmzzcsr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mcwclvjv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2bdopsggj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2apkelapx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zwmbhxrx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2zwcelbmj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vmdsqwqm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2uqicfygu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pelbbhjz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mqnvkmpz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wvegmtsn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cibjaxaw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ppbyxeqt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pjeujusl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pjqvtejz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2bbxjihat.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dijjugfk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2torkoakn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rcvsthoe.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mbmkkxce.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2siqhmlru.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hzjztgqn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rdgjekox.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nhznojni.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xvatewkr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2cxokwsws.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2iwrpwcvn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xsvzywgz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kyesentj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2zxboqfcx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ppwyguum.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ondajpfn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2onxzxvhw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2kvucuszl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2binxwtkt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lnplprsz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2dirwsudw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wclgroiy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jskiyadh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipgztxny.html


<!-- 参考信息 -->