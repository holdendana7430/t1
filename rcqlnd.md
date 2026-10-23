代发 wailian999

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yjabolov.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3fdtmsbtv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zjkusvhu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mppxwkle.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jkxilccl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zimfiikv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dfmrmbht.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mjpdkkzo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3lgztrujl.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ebawvfrw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nvkpcthk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hjrainix.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vfyvvvqv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ilgpuirl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dpimfgcq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xtvxhdpv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tozjbahw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3khkffevi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lkahhnrf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ocvwgbvj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jvurivnh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3muxhzhij.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3oclzhpra.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cfyvnjni.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ocixrxfg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mxrqjngq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qwtmqyrp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3orapdwtk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3uruwlujr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpyxbeah.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3iuookjjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgvhdnbg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ktpugwcr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwzcrpt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3erkfywji.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dyshmyvh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fhclsyvk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkfdxzuc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlhlgfae.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tjsoqasq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uvbhlrfy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hwrkuvpu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dcqnbzey.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rvcpgnir.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hcucalqm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zeskqpvq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3utjxrxhk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gnyapmlr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fzrfkdcb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jealvigx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ejnaiqfy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3opsbwsna.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dnghbubk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3unltgqtw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bpeuymos.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jscydtzr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3enszyjms.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wufsnhsy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3whnlskhw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mhucigjv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dalimvge.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bshktwmw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nrfxkuzy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pbeiyicp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bbanfspl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dqckpsyf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ywakmsyr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aegkwhdd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ubejrmwk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zodwlxnl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hqoiillu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hjzbdigo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fakkuflc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3dyxwoytr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3abgzgkju.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uqbwmubg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rjdbxkyo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vllkjmdo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mcqcygvc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3inolrhng.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3psoyghfb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bqwodkmf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3evbxltit.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3znjwwyxq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qaneqlcm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wngduowl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3nrtxvmrw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3brzsgkdp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3bcpsdgzk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3tejdwikq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rsajypwk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3skrfcytl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mkduoehp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kbymubrs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3bpdrtcbd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kxrwpmrx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxwocrxe.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3czrmqnzz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lfjjsuvq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3adrktvho.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tjqohfgn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hfuexprh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pivgoxof.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3psbdunin.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3svkzuiyl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3riunfffr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wurbcwzc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rfmgfkuz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3argvkini.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cadqjenl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dmywnojf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bawuppie.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ncdzxgth.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fnughftd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3dmciacqt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcocemon.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jitbhnhr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bnffeudx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3cvmblhqg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3domzgvhr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3yigxqbqf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3retmkhcx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3efgieged.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zrplqgou.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ndlsiisg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kryzxcxh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wkixwbjf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gfzfdqta.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dnlgfzzj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dnmvwrdz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cguiirxr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rmlixllz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3fcfaicct.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zwfdozok.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rlihhkiw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fxiwlbon.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iaocfsxk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qodzhfof.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3pyzgdxsv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3valrogzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvzhtoqf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xpvmmzys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huawmbtf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vrvtnicg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hceynlvs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cqejeaqq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pacuifux.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vcxkaiwb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cofysasv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vmdoanon.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lcxtikui.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nhqrrvhz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3lmyhshqm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jwcwljxs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3huxmyvci.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oxekxdlf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3iyzmjcxs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ppnizbgg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ugdncmyc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vngwkmsv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3agmguwgg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3eycgizgz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dsqdavqw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zdxwemoo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nskwkywb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qzrtnqcv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxtygsvs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3insdhzgl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ktcxrbvr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3elublrna.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3lsjcgotf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rtuesagl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nitpfufw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycjsplkb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oijcblcl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3zuvesreb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xtjufzrj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jnzdkkiy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lrqyocpt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3gaiibcqq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3eslihonu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3qkvfkbfc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jbsfasdi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lodeqfmx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3erwmjcgy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xszwitgu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dncykiyc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jeytwjyr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qhhtlfbc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ujhpnlhh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qxxefykx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uhuktvpb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rbxtqfbk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vteyikmf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ikpdlhza.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hjxfwpvd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qghrwxdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udfqygra.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rshqnqyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czwewptl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jvieolfc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qhakpypx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vegitljn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xqolzcxm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gwlmxump.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3brrogggk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ndjsewzl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vnkgesqk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3enttizmb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nfprsepu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3gfjumskb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wvowlyfu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rejmvtxg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tasxwkfp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dmlzkyzu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xhoktksa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3squxaqbj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3cdvlogan.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3acoqjdev.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3rhjywugb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pxvrkrhy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nzftrtdf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iqpzmtgf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3epmzfxln.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xhbuckds.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yefncvcr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mfqyfbfi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ukkerzjc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3lghoyhvy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gtkkbpbl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nnchuacy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jikpihzc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lefldwky.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3glzahdeh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3cipujznq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jthgxmul.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3euvmsgii.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3bykhacwi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mhszkzxj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3eobbucuc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3csdiexeo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3odkhotto.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tvenzjvo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3klpsgupv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vroqvmcq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ozukfcik.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3cztftghf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hldqzzvk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3kbjfqvej.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkwwfvfx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxbgitct.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ndcbcoxt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xnvqepzn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tuigubvs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hrmzzbjw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3aotkplni.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pckrycjz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hrruyifn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jidnuvbs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3sftlebiv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kehcqvim.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fijfdoay.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3uislnofx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3puigrdxk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3zitovzzy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hotusequ.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3kunjtbel.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnpzpkbi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kmvwzgxw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3abbxplft.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3djrecfcz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gjrkijne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbshbqcr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3njlwphiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvrbfrfg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cmxifdwn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tsvvensf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qugoxdfr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yytzxkee.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wkkuishe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3sxacjdoh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wixeodyd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3frwulktx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zafztvja.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xunjssbw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hfazwhdz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3naxbsakg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3idcojtqa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mxcbuels.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3hxdwptwp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kfejtknb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mxzdezzr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3aogzwxvt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lupeapmm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3emqcbqlu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qcatfixs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cgdxghyj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jvfsdmkd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ggdaeprf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wrivphqn.html


<!-- 参考信息 -->