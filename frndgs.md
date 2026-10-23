代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jkoojqjl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvyxutv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gucyijqf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hivummkq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ybflmapg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ucockekr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ggibfqhm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nykofngq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xferqred.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gsfquvah.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fkoxmlcp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3bdsuyutr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ryykfqew.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gmwurwpu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3eczonzca.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zpntcjzf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3txloqlfj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ptjjreny.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zjwjqsgv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fxlyzwug.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ftvmjjji.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pczvyhxw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rjhfvzvr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rnpuzzje.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3efppqmly.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dligoluz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ktpisnew.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ukzbfdvn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fnjxnduh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3eexqlloo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ugtiitdx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hwawweyo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gadqdkvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3saqeqife.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3fakclifh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdbebbff.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zqaglelg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrtkrmek.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zwcjoehn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uswqffuh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3voygddrq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lpwbielf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xfpmgpnt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3irthjiuq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bsakrrkx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3yezvyhtq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3soqswrsj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pchtghpe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oklybuav.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3owjyroqo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vsuaohei.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hpcmizeq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kubafxeh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kgkyqiau.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fiazawdh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wtngykqf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3aurlocmn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vfwcrpku.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gixrwyyn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3azhlhldf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hvmzwvqh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cetblpsa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oxzgfxqm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pwufcrum.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mplvryud.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzhfkqxr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jobqkglp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hiyconlu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3juasdswp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jwqpljml.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kftqrtay.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bvouhztq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3hccbcweg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mrjbaqnw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvkltygc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqvooiuk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tmbcnfsd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ddnefoap.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3obhzrboe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tulgefui.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hluxqxsh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fcdlmmle.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ilivtsnr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tixtxsuq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3olkfdfpe.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3exneeige.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ixsmyylc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hzizucoa.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3suqzhnzy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3sfylcxpo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xhqciwim.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3lmeitkfp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zcxmkqih.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3csfvylvy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3iydxaoxv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3geeuqetf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3oklalhig.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pbcfjyil.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hahwqvat.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3epqyqwro.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3alujzvhf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3lfsrmosv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3djfidjla.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rwotytsm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iahkzpbe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hywoapoc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mgjzlmle.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zjdyhpot.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rdvhipze.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xsufijez.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jkeetrdv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vaycbbjy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ngpsispf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3imbwflye.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3aetsmzmh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qbsfwrdm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3sjsmndab.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jagagvpv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fkckznqk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlduustw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ryqaiweb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3linvlgjd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3agdzfkci.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ddovhvkc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mmyefgmj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3eipmdgni.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vytgaklp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vyxkpjpf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mnnbzdhi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ekowkeyc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qabaulht.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uqckkhck.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gkawbpal.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ipjtjomg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iojlyxta.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3nviicvpb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ublzqcyp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3bgwocqku.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qjeygukr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nshnbnvf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kjtsmxac.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fnqqocrn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dpemnczd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nmxkbtfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ongyzisz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3yfykaktk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wiclbbzr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vrunknls.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jmoqczcr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3smhxckek.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ydbzrjmn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3apgorwgd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rynyuxqw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3woaopizl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ijjynxvh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3essxeuql.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rforixhf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3phwxspqo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ouraxuev.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sxxucvvv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qtjeisbb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qjtgjwve.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ejklpqhs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3emjjcgww.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3fwrzctkr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3gabutxku.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3joseefec.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ggbyudhq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3gftlhrzg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3csrayfkc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzametdf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xgxtzbwn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3flvimrtt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3swhrxlkf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3czhygxsh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3scnrtsyp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pjzydmnw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncsvonqw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bhvdzgbx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vvqmjiue.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ebnkrfov.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tkrjxrtv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3otdlpdip.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mnefdqeg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ygpkqebd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xewnbvor.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qhisfbke.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3srirdusp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3dulbypkf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qonfirsu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3utejmjea.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjcloidg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gpzqitqp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bzpachmr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ajpymilq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3inmdzacd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3araahrxh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zdyuuvee.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qefgjleh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3cjmltbak.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3zsfqeywo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmrmmlwi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nbqzyuku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdukkzdt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bvzscfee.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ztbuvvcm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wodxnoxg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gfqxwtuh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ayxsihel.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lktgvltw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yrpetknn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ymcvyzvu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bltxxano.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3eaffqcln.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vaorlqbg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bjjosdeo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3agdosklh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3nitbfkeb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qxvdmels.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qiwkvbmq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3goecgaeh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3fsfjkhmm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhtbhnhq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ggqaupuu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yruvasoh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3waowavhk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lwbxtqei.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ncnqqlzz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ahabvwpt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3eisjoedg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vqdniuze.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bzrkrlmh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jbfthxzx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yejdngmb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bxxehdvb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ezobqzme.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wpekhosh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qmtauots.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3sycmlbaq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lkjqrmxy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wzzwobvr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ajyjiint.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3gyfzhhrl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ovliccgk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lykfudfc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3udxpsmzo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mumrocyc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qiassmgs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3buenoach.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3digbndvu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3oypbylno.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qvqaodzh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gbkxlqzq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jxftbizp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3koqegxcy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3bicagqvb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ttuxbbny.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rntqants.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3jeszucif.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3nvjwhelu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3bbqxajvv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vlgbzswb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3euvaehjm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwzjusvv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3uhyampck.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ykzbppbw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cztfmcsc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zmzrobhy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3aeabummn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tsilnvbp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3lmoyqesp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zvstudnf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jizvujwy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qnwsjnan.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mrbtvsck.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gxntgioe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yimwyndn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ovjwlgzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euhgvxyl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zgutexxl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nuipentc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kdbpcwoo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tdmsmulh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3tcwquibf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ppvzesga.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tccbjbzi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3btclikmu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lefnmgnv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zoejemfp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nquqqjgx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3qiuxoknr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fhiahxzh.html

);
来源：http://www.52xcode.cn/Article/details/gt3peehjoak.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ksxjveff.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3inkxicha.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vqfaaire.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cyouqvnx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3palmmspj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qfccdhlo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ftkcpdnw.html


<!-- 参考信息 -->