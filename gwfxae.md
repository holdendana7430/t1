代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dknjhyfx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ozmqxais.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hrsqnsyz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3blvtsltq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqrgmtwz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qfgbobxk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3buogdgde.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvfadstm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3eyketwkg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ympnewck.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3oecvevdn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cyuvqitl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3zuuazgqt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3htaaibtb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fvqzbtkc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xstqsemz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gwitvqiy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vsezjrnr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3htxkpaew.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hvmvyosh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nbamkdpz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3engkxhyw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gxhofcky.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wjdzkhhu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3twtomraz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ozlflhjm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gnyrhfqd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bsnquppz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3yzuvezqw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lthbyycl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3xhknshnd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ihhinnuz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bwpwyakd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fcyocixa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3eobtvqpj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3lmvpohpl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mqkopzmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3doyuhupv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cbofxcnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3budzjlch.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3uzznnaic.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vhbshhmb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3daehvjiq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nkfuamfb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jqopglpc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrlaogb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xacnxgbv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vhrwrdxz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dezyelkt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jqoawsgs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jgsjooyq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mguuvkyh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mjylwupu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3iuaxiesj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dimwvjhg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jgghflkt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dvexihsg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xbmtwcsq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jysvmyhj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3giraafrg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ewmmvxuh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bbxcwoxq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vbzaqehn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ezuemhmd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3imgbrtza.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ezxfrgpo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yhnljpux.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mfqrbdos.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvncilre.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3flrwgxxz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vtqojlaj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tjcrsohj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mcvprieb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ynrbnbhd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3usvcoxjz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3udbhsgfu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lfdstdna.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ewqygluz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3skwpztax.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3itknugbw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tadegzhh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3leiyctbf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qgocvwvc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lfqlntfo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymqfqbdq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bsxdokbr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wukgxqni.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3avnscynz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kfcoiizp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mtdoavwr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tbtqiyht.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xwhpntix.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vaksjjbi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gdjihlkz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qraxhkwt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vrmfsbqa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3rokgwhar.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3plfdiawr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vxzqtint.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rfxtzlkv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jqqciydt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3emksveeq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3sixizgpm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ixufmops.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mmqnxycv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wbuzkcoi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dvdotpyj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qyzjacrm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3abrdbbqz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lmzohpwi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mczzdijo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gtsdjzul.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3muarvcyp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iqbrybxm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fpktnfic.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kewaryxm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bwikpcqy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lvcksjgn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mjnczcip.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3msaodwyx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3heknppcu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3mhosvbnd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3iatcgrxo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzitgaey.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gtzuunzf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pgtqnwrm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkvfpsmf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3okxxlqrg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ltodunmz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdurmnot.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vbpqxzoh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ufeygeoo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ouxbrwmb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zrqlziuh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3aqiikgju.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3opwmryuk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ejpuwsdv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lcgcwivb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lkakjldk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ewvorjjv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3dmgbemej.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ttncwelu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ddvtyhew.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rrtbigqg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ntkvuexw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nryjneqv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3anrqnzpz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3undmevva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjlondqj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vfepwmfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfeknrdu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3verjlykx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lplqkimt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ipvhjaic.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mkrokwwe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cstgjtcg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fqqsugsb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fvpouekq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ueybuhvw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ybyhkmsy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3slxgvjsh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3rtrdlvex.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wyntwrud.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3seufwadh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3onzwoboh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uzeutvpy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3pnzmobau.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3yzrwoouc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3nofiifya.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3whjsbluv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oprkkedx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qoewilxc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3dyjflrrb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3okworgfp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nbyllesi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3elahupcd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dkvxrnam.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcgadlul.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bmtmhyke.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xmhelgkn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qklzbqam.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tkdbzadv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzhrjnfd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rgahyutq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ttovxlps.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tdbiefqv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ihiixevp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3yoexuasx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zkvwtrem.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3aleprnhr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jinngzcf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fakelrda.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3dmlinkst.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xuxuqhrn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lzldryoh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukhpyaic.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dnrnxhkd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ggeljudr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kujrwbgk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gnhykiah.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wyehgdvy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fghaccuc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zzecxolu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3bwdwgqfz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3oignarnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qghlqytk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lpivzems.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbelrtma.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3waeugwmx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3spkkwxyo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fbonrfps.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aerizspt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nheovgvs.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3odewpjbi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hdqadjmb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3yfxavlao.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vkwkujvr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qdcnnist.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3yqznnznq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cczmszek.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3txgcsntk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3kobeqmgr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qeutfymq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3cngxjart.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvamilfd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fcgvmmrh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrcycukt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fdgnbvjr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3usfiwidy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tfyhdulp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nkeuheen.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gydwjmbj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jnspsryo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nyihwmkb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ebqkpflz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3scewbnwi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3mqghkgmc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lzntzmip.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3snjoyeim.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jtdgdabu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3usxkwiur.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3pmgeqrjh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jrlkftgp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3szvxtmsv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3stjunyxz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3fkrgpfib.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3imgqnpdo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3houwcbbn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ufvuhdee.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lhjrwkgk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqmighm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3fvrawsgg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3yuzjqmpd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gjxawerq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3amgtibvl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3miixopar.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tjtcmnnz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxivlrab.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpnieyxs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3tuqjoqzg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qunxmrfb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvensxgw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zacnsqqt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3floqqygj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qsviojfc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wkbgitps.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ffsscbcq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3uudapeql.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pamtxeuu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3enbtqdpi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rofnvlnl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ledrystn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dxajmgrl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hahunucw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3rgeneliv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vcocibma.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jofmbqfz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3teqrusee.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3lmuofpui.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zvmdxnxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yropwocc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ugjbsqbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulsxlora.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vaecswml.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3sifzoiip.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bqdeoxit.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ulpaadzg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xavlnhtb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ikegxjia.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rumtuskj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qyraigel.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3tgxpzvks.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rqdkljwb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3slkpfjvu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3aigmrffb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3tvxeokwd.html

);
来源：http://www.52xcode.cn/Article/details/gt3hrmmusju.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3jucvtrsi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qjcvugsr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tkosccub.html


<!-- 参考信息 -->