代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tipixohn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2otpvvqfs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2okdhjqkc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uhpfkaxe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kpegpkgn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jgfdfacy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xubingte.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rpcvwfgj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hcrmepwh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2exyykilr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qaxiuytt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2udsipyzq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2efllmwav.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ssddnzyo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ejtifgya.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2brgvkgxi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2pjxkwfqk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2rtebceyd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnknzplz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hgfwgaaz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dntaxkto.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iagslitf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnwinqhm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqqjfkvr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wquqjnfj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nvfbamyi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kghklmrh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijruntrz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2myabqluj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lpkfgudk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hrbloolt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fnedfwct.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tumbsmmc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tavsbkkp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fumoxkgr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ghsgbgsz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lecbrxpa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2zcbdgnhf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dfsufcjz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2auorizez.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdbcaqr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ecnubuzx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2aayhawiw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2trislorc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2buuttbvp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2liuomqfj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hfjglxkr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zbeydmlr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ohpzntka.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2iriohxjl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ylrrocpf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bhewyvpr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2simutbzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tovyrfrh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jjsyqrsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epvmeufi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bdncdteg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtekzkqt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lwdnqcnv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ueliebbp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rfglpoij.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftmjkmog.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jybfaxnc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2nqhnxgts.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ubxnougi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ctrbrczd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2atqlgpqy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2stvsxrch.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2highrweq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vbmhxpdz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cmccshor.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lullqgmq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bgqvrfty.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fzuvkqxt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qbjybhyn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qtfohjbf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2nzjkjjag.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zzlylpcy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cvmgzwtg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ttlfpkph.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rpjkwius.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dxmtwesg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2svbrzgnq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2plfldvam.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ilzregit.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ndrxdwme.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bobvxbid.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uyrmlvxh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gjfbgrxh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ocpctrqh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gamhmmsu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qluihqeh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2stupuajp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2moclzulp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2prsawlhe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyodvdvm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fneccgol.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2qohanpeu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hbqzuivw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ihhedttk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxhwkxnk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vlnbcuyt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wqhbporw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dmimrgch.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tbhjlujw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lqykfeef.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2pfkcrjua.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2qqnsbqxl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oyvunuup.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vezdelai.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2adgffxoh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2cfpslmkd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2djqttqxp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2goisvscp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2zwqnilfz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2puelgidj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2sgcvaqns.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hsxgykii.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mljdeisx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vwftugsy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zicsgbdy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2dzwbrhyv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zxzwlxui.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zgnhmbec.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jlrsnclm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2grqpkgcw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jupfyzov.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bnkstqmw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lcsjsjuu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2btndufht.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pgtetrpz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mnkpqabk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uzijfehj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wwxuwjzn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2imjpfyjc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aaruzxtj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xuegtqom.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ygfambfc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pvzybiny.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2kvbmghcn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jwwpmvab.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2cowfkito.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxhpfhrk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nwadwgjw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ycyapyih.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkpuhagl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cpgvzgzu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mjbpmcrh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xsqaruyd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nisqbngk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wmdbkton.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2duxnxiyu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lfmjumng.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qlqdezsc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jbvdmbhi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2cuqpqppp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2uhcllfiv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2gehgzphn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nbaxqkfe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ltkdumvp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hwltpnsc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mcmzdpkh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2nqqjlkyr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ujmynicy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2geqsmzvd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2pmlgpvxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcdyvyuf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pmyqpsey.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2eldqqaok.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dmwejhpc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hjxsoeor.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2exupdrlv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wszisexk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xfqputis.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2iudyeepp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qykbshnx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2flhxuzvs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ckfmskrw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2efivettg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2owkvvprs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2akpxvixr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zezvpurl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2tdvqymlm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gueqaprt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jrlzzvnm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2aggbckhe.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2bslswitn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2uxmywzal.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qsccbokf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dqqrxwup.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgcsohep.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2kntdvudx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hksgwtnd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypsjdywh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2spfzwaxs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2cpedowyf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fmeolklp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ninpweex.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vivdkzst.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2letsfgmw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2drptobrt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2oetrhagy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rimbrcnf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ghhdxvho.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eemjhxnt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ieijeziv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jdfdmmke.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bsnxsaks.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ttzydplb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2amhbqvcq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dyxgkhac.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2qnueuudi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ijmrqdbm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2uuglagqq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2bhzeqhxe.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2thaimzpw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nqcqoryn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qtrwvzbs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hjozkyem.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nrmahnih.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ontssngv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihlrxxhf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2obugkbho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyotjshh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eoodkbxd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cbolpcno.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ujxxadhp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sxvuyxrw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yktybrge.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jdlgqriy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tlajimte.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hkairvgj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2loaulfyh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qfqeftzw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2nnxtgzuy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwxytqka.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aazqpkct.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2yxqwyrbp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nosdkgdh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2snswmpol.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhoniqtv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2sqxhohnb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dymjtbzn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nvdlduyw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2pqzbkosa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uwxzbjsr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nqjromsc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vmcfqhiu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ftjpgbhg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qcrmeeun.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2kjjtkcvf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xdmfwhic.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jqrgsmch.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bgpqizze.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wvlxrwge.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bylvwben.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2placxugw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2hztjittf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2xpftirjo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jshluxqm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bttpoaza.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ccjfqphc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cjmwqkot.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2pyewjqfg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kmukxsxy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zagqjbeg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pfszmbyb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2tdtwaojy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qjynorug.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2pnybdkln.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kbbhibog.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2byzfkypj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gxhzvvus.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gthppwkr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ljqwwbdx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jfvjcmqz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jklqvzdz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wleuxpui.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2inwyatft.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xhqmrewi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2cmomdrze.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2paecxvzz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2azznrhvz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wxahyhom.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2kyhvokjd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2bzxrnrow.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pfvbhxfl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zdduglfo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fhsryram.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2odlbmuag.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ormqnepr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2prhjcwhk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2abgmqgqv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ckmkhbzk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qpalmikj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2fpuqirle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blkvdbxy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fjflsjjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkmpnuja.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zlerxoec.html


<!-- 参考信息 -->