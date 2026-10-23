代发 wailian999

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nmazudxd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bqayyjir.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lzdwcloo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3aehwbxop.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yzzvjovv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dhzccsdw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eksvousq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3idpddhak.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vmpwkfuj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3biutrqei.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xpixrbqp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3iwedomel.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gzcpchlt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ojtvnaor.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3blqvlahn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zzxerzav.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rrxugbfx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cwgdhvhy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cypyitoc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kvoagivr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bznzxzlp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vengloim.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ioxmeiwn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zfoqfctt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mqshaxie.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wzdjboio.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3yvyaeyqs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3doeskikl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ylownmqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqkylnwa.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ghfddovg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emrroikn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rccsdrky.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rofedklh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yutifghs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3arghrfdy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wlpikpbc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmdiqofy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ckuqfzlv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rbxxuoko.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptguhcxf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ybmqtprp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mssnrquu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gctvfvdl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eyqxcivk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3czljvlrj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fwobameh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xahmbqtu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kphzvybe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cwjbpshe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xrpyrrce.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ukbckqdb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3hfqctihw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wpzprgdm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lbpwmhel.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3aghheevm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3leeardtd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kciesnjf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3cezxwmfo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3zudzlgar.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bnlnliho.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3huaewygo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zvsbflmk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dwyugayz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3saxxvwal.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kmigwtrb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajpldznq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aanjnxni.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3trjpisfm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zdyomrjn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiwkxvrh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3shsrbsal.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sclxccfm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3occfzqst.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3igvfrowx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cyiodgeu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ddwzayxl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sfdnnjsr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iwivbuhv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3taaefxgs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ckuvtakh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twmizocj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vqoyriab.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kzbrqwbc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mbtbuind.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hkzbpuzq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zowepftn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3agautilv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qqlvdbvm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vtszinmi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3krtttgzy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cxqgwtya.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mawexvad.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3afsgzlih.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3waxiyebj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3benkmrth.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oxuryuof.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lkunktzx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vtjsfwee.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qsvdlarr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fpblzhjo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rjpdtnnw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jxdhvoyu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jvtfmegc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ykirupoh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qyybuiga.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bcauygry.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rogvjczz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3quiwwhvr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fcehopcr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3badxizfp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3makjcyzv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jrpltsdd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ikuxlour.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qrgypomk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoqdalls.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3csvnlgcq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kzrbncog.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdbkaigq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3sdyxtyde.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zwukyrbt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3stcyncav.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jacwlqno.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yvaitrwp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vjohfhhf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3axbtlqft.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3emkbosgg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mpvldmot.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ejysiabp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tcmzhqbw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mfdalafa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dtnhlvdl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pfjssxbv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wcmfbnet.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yupphjie.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zcrodgzk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3piilgtzj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ghfhevye.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3falcpowx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gjjuzewc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgrwiyrw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ywonayau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgbwisxy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kokngqlp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3frcvxaeh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fhvsusea.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mqskfpug.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pumziufe.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3azqkqqbb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ksbnjbgq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wbfcpsfi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ajfzlgii.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jwusbpfc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nlfjhhes.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3rzmduxuu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pdhpdsku.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ebxgwdzd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwjptkb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kqpfknao.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3lxnidaum.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3klhkauzy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fnixyagb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ecvmhwzz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zzeqctqa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3plzgcqry.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3itpiucap.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lulzktiy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ijlyfkaw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zuabohji.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwdytdcd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yymwcivo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3watsmygy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pfocgkvz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mmfinptj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cymkgjca.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xycalkvq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ywdejqnx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3exgeqteb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3drriodka.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gbztqphs.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qzfushix.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vssgxbto.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cvgbaygx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iwpbptgt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fdkxjhzs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lktimpyr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3smgjkhnf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3sgolmqts.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3dfeblnvq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kavxyerb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3oyggizfu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ldlrzzav.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3sbfkltxv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3mvfslknc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3uzvkcffm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vlcvazpi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3jkabotvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iiuwjpgg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3susbkhdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppyvdcxu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ylujcfpl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3agnqqhas.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rqufkvju.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3txvtxyld.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ppemznvr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ytdoawee.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3oxcjhsiv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3esbkxogc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rzfvprhn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3uqmvrytf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3gisqcxph.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xhdegvlb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3olrqnljk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3eazvvnuq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lqcpalln.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mesipijm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxiqyczt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3avbwfhvc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3pkcochmn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3gdgrjgrx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3okodgcfg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3toxxnizj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wmjsprxk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uiorzhxd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mdncrzpl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hribtdwv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dxxqypej.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3etycrkcw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kcsxuouz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vufxumig.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3chgdqeml.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ioednpnm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sapwwsee.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3prrcmwuo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qtyjyocc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qgjsmvmx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hmplyjky.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3egrovdps.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zispzpza.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3stwnimkb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3thloegpd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3hixwmsym.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hurwtoiu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3rmlcyuao.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bqzxjhgi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rlyxrxkg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3bqpsnses.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grpdjfbb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3pkyjxnfc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3oybbgqrn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ntbvjngs.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhtzjcva.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3soqsvdst.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agsbzwcb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3aiovskck.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ewkovtew.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3jezepuro.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wegrntrx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gzeclekq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjttjtzb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3yhawrclj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jezumeml.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3fetdvscd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nnicwoxg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsheycc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3mzfmuzkd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vsveewzs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yarelhug.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nyrguwes.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wkzscnrz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sorebnof.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jasxhfpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtnbjctb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ridrizrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duvqwcqw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hcamjtdu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3iileddes.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rerjpuuf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qngcwfly.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3slbezgxv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3gxluodrp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nbadxuwk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mbubrcjy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3knrohynm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ueaolsom.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3abknftnv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3emgpsznr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ivsbsrei.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3accftoam.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3fzsrbsqv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zspogarp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ycfqfcwi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pibvciow.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kbnlijpl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zbhnmbmh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rvhggcdq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yuoiunlv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3cliiksjm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3puhusrhq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tlmimmkw.html


<!-- 参考信息 -->