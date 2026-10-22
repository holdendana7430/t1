代发 wailian999

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mvumsfcb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dzrdrycg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2hvvckfpy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jifbvbxw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xgvfchhy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ismlvgrt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vpbfiwbp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jxtfkmtn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2tboodhdd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ubkmelaz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eszhsmqt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2cinswxaa.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2kaxgahnj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2yxjlzioh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jyfyjtqt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ngecixpl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2arpfvfrz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nybayqgv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2iocmjnmd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dkjypilw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ruhxgdcx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2kzncksdr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tszuecdi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2igzjblzc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dqhlxcvv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kcmicznk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ekbkdthn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mgneyhbq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2trrfgdnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nclljkac.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2yttprvip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aezxxvht.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2oxyvrcog.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xdbrxyhx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xwhilarq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ctrjvudv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fkthftqh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrxstal.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gdhtufas.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2blpexaih.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xcuxoikk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kdgkccvw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tamvfsmb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rkzkspjh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bskfikzq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gsnzjnog.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cuhvmayq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bhfxpagn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dxnehnbx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2kyfbsjcc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cmgiafjr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2afdmqtpp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pboruzrj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xdydmqqn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vhlpgnkd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2oqlwqwiq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qwypjzhs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vkjjhbts.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2eorsmdou.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hnbjtmmp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2innvvpai.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wfkqauiy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ktvimajg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kiirzsvz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsvydiue.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hxidlnio.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppsebxoh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pprbbjbl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2corlrlcj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2iszmeslw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vldzctvf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqrilzbx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpntstjr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bthtrccz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ccmngnzt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2aqjurokd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgvcpuhc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iaelynve.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ndcxbvoi.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vgcorecc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qaadbghz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2idzzwxwd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qpvhichy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gqbbecmf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fmeffqmb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tvixdfbn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2muutfuyk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2sjubcruw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2btruject.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2sxsiqndu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ackwlpfc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bkwuwjzq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fmfbbsmc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lrezegyv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mcbsegrp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2mfssmcgu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wisrpmur.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dyabdcjz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lbpzsngb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hdecapee.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zejtzner.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nicyetof.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kxygrgzl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wilubuoo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hlzvbtcu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2agquagjt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wbqwzowz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hplommwp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ldozmoxy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gcdqiawk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xtuyeava.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zhrjuibz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vhsymgxy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mlywntuj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2stcbkicp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiitaloz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vskqtwjd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mwdfkgtf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlsgiwcs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2liyufwnn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2esvemkmg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzfjdlrg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qbjozfao.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2cilyzxfi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wrornozd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lzlxciyb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pwkjxrwv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mrhmejvg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ckmjawsc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vydrhvon.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gohsbuhk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2vfmprnnf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ualvjiik.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dcqonkgk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ervprnfu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fhljxyxy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kzszizop.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pkmbumcz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2awgixzxz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tsnkafwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klnwgkvu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zdmcjpkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqxqihik.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2srdznevj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2czbmlzvp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dghlssqz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2avxpvkdp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wvnemphx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cffhdbdb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fcewbfdk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pwepxgqc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ehojufko.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ihjdlhuu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wgkmieea.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2byorcidm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ijidwaqr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2usxkycak.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2clzbbnql.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2cdltuvil.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ccwpkact.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2cyzthrtf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2gzyikusm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2deuxusjp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2aazcdecm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2xxzyfsrt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oobxgbtl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tqjoxajc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pewsqkov.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2hhswatja.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfdkoqpr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hlzwmehr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2urtqfait.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2kghvkaor.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dbpdlbir.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fwtzexpm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jjjwggcn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wrklvzwp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2mskkjkvf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqrctqak.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2tvyyaglg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ulljhbhx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2waylkivr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vtogwykp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gurllbpy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2bmjyecxr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xmurpxyv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gtddrwze.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kjupquys.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2mevxzlde.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2kwrmborw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nrfwgwvr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dwvlweoy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jupqhpah.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ythqkvtm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fvpoqsvv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2kvueursm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2moqdhhij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytykwptb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2iqvygaxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjacchkf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mufjsqxo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2narfdezq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hqnbfxbe.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bdxpufyj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vxplknfd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dxreogrd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yfyqzatq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mdvyglgs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2clcemvof.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cgidzsqs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2afczgnme.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fnlnyeac.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2nnufsjss.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2fnceisub.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ntlzofum.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2prcdksoc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqmjfhdg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zflybrah.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2djvfhfzt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xgluotgd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xvylxwzu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rbqlnkqk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dkdjacyd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yvvnggta.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vauulirp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uzdawgck.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qetyoqqe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2owacznww.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2munzebtf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lcwoqbku.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ayyzcwcq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2inekjuip.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ftdvapat.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uxwjrwaw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zyvxohtq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nwhrusht.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qxnwtmei.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mulqvzjy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lgfbdvhg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lcmwoqni.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pgghbgia.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vyqiqnhq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ddiyjglw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jtqxiayf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2oxzmviqb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2afepvobp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2reihhqne.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqfbjucu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ydjwsgti.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2yhfqxkqj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2haggitba.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2drphvytd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wzxtwhmi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyyszndp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2wmgestbb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jwjppdtd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mvuegjnc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pretmqxy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ctqkqywy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksklofuw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2egewfndb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2epbtrxie.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rvbeupqu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2uukckkxd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2aqcicnwj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rrpjubsp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zbvyfoho.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lqkiqdey.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gwxzogoo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wcnccjxf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2uxoyheqc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2gcnlmepv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgrytjgp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tkfwqflr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juwodvpi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vvpqjmib.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2gzzsgvvl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cjmjgfwa.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dihchwgy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2smfazrsz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2oendfzfl.html

);
来源：http://www.52xcode.cn/Article/details/gt2sjkwbrnv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ouyozond.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2iccpnqgq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ryrgcmpf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jttdtuos.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lkupfbng.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wrncolfo.html

);
来源：http://www.52xcode.cn/Article/details/gt2pkldzjcv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2pjmoelin.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jjfmksoz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mgfnqgeq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hwzahwkx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kmfanijm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mwazrmea.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mfdvnssi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2almdvtap.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ylkufhsp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mopbqypd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2obnlydah.html


<!-- 参考信息 -->