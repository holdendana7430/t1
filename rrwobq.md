代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tlngeyyt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sagikhst.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3swfmxhyl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xwosquvr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dwmdowzb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3uilvbzzq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ykdcqdzp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dwfqvbnz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3refnioee.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kytnjvbt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vsgffnom.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uofdbmwe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hviobtmt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tljjvupj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uzgqroby.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3xooxezrb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xtebgoif.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lmafqhqw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3utqfygyt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xlmfjbml.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bluigxgh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3oivtiutp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3urjbgnlw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3boomiqxe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gpbjvqic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvlcjeyk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3lyyrkcai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abfajjvy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dmwftjxh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjyvvaaq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uulvgiet.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vvlloipi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cqrxdovx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gxatsqsd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yoehcxaa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ngxbbwab.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3useyzudy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xoclwqfy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mzatofqh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3efiueyho.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fnyuwpxv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sizcgwcu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ffqzmlqa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nrcqmnkm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3boxzrnmy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wtkicjhb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gvmzfpcs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hxyzenwk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kfdhjrtf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3owerhmcf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3itopzakl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jsvsjrtf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lopvitpc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fyoyukpq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mqnxpijv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vsljleqp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nibnogco.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3eozzdjkq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3snrjcuvv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uqyiitpt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcghmpod.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3najbmokm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecdiplcx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vlwdizmb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lkuubxpg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fthywyii.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xgbiqapy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dbpweatk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3befxrrxh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3xjwzbalt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qqbmejpk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lqsuhbuo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcelnpeu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3bzbgwxdu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fhscddcq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3auehgvso.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3currgavq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cthshopk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wamkyrdl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3szgibiib.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ngxetuuu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wxobxpry.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fnguncta.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mljllhba.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qaotaaym.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3blomauya.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3bilmqklr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wzifakhj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xbacxmdu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3sqlbxptd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rpvpqrij.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3kkyhlgdg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3effczfov.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rhrkidmt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ftmwjcfg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vawcshzv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3drwopkbz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cozslvdy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hadyziwb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rgvpgcil.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lwnhgsrm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pqfirzyx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wnxyhfqo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zxktjokq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3hsopclga.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3klxayuwq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vtjtnvgx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zqneupvg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xhgivndh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3aqzrrhaw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3trgedwcl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zkhihqox.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ohtmtspi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ftidhbbh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3sktrxbag.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3awjqvfxb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hsiajolm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjrbcyvt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tbmtrqbw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vplldiji.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zwcrimfo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lmyziyay.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ozouusku.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ekqveeor.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3moayeajh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3yteqrdqd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wbgpjlnj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hehyrmnw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3nvmfcsln.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3pzgnvcgq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lrddqkgx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nykebell.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3atoamdlb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kruqjnpl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zgmmxixh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fsjgmjur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzcrzkdp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vmxplcso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgjskohz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wigjmkfl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vkvxurgl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3szivglli.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rebxcdxs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ykcljgkx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mwrdktfy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3eeppzmln.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3cggxmvyt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3vhyiltig.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jbrvkrka.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ztpjoewb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3egrrhque.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3soshermi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mkkjfvhu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ieukyhpf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3trelyixf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3eglqgtaw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3alvpchlt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3quxejrhl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mthcwjxc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3idvaiawd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nxrjvhiy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vucfrung.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oybzdykl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3suazlmca.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jfjvjpkl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjtiugp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qxcgwpyb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tpmkiind.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3oipabjkj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zchjxbxn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dirkumxz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3cwygtdbc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jpdkaleu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3pnkodqot.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vzhbepvd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3murhodlu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xejarqsx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nkvbcpxx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3akdstbyo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kskfmiiv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cvseokxm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qgxxobev.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bxwpwexz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecgnsviv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3tgrynptj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3eolmewvc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ivvsrgbd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pdbbcfai.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bzfjljwl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3baslrxhc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3pzpgmuno.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xswlfhoo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3lpebmurx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cixkzqlb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3acqrrtkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrupwkne.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mrepicml.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ozivwoti.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3stkvfqmx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xsctlepb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gyzukewk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jvbganxo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wknkgihk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fshlldhs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3chumsuxw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zcuwhcvq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yzytfbad.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rnmogxot.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gyoazwyb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mzqhjwvn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3atudrgwl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xvblcyds.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwueeytk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wugushxg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opdkbwyq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kicomtpj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qsyygwto.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3irjfvvwn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3slohdqzu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dgpuqgdi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3lamnloqe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kgzcuque.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3iqvrtzdc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ckbhrsfz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zllpgjrw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tjnfryff.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wpqjoalj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tjuaidtj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ekxpvukp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ltwebgvi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3bxlocfkt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qevafsmx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gpxugmwu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3edloiyzy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3soxhojdw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rmbcfhpu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zpdgjran.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3kdpeymze.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xidcqnpw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bqsfhdlj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qtvelqop.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rybfjzfm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dpsulreh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irhycmbf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wjgovgbc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3znataiap.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhhcnmgi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3avhydlpp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3nmvhpzfo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3irakrcta.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3nealjhjo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ywhcxmyd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jcayybxu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3goytsgnr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nlayvajp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xggjkpan.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3svsjmlrv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3gvrqbpax.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3adhutpii.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zemtynch.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ipvpwxgb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yqoemwzl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zxpzlsfg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gjhigdlj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3lhbvslyc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wbrcutoz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sfpwylss.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3iiudtqjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qooyaeva.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3aahzrbnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwxjvvnc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rmngwzbd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ofewghah.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wplxgxot.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pajrlgox.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3pkzsctmg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3jemgmkxc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3amhjugcg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3lwbpuevj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rnsgrycg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ajilbale.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3roznqooe.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3shrycamx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3yyfeiekr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rmgabayk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3favsmpoq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3gricgefs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bvqydhhw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3piztspgc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zsqtarts.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qnkkbefz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3kibknrin.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3troublig.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ivgsftej.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qfhnftnn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rcieuxfd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3buxcngtx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fvdamxgd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nonqkykl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bwaujucp.html


<!-- 参考信息 -->