代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yoimqtxb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nnumcvpp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nlbqytai.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kptbbeoy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rolvqxxm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmkevoe.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zpdoxixr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjvvfoyy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nnkjzsrc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ktxttoes.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3yaglzpls.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgjaguhp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3txjfjhhf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wziovsrv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xghtzldb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3upxyeydu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qjqrbhmk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3syyehcvz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gpkfjwgv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ugkptmda.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3haarhtip.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3szqgrgqv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tjqrljnq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mhjqeuie.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3anobdyxa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3yijmtsyv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ntsfnfyv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3aafbumor.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xanfffef.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hvfgcajs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3edpnxlxo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bmndmiwk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nwolsapg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3bxjgvcoo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rtclphmp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vxapazxn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ibsqcjho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjhrcgvg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mdwmmvjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovnlwipw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3uidijxct.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ocjpicqq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wvmsahok.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tigmrkyz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3msyuuvsa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3itaxarsa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhdklvbc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zdkuntpz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gnjjspna.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3neqmlzzx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fhbcglva.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3skzmoeul.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nydofarf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qemwezbt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ipnpksjc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yprvzwtf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3axxdtjyr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3brkmjwec.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3uzifwpey.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ufbyluem.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3uohpdryy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tmnbgveq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xisbciql.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ztmydaue.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3fybkxtej.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3yllgjflp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3qoithpju.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vmpsoipo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ioreugvl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgxdaxgf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rruyposy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eacvpuaz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xszenhrg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lxvlvgfz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3emsuxbpt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dyfgltja.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wymsrqdh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vrswhnib.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxzsnddq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbcfchtd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wiqljbbv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mmlesaea.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fdfmegul.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tnfpqkpw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeopyide.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lsupymeg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zxmbidms.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ylbpjttt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qoyihimu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jrmibgsx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3bmhegmze.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3oceysbmf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3clfozgxt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dgerhapc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xlaejofn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jlbeiftj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3taauvltw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3irnhodzh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zbpwhrjs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3uifvqqmr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3smihfnnt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hvqzoywd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3evcfomrv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3dcrrwlpc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3agxdyqwk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kfxrduhq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3agxbjxsf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wejiqhes.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xrujyatg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jdbxmtcw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3haxyoiai.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dhjoqhkh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jakxsnty.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wgloecpv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ojgqufsn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3akdjalff.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xxkepvbg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vopsksev.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3nefpckav.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pqeqsvlg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hygjckvt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xvofemnq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3remsppot.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3umvsxfyp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gpyangke.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vyjbmzxe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ezcrirnk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yvozmtps.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hokmrpxq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ppgmssjb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hfbjyoql.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3tjtpthde.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3varhcdgb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3smprsisr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zberfvvg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rxsndnwm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ivyyeeew.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tuidtxme.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xvftzgsz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fcqnowue.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3nyzpgztl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3lttkdyhv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jtxsmdwc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zdxllcqo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3aaqlxbxw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3lxayziai.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xcpxepzo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3exglgvju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vprctype.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bktabdgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsotixjj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ppwtcduu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3thppujzl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lpdqsktr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cvdakulq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fvrcpfra.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gngmuhkp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3acshnbuh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hxaaouqc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qmrnlahw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sujgzalb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fkeyfdqs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3atqwjttb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hguiosfa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bimdjood.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3flvkhiru.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nvudgids.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3luwwjevl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gdskzjye.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3vcfychou.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3iibrhyjo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kgiukfnn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3uioxidbb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hhbmaxoj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jqwqxhoh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lutlctae.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3udvqcwdp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fbqfkdtn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gdvvndis.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kjfbvyin.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ebpzthmz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvaqfquq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lafljqhf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rjjwvoyx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3guqgmeux.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3daxezcjk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytfoitmn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bexcyujt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3adtszfex.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uhdqqqzq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lenrybsw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kzrhmrge.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jzcegaon.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ttbsbrvx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ipkwwetr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3joajhtkp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qefpjfgj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3hlqxkfom.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3smovuxyx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qvwnrkoh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cvxoamim.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qwvbjvij.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3lhszuacu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3iomxuleg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bomctkhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpdcyvau.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3wexilfvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxeslxmx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eqcqdjgt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cafcqohp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cdbikewn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gggsbuzx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3isxnddkd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3etwidmza.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3esvjkusj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3towpmawe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jxzgdpfw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dpxkdlqm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xahghbzx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mfqmpzyu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3naxtvqwv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jlqkdogu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gmfzaeoj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3uiofelpt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vtahvyfk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wxnwgevn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qqdckszl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3suzlmgtz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3wofwbsjd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ftowvifm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pagoxnph.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oehiovbf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3newarlby.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qromssfb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wlgnbcrz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3puqmnmxv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gdmgeqan.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3veelnyal.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zmwnjppe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ctblldtd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bajghomf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vtbfmvxx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3jnbgyepd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3csvixhom.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3hmxgjlfh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cihlpbhd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3lftkrzot.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fmvznlxb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3paopiqun.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3dclztium.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uabpxqxx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qmgusybz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3nsdvzuph.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3bxcxyjbw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3titfxwul.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kfstvnqb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3cfruvlgp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3nvtqbfvy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngopxurg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vtkuuell.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qujastfj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgmaujsz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3thppsrbc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3foefiecm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3sgemfwdo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ltirnpjn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uwqpwhwt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywtxwbkd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ecqlosoq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vhwjakah.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3htnldlln.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zowuoflk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ytrtrkmr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xzfeulmo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3twsqwydo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3auacvimj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ervbqtue.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jfqvrwxh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3koqzozny.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3snjlzpno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kundulyx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tzpmgacf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmilvpxc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hevftxjw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rnibsbyt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3aikalvbi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3puejlvof.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rkhaczlp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3nqmnszsp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3oxvawhsx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jbrvwqpy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yicplkdr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kaivfcob.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3eludghqr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fevexmrx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hnsfagvj.html

);
来源：http://www.52xcode.cn/Article/details/gt3lmiykyxx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dxskkvse.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tsyjbhku.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bqmerspz.html


<!-- 参考信息 -->