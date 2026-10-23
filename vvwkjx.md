代发 wailian999

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rqnkahog.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hcydhkuf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wggclgrd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3irdydbdl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3omrwnifj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3oovvnwzo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ehgwbncm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zuchdpku.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gkzvghsf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkcyvsiy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuulqmbg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lxvoeiuv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3iaggunuh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3rccymgqv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3klozstul.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vyrlxfcn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3olsgzwpb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lsoqtxiy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xxpfitsr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gycmrbqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ubunyxbg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3fpgjrvsf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hjfsfypa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3axfydfqh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3krrwdidf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dsjgnndo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kuwzpxtq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3czbaszpt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3iwphykae.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3icmscqth.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lgffvjgc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kemeligy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3pbrqzryp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qkzaojum.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3izkarjeq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gddmeljk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3aibqjqxy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gpdccqgm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wdzhobsm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zhtexozz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vmaqksmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmsjgjzj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3htrjamzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urjogbsx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3xxurijdb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kqggmkxt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uruxecmo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zrtnmgsc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eadjgtbu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkytbxvg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkcufcnb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3fhdgmeei.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rqqgicww.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3pjdfgvdf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gbggavxl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aizzyokb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hycyekfw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pdoxgafr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ppgpwpsp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jaxvzmcg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ybyadekf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xvpjsiav.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qpgbukzy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3bohblqgk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3orxotkfk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3drpeumpm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sxeckwga.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jwyuvjvj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3eyxgxxej.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pnrslbxy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3uvzhiiuz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3csmfbrru.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kblogxfn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3laubxngq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dndzezoo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rdcoflti.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlsyngnc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ixydkcqu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sbsljqkp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dufakiec.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ovhamnpd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kzmviuts.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdohtscs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gqjppkry.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zszppqit.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vphllqzq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hihtgtjr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3celmcpge.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3pofycgem.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3alpzektj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kbjqwfly.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jedwukxa.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3insfkkes.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zyuocypj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vdwrfcdm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wffsfjla.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3beqrhjwj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dnkeiqpy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ltzacjuj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jjuuafhz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kwgelufx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3axnkkvvd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zpvojhxx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ixquriqi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dhmihqfd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3stjskisa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jdarmgno.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mofhnznd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hpgenlbe.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3avbsysdp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3euzcwvfl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sdbxbdwn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3adzoleds.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3chbnmbvp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gezbjpsd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ockixeuc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yepmuhkp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3opyyrtpk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3soygzzwm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xiwuvrxw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3vxyciikk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3obbvecri.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tcutunrj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rtmaglyn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3tivvjjrt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wwkrpois.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3xduuvytu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3khxfjdal.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3letrrysb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ucflrqmq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqfitsfo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lxlnaxjx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ybctxclg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wmtjanfm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zjkmqfiy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ypixfrit.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejcjrsov.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lmrifbzm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3utvtuhkn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mzrwrnjf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fjbdoxjy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gkjgzvjb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jtjcnzlq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3iwhwsmxo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hxuzchpj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pbauwmdd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fitjzqqx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jxvefico.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gsdifggp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yslwzbyi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3osddgxcn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fdkjjuci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydpnccvp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kymeuuxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekinsphw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rjsyclwc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3zmjcblpc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3esktinsg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bkysouuj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jzqpcbtw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mgfxckkb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ytegttib.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3vajhxalm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ykqfyrkq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3itgiwzke.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3conlkldq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zeyygxqi.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qmyiiexl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zusbbhzu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtmlpcw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3altibiys.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3llkaabyf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mtchmjym.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3lsjwdwbj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bngciznw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gdjczfyn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ubnvniwm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wtnrvxfb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekpekesl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3fhyobpth.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fghrlqch.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3csqtlktv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tdruxgng.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kdonuyli.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fbbzrhtx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fjhxdkzw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qdyebbul.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gzydanuo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ojpzexfd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3lczhnevj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jcsjuuut.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jnjanhba.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xezfivku.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uystqegi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pbjzjmhm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lcoollnp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qhyowwkf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cqcfcqmi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3njuzlozz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3aytqzksl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yztjtwti.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bxzxxwsc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3shorbjkw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xnfbyrjw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3onjusvwf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3hhaljpbo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ttybigmn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3kxefmypf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3eqbjvszx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjviildw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3tivlcvhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nduetwad.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3itjlnevb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3shasokox.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sxpcxuqy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xkislmld.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wzgiayrk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3qkpnjsqi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ckkgtyjd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pmhhlqlq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hovcrvwl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3zhlfhpty.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3onsjvqsb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eqgxpsxy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3fbrsaogk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wehjejun.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ubefolya.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mjmfitpq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hguwsksa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lwwpwuql.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hzznbdnv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3alxrvplr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uztkxyqq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qpznsxho.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jthlkxib.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3odveuczd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hadmkjnf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xnjoxkex.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3csruwkmp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3geuojsmn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3oggoozsa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3anlxjqjm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hgyzdyuf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xkfcvbbq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cbbcmtdr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3bibppcpa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3brdgzivw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kxwchnbv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cutpjxwl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cgchdmoi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3noqgxjhl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3bassglje.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cugtlcgb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3eepqznba.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pmbujilv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3igiirmqa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3yvoudcmg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3azqcjmev.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ziuqdbso.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnmnndji.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3wjxptmer.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vaituexe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3diwcunpg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3taxungaz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3wjbypxmp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzfhvrqw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3eceutqmr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3tiwrjmxc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hfxgrwpg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ruhvdjdv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cavjplhp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3sfyitaqf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wbfrffxa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dfgvzvax.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jhggfqhe.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3gdjmzbrv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3guqmunly.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kmzcjyug.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3lzdjkzwz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxcoyvmh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xlzegrxa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rpwwmmbi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xqtlgzvf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kdodefhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucjrnqpn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zhmwcuvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydxwudhs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cwqaqihs.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qgpyjwca.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kfwkuqgn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oesciiqf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3hburmwel.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3vstpbptx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dokddzup.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3sfgacxud.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3dkfqzefl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uvbakuov.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ykgggyzi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3janauyvp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ceciaeag.html


<!-- 参考信息 -->