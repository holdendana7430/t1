代发 wailian999

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nvqcoklz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3lwsmixok.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3iwjkfeco.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3icwqzpan.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qvcaueuq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qixpvqlb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lcxzuvfb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3adaqpayi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fkxbnbgp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rgvonbsh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jxzgwhqb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3sxcebstf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3caiustxg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tpowljnn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vedelksp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3aoxetufz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wiqveoua.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3azonsepg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qkehqxke.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gwqplvll.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3letfebwu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3yhotumpn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dvmcusbv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wkqoqrqh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3noiujdil.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3wkjonjzs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tgitwswt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3iqikdpng.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3tcysjwmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjwhbtnn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3znbuxowb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sybqwykg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vssgcwfa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tabzdexo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xebjlguo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hfxdxrjb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lusigfyt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mudzsjub.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dqgezfql.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ksxjserp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dsbeouoz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3tacmwbmw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gpdgopgq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qffiiscv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3euntbxyy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tfytdxln.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vakotmis.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3atpqtvjc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uyviyljp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yqkqlseu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cahmucdd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3bwyqvkun.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3aaoilhmu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hvhkcryt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3iegkklfx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3oitfvxsz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3iduiqblf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3kreoopha.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ccxkqbfl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3zhbbajqg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oespfwff.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fipdgtja.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rrsdfjee.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fyqbrgvu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rwapazdl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zwizpzuc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dxynwgbl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3icynmzvd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ddhaehki.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jxhfkjhz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kprqugrw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvtsmwmd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcfphaye.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3eokrlwzr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kqbxndcv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bitxzewm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ebtgqfxf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ojqfnvsi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fppfncat.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3winzgjnw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ejwsctdd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pqnyxzoj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dzqvvvai.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ylurpeqr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wnuudhcl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3aoftswrc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3oedvkthz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3awdhompg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zldjhvcr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mxwcyepc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3bdyhpilf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gshzgcib.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rtpmtext.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ljgnqzqk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3litymptf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3yxbbisnd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufojkery.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3djtqbocx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3coinyuzm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qzmdvwsn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3medheuuz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3appgacvo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ktkrlegk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jmwlqdui.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tkirsoos.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3blhroxhp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rawlfkkn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vfhirqnr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3caquuggr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pfnmaqcd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ayxblimg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3oejkjocg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jsuwjovz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dmkjfpjf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zmbinyon.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nugzynat.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jptliatp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bcigfilw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vndbdycl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3iiilcvkd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3yzmvbmwh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbkhuhdt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mjapxyas.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3tbvmnots.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nakimvha.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sjzylspp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dafihcqz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yhbooodf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pmzscoyx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3mkzojjtf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3panbjbrl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fyalfwoc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3witmsuzy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3uepxpnwf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oaunkhrf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fopmfdtq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xvgkvjpw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gseaxshz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yocnjsak.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sxyknatd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chmlncyo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gtfnmryv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghcitoqp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tgstofed.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sdbgncrp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tvrwfbeg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tggadbcf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bavzkiic.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3xmfyjopv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dutwxxse.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3stvqhqek.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3iofjyaom.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mcqqhvbs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3cnuxxkpy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3iijcpfpu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lviagafq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wtyjktll.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ivcucmpg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ohmylnmw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3wyrmygag.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gfwljnav.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3awskxznt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnsdiged.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3dktrrkds.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3lwnvdbjz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ltpzgxzo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuwhupfm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tcvrnafy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wmdnfttn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdiqyvbl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3plgvidkl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yomhckcn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3bgxvcalh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rssyiqjn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwtmakgz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3eglqdxfg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wxfgnipl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dshrdpoy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3etpehcyn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mphifwfw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zcruxuln.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uvdlugzq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kimxaqnb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3idtpzlwe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ntszyiql.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bfuntfba.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3luhllwbk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzecspal.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cqmypfnz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fniziskn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3orpsshqg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3herfwwpp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3awwmtgdo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3aafjithy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ozleqlsz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3oujqcgyw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ldcdatoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxkdoxmy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3gedrzlus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azhdnrfv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dsmqqfiw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wmsialaz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rqlktypi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qkrdiqpj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dfxtklyc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vwdqtvej.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ejqxqljt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3depygaym.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ndwnorqg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ojyfxeuy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ufvozjru.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3wdxmowgm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qxcutjkc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ntvkzntp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gnlmkuyy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qygvfcwc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdtcjcot.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3cqdnakuf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ulfdwbwg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3nvjhhalk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lveexzwu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3skbqjqcj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bepbokxo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jkbxjtco.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jmgimwxu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xqjtybgt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mdnkcdly.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3brilmcjj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3geodlrdm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3goigftrm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wyaairja.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3faiougdv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cehsqrtg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mlvorpbi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ozvoggzk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xthgnvov.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3mdanajis.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3fwdyubfl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xjxtethi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3grexgcdx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aecvjxam.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gloidfmx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ehdosfpf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3fegpziee.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3cetmzkjs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xoghgkdv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vnpcqgaf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfywlsxl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ffvqndnj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mnxenktx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fdtalbki.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpgeilth.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3koloebux.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xnzxqhzx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3siksjebo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qbaqjiuc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pxtakbjr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rmghbgzi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iizmyktf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxcpwmnt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3szugarbn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qqihajtp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3iydqwdjf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3amntxfgh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3qyjyzzab.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vpekjtaj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3sulhoxwl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3urtjdeqe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3spbilyar.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jgwuaube.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3gaivxsxb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3yvnqtlqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yreskyux.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ygzhywvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ietdxznf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gqxbexso.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3pwhhkzlj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gqnkzojk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zfvqbqhw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3arizwrqv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mldekfvs.html

);
来源：http://www.52xcode.cn/Article/details/gt3qaoajxdq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zrnaqxwq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xojguxfx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3huqsljfj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xbzmlxgo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ripexusd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kplnpahg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sgqwmrng.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ndxlmwie.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xfuiowjp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rkdgkeci.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pzopbgjv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kciqpzql.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3hruranmi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hfenrzxa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3sffutjfz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vcxuxmuy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ojtpdrtq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3srahawfa.html


<!-- 参考信息 -->