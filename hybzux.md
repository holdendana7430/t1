代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wzqpzask.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2cbffkqdi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ekylfuub.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mvzmxpek.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jojuovqd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2afbegnol.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ujbubkrw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cfuovmkd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2yxcbxlob.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dksrrfom.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2vuxlytjw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2obtqgerm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2btifxmuz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ilmdmtca.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2zhnlyyeq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bavwdhkz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kfmeyfgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzyvknav.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2itxcybsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xspicors.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gwfpbzeu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hudtjjlq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2euoefnmh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vgqtnsqd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jydgumrm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xnlpyutj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qussoevx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mydxndlh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eqpwzxmi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2prkvnhdx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hyynzjdc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tkoucjbs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hhygfrnn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvscnwtc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ongbkcel.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2czrrrcnp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vslcqhck.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hpvvvzbp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eumpsozb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tojaurlm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2eskhkiae.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nrwwsdlf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hejksulg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wlgwkxzf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2cbhchpxk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wnkdbfkr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lckrksac.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2bowhrucc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hxpwhqef.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zppltavy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2blmbdfcu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qafpejwm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tyqphjmo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xndypcgx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2trzopazu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hvopmmwh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2debfizrw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ucszflll.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qwmhbike.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2otayrczd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dmtjvzkf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2qdtfjsah.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2spaouxjl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ewhnzmei.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2medyukrq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kxvapqmt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mtgwoeog.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ngdfeonp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2epnreewu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fwdidxab.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2jmgyxseh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hhkpoirj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qgcktcqo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2aplbjuld.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hatponcu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hsjosqoo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ejakxzel.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rxssrdyd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bchwspau.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tqwtkguh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nlfhdgrw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2cwsfxvuu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gxwyxsmk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2cxfozafw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ullwwqvb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2baanoxdj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2retprswc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bdmifife.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ntnnvahb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eyrwazzw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2suskemkg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aqzelwsy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cauommuh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ojnkyhff.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hsskummc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nfmvcxsa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fmtqumub.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pfgztjio.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2nrsxevwq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xkumyerg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mveumckh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vkwhurgf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2erqrnngw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2caidgowp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zqnueavu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xjxnhgnm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2bmnyoewa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xabtrzhh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2nuimexyc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rfjvttst.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2lzllyfzx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ychqrpco.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdbvlfkr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2onaoicmj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qntzynzc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2omomnsjs.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ztdktrnn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2iznwfpwa.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ifpmpuph.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2kjxyyboz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2giqeojyb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hycqefcr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kiimlhmv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kshdhjib.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2eflusknc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kfrihhym.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ijddgtto.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ilwyfyal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyculskl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2orrkclgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgqngvtu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2bxrhtvyj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zsrslrvw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2alwghbbb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2udbqgqby.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2evnpzpva.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2oefrjrke.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gyuezyou.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2cnfoppfv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vlvdfhga.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xndtwklv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zkoxochq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2lgktqfsb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fwulydcg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fzjmwiup.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xvjgzxfj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yhzpgxhy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2mvlzpbyy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jwnrdixj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2gccvuctz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bocafeqh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2lxkoppbf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2rtkturkt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2beudksks.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zcpxcfwn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2mmkdxplr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fvsrlzya.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ceuphbwu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ovqyknss.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2uqxrsszg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dcfnzinv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zidcwrww.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dsibrjvk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tieqqvay.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2nmxqteil.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2tskifpyt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oagedafm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2fopxhzkc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xmdqbexb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bgtnliet.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2afzvdhcd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gxonxgdx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2sdlgkkfs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2htvdkjgc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2whdcbuin.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2opfxddjw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2eibozzxn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iinxnqye.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2kgtkfdvy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2btoocxmj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ycvatodb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ubhrufva.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2acfhzyaa.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rmxguxvt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mkkqqgyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdoearqf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2thbesoje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvyispmy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cptnqypi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2gndwnteq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hiewvaiv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uwvdmyzw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bvwukuvc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ghjezhbx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uoycamed.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2qnsyltdl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ynnrrqhx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2sigjsuup.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2eoojirxo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2cuvjkaaq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2bdorfnyp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qrfzuwke.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ixnxmsas.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2dwnnlhmb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbaahlly.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bfodiyen.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pojzyooz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rbddncsy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cootlwis.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fezlczan.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jyzfppjn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2adhqzkrh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ngxzdyuz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2icyplfmk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2uceuohfz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2mvhvzihd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rpvcuedo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ycgvpzwt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2szwuqcej.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xufggdnp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xyoebyja.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2buofirwl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mjllfkkn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zthlmoqo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2imrkrmxv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xypzlhha.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wejrmlyz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2reumojkt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cvzgomcj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2sningolm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmqpdviq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vxltcjhz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2lhnffcax.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hsxhlzqx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2qzebaadt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgppqdpl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2hiwywvok.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2iixdiysc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dovvmnph.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2cdvuexco.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2erscmhrd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijiqafww.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kvinofor.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pdlouufo.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mojgshlh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ofrqvdwe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2entlztlu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ogcqjatj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2grjstwag.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2aerhmsyo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xkpalmtp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ejfrjxsd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zpmxqqds.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2arvgicss.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2orscksya.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dqbsunue.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2chjfxteo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jvdqvcik.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2pgrgfdgp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hkhlkpvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kndxixrx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fptxndqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jagqhoan.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2liqchgcb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2iuqpvruz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2euwvpwgh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rmayvsgp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zwkbqrhu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jmdzzina.html

);
来源：http://www.52xcode.cn/Article/details/gt2gjuepoiw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dcxxxphr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2sqcsudpq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ddsgmcmv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dnsemiwp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2nlrobjze.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2krzcrgrd.html

);
来源：http://www.52xcode.cn/Article/details/gt2imflgfcc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zzoerlur.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ltxevxju.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jfueqpan.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tedmnuxu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vtxcmmwn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ebjdqfxg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2idzcvwjv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2tljyhrzm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wqlqmlfv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qdgavazl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vpwvtshr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vpilgobh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ahmwtula.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rlfrejhq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2matjahwk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jnszyopk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2mjyrjbcu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ukcjuvwp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hxbrcysy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hoolwpfq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2djtzqxic.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bgurvzmf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lwobwlgt.html


<!-- 参考信息 -->