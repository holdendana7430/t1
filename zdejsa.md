代发 wailian999

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhcfmpjf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmbrozg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3varxwlyf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gonrduxs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3mavemimp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ksythncj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3luswlvgo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cianflih.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ucbuzuhf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mvurswvr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zrwbrtav.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mutlnafi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3alojhveg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3chycbbtp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dukncwsh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zkbktgnu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mlpdqubw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qxruiztg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pyjctazq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gluzpenk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3threiynv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wmxygnaz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lnkwbknr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hqswwjja.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3arygtbco.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3djcmoybw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wjtnpyqs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oadqjhfy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kfvlebfl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3sadvlkfn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ozkptbxl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3nwotcisr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jmnhhkxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbkwavce.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rducusif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3daybrfic.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xqdhwkra.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ogabmrao.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jbeixphn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qoxeexrr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3osdjtrkw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbloegwe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wetvmtwc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qnenacgy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3raqjcigx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3umogkvgt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3horqqhop.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3seewkibt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jyptdspd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fxfuabrg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3fwzedajq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqfmstrz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3soltsoje.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3thzskwhm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3adgmfsnd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zufvxzzc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gbfkvgzp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vxrrdqlb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bvkpncbx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cbxpggug.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3knlwyaxz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wwecxufu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lwchvvsa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ympwshyn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3frbtrpdz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqovfpbu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3siudnwzf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eyhwxcyi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zygebkhz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lobcaboi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bafuhxbc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3weadxkls.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3cpxjnnqv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nbsyqeue.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vzggerzq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qmjstnti.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlkjemjq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ptfjyzzd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hlcoqwhr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xnnffshu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtjgffsg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3evjsybsc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3diocfkdd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3anuobsgt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rcwpvgpm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ibvujwzd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ctbrjuls.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3eozumjjb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ezgogios.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nutljsmp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gylrjyax.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3gytzluuj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ucgdyyko.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3khdsuciz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tyszaywu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ruasurrk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fddmespl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ebsnnnku.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3pvggrmir.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3khjnherw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ttroxzpb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3fupuuiiw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uzgtpcki.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3efuydfzj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kcblgkzl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ckvxaxma.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qlxnxudn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wkzpbbkz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bbgeaqqg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tplmskmm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ytirhfyk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ecnlxvqp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3oanxrqlb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3clcklkmm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dpjysghc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dslrkgqc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3noohsnlg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fdnqlpkw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xgsrtgmv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaxityzn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wvimefgo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dztmcmcj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3suqyxwkc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zlgjdhni.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgaqfyr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3leluuyqk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3meltysfi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mkgvrvyw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rmmjieia.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tjxigjct.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3akrhcafh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3djavklik.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mjbjksif.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3wpwijpol.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yjthvqgz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3aiamngvt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3oipeanjc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vhdkwzlv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sstutlte.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3olgvibwh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sovnxwum.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zdnrkxds.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ntwweinc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3anpfhknz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhadrucz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ejdqvaml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swxwkzyl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3buibssyk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vfwusowg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jbzqyrhm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ptbrtfbv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fyylnbmp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ndsiwfjw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3tcwklhjt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ilwzibfr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kfwbvcgx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wiunezun.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fiudkebj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3aeiquufb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3itennfip.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tsqcwolj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lqmehodq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vircnjzj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3drxfwnyv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3eabhiias.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3vdbuuspp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ktsbuvok.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wtloybtq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3tahajews.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3juedjdkk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zrvbuswy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qhilhqcb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3exnskill.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iexqrikb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3luvyjnpe.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ybjehsmg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fcrgwwil.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wfrjdpln.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qchfoffv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3duajjkrf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3huzokwur.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3calwbzzw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqluxaez.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3iiwpbanw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qpbffyxq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3nyuevkha.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3suukaxga.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bhleeekg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ngklamut.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3sqevycgf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mtcwzbxt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3oaprxbwz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3enzibzfl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rmqhvdvj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bxgbbdci.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3radhhsid.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jjaojorz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3njmkdgji.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3scfzweqb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3psxvwhjh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3kvqluuva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkfjuamc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3abfqdlyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shtblved.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fbjffkvn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cnqsfady.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kzatvxfu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cniafwjc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xgbbgbhf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nlsdqrik.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zysytzcf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rtdswkpk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fpvvloyq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yqpqrecc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3lzedtbta.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3naqyavyc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wjumpnhb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3wyvprpbz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mcjscsbo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rrygjgjc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3thckfanl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qldvgiub.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ewqylmmk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3bmpdruor.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3jbkhyvny.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vezphjzr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kftkyjdt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dytokzbt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3newvggxv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gqaqsdha.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xxpuoqna.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rtvlkyfi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3yvkxklhq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cykonxjm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vcftrmzk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qlsyfrew.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tvizkzgf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qyqaizrn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3eklmbfws.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aqczwaaw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3liabixta.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3bicqqphx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3crnwnusn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3podkxrel.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xknuliyu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lyyuidsx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lqlyjljg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kqszrcvv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zadlzmsy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tjczeypw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3osykwufg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajeaepmc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3oocnhjbz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jtduklwu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ltvumnjw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3boiplrhq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ngnylasc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3umkpztsl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3gxduohyg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nbewymxh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3gmkdsgtf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mfvhclsd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ojgpqcif.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdbmpyev.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vlxdvigf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3evlokyhg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ftxotyvs.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3lcrnvrwf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wxulsglk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ambjkvyl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vpybdkik.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qilfzfea.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3taykcjrh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3aduocrbb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3riipzkxl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3uftpdqnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbwvlrzx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3cnydgteg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wryqxhdh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3celkznho.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ondqizni.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3smrflovw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dwijjvgu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3dowdbygm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xhrjrmai.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3edmnyheo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3dvhqhogx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bqgnngvi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qdaptizy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3khqmclqc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ozmwucvi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ogwglvuj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yflptmek.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3vvlmvegb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pzlkkkju.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ufhgnwed.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sgwdezkd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3shhnctjd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xdwadwae.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fgogcxbj.html


<!-- 参考信息 -->