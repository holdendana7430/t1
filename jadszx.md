代发 wailian999

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3zwozcwbr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3pmlqbzhf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lncuszjq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mcexwsoz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rsnbyxli.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bbdykrhc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3bjyyyeet.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iayrrsan.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3icvtzyyd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xsddggvk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3uvfybyja.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3pkmqrelv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ucuecqvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oylgikct.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mfgihlri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoqedmup.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yjjbookz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sibliyam.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rfsckywv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3etnmetwa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hzfgjtep.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3teepzvtj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zvxtzvug.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmsgbht.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovvgzoia.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ttgcrfid.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yqehqpxo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sfmmhebl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3quacikac.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hlidesnu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xjhungxw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vrwrpusk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3njgllsrc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3mdeugaqx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fxxdxcos.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cczyoebn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dyezzmhd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jruxadqn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gzmuvrfy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dhcavfhe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jnwzzupu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3auiajpks.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jddoiopz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vkmawphh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hlfdvzyx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qrwwuxak.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bulqujfg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bticniof.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzsbtam.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nstzbzuv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztnhaymp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nkgvoeoh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kdlresid.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3eqnhvuhg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uarjpyvq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycbfqmdp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdgqsguz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bmynbfdh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3cfyhqvmx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fniujyso.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qawqadov.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3outeefng.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ocrhkwne.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hsnpjpjp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3djutgxhk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3khkoiqpz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3fafgkeqb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mwyeypxh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nisooeht.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dbnlghma.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wxaqookc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rcqpwfjb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ucfyhtup.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3itppsikk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ibwqjrid.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3teeourpi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3fssetjfk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zkaxwdhk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3phlgvhqf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3gbawxlue.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rzmesvqu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bcdrtzuh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zmyndakj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wsojzlan.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ioojukvm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dicmnfwr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xfomtltb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3likeqoyr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3obhcujqz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ydkyevjo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fclcxajs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xjrpptog.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3zweyivqo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hwiflbdm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ecxrxuzi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vpsuaxov.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nvfpqiet.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rmedsgrf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3htgyehdt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tuwoiiwd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ayyibaai.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gskkmqzn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kplqctju.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3pgicwgzj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ggrehvju.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3drjaxncx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3rpmhtcfu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3myyqqadz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3uqtmfxho.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yygdkxjb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xamcwnuc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hvhswaca.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ofrnyyuq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3sbdgznis.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zbkmnuls.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3imekyoam.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3quplrsoz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wfroxkqu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cgkzlqak.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3sqqqkfzr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nhvlezeu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tzhcxluj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jmajllsq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bkkevmhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxczcrke.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3chajccvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwosmllp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mtdahcek.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gufqolvx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rcnoibix.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3wbmjstun.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3soiyqail.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kafqfzhk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ezngivqw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bkxxdcrv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3flkdhelm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ujdjnyxc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bzvbiyrd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3nafhgafl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bgyptnks.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3utyfcopw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xnziaweh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zmdkquco.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cqwlocwd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3owmbesdf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fecbfrlq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bnistotj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wnuiccxn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3aefotoxy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ctjddfcr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3umfegdmf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qakuzrti.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wsbyapza.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpoxygxn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3oyiprxfk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3enraurts.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tumqdwou.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3efpubgep.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ralmehxr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pthnxzat.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vwmpfxxj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hkiufaub.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcwoaxex.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gussrlfw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rduxnxdv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3sxkhkibn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3komdoqaw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jskhztoo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lleofhqc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vjwhbbrs.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zbwfipez.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3iapjhyjz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wizbgorw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3tzwibpfn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ykvdbnqb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3onpxliqt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vucfzoce.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3erbikzhq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3eztlvyxl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mqxjlukk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zthtvidq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xajintzy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3isgfqonr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbvjbvoe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jorxnpox.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ioffeaum.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xrxnfmdv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ymyxckoj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wjxkyrft.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qgwngjqb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qkhmrhzh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3eaconkra.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3afqubrnp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xqlhflik.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qwccengz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3epmlhpcl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qkrzdybp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pcrqsmde.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qqoigblm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rghbjaft.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3filbdvjh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wwvvxdgl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ptcjrsme.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3nwrunnsx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3utaajqjp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pzgpcjwd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xbwwqlxe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dybtgckb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tzxamfmm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dvozhyvg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3uhmooxwt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cvmvvyoj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3buztqgyx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3smlylglf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ylokkhmi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xnxdklvz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mfsgopee.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hyubhblk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xaqrlefy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3spycrwea.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3lkpgoadg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dbzsddzk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mriodcpm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3slfmmall.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ggybucmp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jgimldqa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uxwpyzoc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3dpvunopo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rcittown.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wibaltca.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3tvzbphcv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dvcfgldf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fmrtnzfe.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxwcnvqa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytlbrsvg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3oyqqnlng.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3olbbikmv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ccybojve.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jwxzxsju.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3oiwdgusn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3fuqwlbjr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kjgseoab.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bicwyezg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ssjbykvy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hmuejkmi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mcepmdgf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vuxkfpcp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3agiuaaid.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3tpdsqtck.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fuuzfhwk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3tnayptmk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktfucpio.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bqucxzlh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3gbrpqtfr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3aiemxnjs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wxfrrjaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imsadfyc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3rsozfjfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmjwwgrc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fydjbeft.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hxjmkeqy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tfbhuqgz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ouxkywzc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3aiyolwae.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xlgzlgoh.html

);
来源：http://www.52xcode.cn/Article/details/gt3pjvmhmfi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3njmjzloo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ppdcbbkq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jiefuieb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3drtaeitw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3iicrpqkz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ogefkanc.html

);
来源：http://www.52xcode.cn/Article/details/gt3ysviefwh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rhccewat.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ccukkorv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bplqiadw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3udzetbhj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dscriyqv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3gciygwux.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3catdaxyf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ckbwnaxf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hxliwlck.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ebisvysb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3zxcauote.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qgdqzyno.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3qhyxkhuk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3musmcldu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3okazradu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nuawbzzt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3cwpgouei.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vkpzavvd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3rngnrfbr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lsceztdq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mqcigumq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3micfcqyj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pmvbwdgg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jeijsvyo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3pjkgfmlu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ahyabzml.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ymujioup.html


<!-- 参考信息 -->