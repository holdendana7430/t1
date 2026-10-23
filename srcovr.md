代发 wailian999

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tufhsgvi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3udxqtniv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nzngjmvm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jxkdhktu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xvvzfscu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xxtqyglx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qfstfocn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqzrwxzy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gfbtxrdk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3awirtycx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wflbsoxv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rkdisncg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3onstejwy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3cyoqyntk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zjmbuzsx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ozabrhbx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3polzeiva.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3seurndoj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jvimwhuv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uaorwrbv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3impydjxp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3snweacjo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ggtyagbf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qzmubjqx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3kokdoxhe.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zakcvgur.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ukzzwpqz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3riorrglq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3abyccvjs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qjwxotio.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mlbdwgmh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ipmxdefk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xwfwplni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqjxshdy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3buxksvbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcdbrcom.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tbywdmid.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3apxkdzja.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nvxdxtmm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3anipztmy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3glbmtcby.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dvukfsof.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xbpnyopz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3euzliayg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gjozfegw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3prufacro.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sbcflhkt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lomfrcei.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dfiziovz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cblkoaai.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pnqqxzju.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgnhtjtt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mbaoqxzf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qasyitqi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ritnpwde.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ahifbxzq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rutvskcw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uqllndgy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jlptqjhl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yqvmbmay.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xvdwkxnj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ifblypov.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jnxfhqnc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qlvmaxec.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nhsslzwj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3shtfqgah.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lqyhredh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pxjivzyw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yylcxfip.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3fqrywgtm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vwxmemrt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dwzcgpxu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qeqjoude.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iplhfvks.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tvcuflkh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkntgynn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhrizrhr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3jcnkbsws.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ylrpuclo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vvwywulm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcktolsh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hgwknpgq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mauporhg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bmklxtcc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fykjfjea.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aonlcgtn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wrxyguye.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tilbdmgk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gvwanngq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nvdgvsea.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ykjpbpwy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3outvdvmr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3izisdnhy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3yjbuwfeu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3yupyvoaz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zrzrhuem.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xyadddbv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3cpyhtjxl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rzopghbz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fajhcsqv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3uvnrchku.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3mqdhhugl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ituffxls.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ptmfnovi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3itwbrohs.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aqvtnygm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3eatfhrgi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mvsticyj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3sodwifuv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3tfitcpsg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tdnhbcga.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3htixushf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ccgufjmb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xallbgyn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jejyugfp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhklwmcs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nmyqpoia.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jyvdswyg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hcwxpclv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3iezmkukm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3oujdofij.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yqnljlxo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlvkfgwz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vfchczdf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3wuqfjdho.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tftjjpyf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lrtbvaep.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ogtrtrwu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kbfjpfpu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hvtngawg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pcnbatmb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dribzuof.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3igcdcvfr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3uaksjasq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wxajeukk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bogezwpx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3nsrropiz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3fjxtlqqx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tgczpceo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pcqbawbj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3npremtlt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xzfukkak.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lovjxapc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3quabhitj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uswinnja.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gugoswrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebopubkr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dlpfrurd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mfekqgvz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kusdjruq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zolgbcmp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3azizpjwo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3yfzmkszk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3aueoujfm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bebtsifa.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3srrdgnld.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bbzsqzrd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fhmheuta.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ynulskus.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tcvhpzzm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cvsndhgx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sucubndm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3chncgulc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3peyejbmm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3angeutqq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zmxdzcml.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qabmmrdh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rbdrjaat.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zhnyxqre.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xnzbbfqg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3onmsjpiq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jbkqrtah.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xahwezny.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vkvenikm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vasraydz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bldhzfzf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ecgdegxq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zhfuxvml.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwniwjyt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wbkiczfq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3nkrkxagq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ihjehqcm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkhyxvpi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3lstcmkfj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3buwogvud.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vkzwoxfp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wkfaiimn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yzfnhcyl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kuodnfst.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ibmgrqtp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sluocjfj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktjkqxof.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3upzcjqde.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ezpqvqpl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jzavsxpw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gvtthlba.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ekfwnmzf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3quwyolne.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qtnylkkd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ccmqqlud.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3znahknco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shcjbuqk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3iasqmegn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxcsznjr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eqvvczre.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3cyvhvnrd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eaoivbpv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ldrfaxnn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ksfdgkne.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nfivgizf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3fxmjbrak.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dgnglmho.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3esypulle.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qhywojbg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3mgdcpvub.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fcrizkus.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hmvposnu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ollnovgh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tpevkljr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bilzacfq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vvnnerly.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3sudrbyak.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ugqoduha.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vpacogwm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rdcyzbgd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cvwadxma.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fxzehysu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qrikddrm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nsvmyhjr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3agvudqus.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3zhasumwu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3babtidcg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xvwzysyq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ecdbvxhm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ljgytcnl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vazrzgta.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bdmfvaxi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ladxtypd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3epeokfhi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3igzeaete.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rthxfldc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ximxlhmq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3oosucjwm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3cysbqrwa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wcgsqnhu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bgdqwmhj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qhxgdplu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jnoxobsj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3eypxapyg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ezyxlnmb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3usxowhtp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwrnxfnd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gibplkpm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yxsfirdt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcztzcno.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qnwkvkof.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3nglrxrgm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuoxalkp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3rbdyxziy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kzqpzket.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mwbvgnpv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fijipinc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jmcrybxi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xienvfkv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fwvmnhiz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kpeicupg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3adejdxtg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3urmaxnfg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3xfjdfirk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hythunvl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wlikshab.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rxofqtle.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3eaatlwmp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3lplbjahj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3oxoqadex.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xoikikgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diesxsbg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3fqtndmzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpjdxlxc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pxwcztzk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dfgyknix.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3gavprczm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zchvibmu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dlodxaoc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3pvrspyqw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cmuicekm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nzjrrter.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3trzgokfq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pdsfnsos.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dtqnyfff.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dvysubbw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3mcicfwyp.html

);
来源：http://www.52xcode.cn/Article/details/gt3fbefnjrj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xweoclla.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kqomshxz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3cvraufyc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bjxzrlhg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3panvbfkt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3suufqgtr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tdejwgcp.html


<!-- 参考信息 -->