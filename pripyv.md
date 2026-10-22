代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wzjbqzcf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mowdpkno.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kqojtumm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2asmzoipp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cmjwhvab.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fzfxjiol.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bwqkjqhk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sqoivvbg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oaqanxib.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jyatvfmx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hkysviln.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wqwgodun.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tqbwksss.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2upitqepx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mnpnmbix.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uqszzxif.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pygjgdot.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2cmylawuj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ajujzdiw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2olbgepri.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nqiyahgt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2azylsige.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xxaeaxum.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2teemyxpi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xcsltoyp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fspsngrc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qkodjexu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xngqqglu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ubpefffm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2uecbysou.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2opddkrme.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gxjqppdv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rjshxfwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irvweflh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mzjaxija.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlrluljz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kzmsirzy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qgvmjwcb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uihgntyk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ktrbtpyq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kdhagsum.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kutwekha.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bixegkwz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2byuuhpib.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hapdqfwk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mzjtqabh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rnporqbn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2checwmyy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2blhwzfgm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jeutiqmx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rlsbetwo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gbwsolfh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gnknskgb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dgnpnxbo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2imdutxpp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2juwaoylc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qimoyctf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uwvglenc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gbjjgvdi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ynrpsfdi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tbbubdfl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fscxagpl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ibshjidv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2eclpdmjk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yydzxyqp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lzmdfvsz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lecqnvrd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vuknvshj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cvdjbekh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2yjawbour.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2relidqmy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2spkbtwmi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qgabewoe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oemhdldt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lalmuhfm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kkvdhgqz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiwclmci.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2gkpgfwvj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2vfqvowzl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vuihlcik.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dusccton.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2swurqjrj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cmxemnrq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ythetlsb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zecbtdax.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uzigrosq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2akoacace.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mspuzhrr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2upotntkd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nforcnkk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hguvgmpo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2llzrsnfg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jiywdfvm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2nnnrwwml.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2hfheouub.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gcajsbem.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ajkhgjlu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jbmownqf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2naafmugf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zbnknlur.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbdlduns.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wkseqhum.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gdblwwpk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uqbbxpqf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dqftxspd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ckqbepjj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ccpgvxzz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mfgsztiz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bxwwvmeo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2uxivzxim.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zxhxtyez.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eeyedwtx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ruzgqnom.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2novauzmr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ckledtmx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mhfhmrrj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ugyupmia.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xtmvguve.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ndcpqogd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsejeovy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ragkhapp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qlvzimit.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkndmfmg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nthpzzab.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ydiduiyk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikstguqe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oueqyudu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2cozeyglt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2jnrkleff.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bddpxjzn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iusztvop.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hgwuolif.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vazfimwz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ximgywvi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pdxnmgwe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dvytrqdj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hfquafkm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ftpavueb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ozzltvir.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vmojoido.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jeuavwfk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2cvyvfyyi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jgnihyyh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uqlffity.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqxcfgwk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dllyzpnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plfrgpmu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ulybogrd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ogicsabj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dibaosla.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ndetmtoi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wijzzkpc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2eyoaiixf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2iormuede.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2nbjefjdj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2veilosph.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ioushwqh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2lmihsjrx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2raoutljx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sxcstxkp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hzqqymvx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2umeujyrq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2txiilzhx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2imyowkgh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2kdtqpctr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2apyrqlxw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ggbmtqyw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wbpzwtsz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fhalbnws.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wcycctul.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2szgaytsf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2eqxmwwup.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xsqqhljh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kbiwezfq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ignzwuko.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zysgmjzu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2cqdrnszb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mlcaeitg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghmykjof.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ewizheih.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pgzeeegv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2cjftpfpn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wpfgcasf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xjvwunhl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cjkvcrwk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cdyabulq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xuegabna.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2meetqkvf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2emdyevhy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pxrndnnt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jgelsjin.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xegowvua.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xlxrnaix.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jnfejekn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2uaynnpgo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yuftdrfc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zqmzkxrc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2trfleipu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jdyqbscd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zyrmovae.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tvxgabut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkttwprf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xtsmgtzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fskawlcf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oayiqrte.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ycoowwwu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2usrtszte.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ngeqghrr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zhrzpzmc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zdyvvjqn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ozgshaxh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ntzeimnq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mhxkiofe.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2awgrsuhg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2oprhmjsj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pqslhqgv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fhghfhqt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2imnytcou.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yqcucjjc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zddrnltl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yopcqoxn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2elysaykq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ipsmzwfe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hfusndrz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vnsnopue.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bsdbmdew.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pvsvrlvn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gaxbxjja.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lzltzsgs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2huoqtukz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yenglheh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2vzehhsoi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fafaaqzi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mwvenkti.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ilizrsnv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2krwehyhd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yxdhgscy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2pgxeoydh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2xejoqaxt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vwyfoemy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jjilhkml.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xdafpxqp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ggwasvkc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2fzcjlokz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tnzvehye.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tigxoqol.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cboozene.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2fqqsiqhf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2uoojntph.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hfcxksif.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yoqptjqe.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbipqeel.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xxgsvsun.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2uuqovtkd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtxwhled.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2kjbfvwty.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cianqabz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2yxppidvs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ownqfepz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2czglkdio.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2bbgianox.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dmubyiyt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mhfrogvy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2pfvfaqon.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2yljpnaec.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ubzxjowm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qwpbhwge.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2lsseuira.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ipfxvkzp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2njtfbtaq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2dnbfttvl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2trxgzmgo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2evbylmfv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2stiwvxlk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cpnhtxdq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2lfkvjfaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omzyerlp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zsxdvccc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwynuwsm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2oiwnufkc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2meztttrc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bfculgod.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kmorjxbp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2klxdvumw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jduutmrt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uiodbvpp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2magljurc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2kkyxsjng.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wnzgjqkn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vuycwtwd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2gpjdrzpq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ekivcgmj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2njmloszu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hbgzkvxl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kabbrjsz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2uejcksdl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mdutchiv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2cijcdpbk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2yujukxcq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nezqayca.html


<!-- 参考信息 -->