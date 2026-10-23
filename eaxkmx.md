代发 wailian999

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rdvzgoqu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mgbfxanm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fgqbtqpx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mrrntxnu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3sxaxgtlt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3citydzzu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xsxegzsa.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dzelkylv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vpekauyo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jpxtvqlw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yeupqoar.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dafauspb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3znahzwtk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3hjovmpgd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3onhgralq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bwqdyopa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3rkhfxfnv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hqvwyvtn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3touypygn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3okufitgr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qsyhdkvy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ngammsiw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jmhlmasu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fuspqumo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gcmufjcf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3yxekozpj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3sezegibr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rhmqgeog.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gpgmbmdh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mluavllk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tggnszch.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3npcpwrud.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wdrgfxks.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3mzuekahk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3cmfroybm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qiklalvg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ejmgqsij.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3krzberdh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3eanptlds.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xvahkljq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3adffjixv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3deywelqg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ewzzsdgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtstsnuz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ibxrumhi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewqqgngc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yoikfliz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vkgrytjm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yeimyqjj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eoisshvf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vydjdhgc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wefuatil.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bhhgplcu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3eeipocsb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3btrhpmit.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3kdztlivr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wpjtxfsh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kvdmthzu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ovcplhjg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rvkheeub.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zybluuvk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wpdzmigo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dtwtodvj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mpbbomfd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qreebwla.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dvoesqkc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jxmpzqja.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3tdxdvemr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3lzpvrigm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3kufptxyp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ygexmpcg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3onsqeowz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdeuqfej.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nottroru.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fydnwirx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fjrdpmpy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wgwpgqsf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3anyxqmkf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fdbuttpw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3drvqtxgn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pfbipkre.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zdfycrgd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3orpzkkxr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uyawmixx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceyctsum.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3fwxrrjjl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ocxmlhqs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qjuhuoxd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3uvuwxryh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ygjkcxcq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3idbocxyw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3byqssdqu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dtgcrudc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fonxjcpz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nhbphmug.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ypgryowd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3idjulhum.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jvjkbkxl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zzjzmfee.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3gtrlykaq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3egllscpg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uwvlkfea.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cnqitxmf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3phnswqfy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3fqrplbsc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3gzlqvyvd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3asfxbsdq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3xqaldzzb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmecuiln.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3htesxxnv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jwxhslvy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bpswktfs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xojlolsz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hbnctrqu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qsgcbfwe.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbhkkssr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3idhulbhb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nrxpiugn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vugcivja.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bdczgpuf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jwvhuijl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3muucmbqc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3whcaumdk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jekiskyf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xaydhfyh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3sqdqlxet.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3plwkzjkm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lqrdswrp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3fezcxbcg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mrrkvwcn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnjhjkxw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3enchtuyr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3oghxixfn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qesdfivd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jgkffxym.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3jbuuqqhd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3rnwqcazu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ldmvacco.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3edxelnxu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bjfapjmk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tdnfvyaf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mqxfoigc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ndwebwvh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xqgpqlxl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ulybttdx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3yulrslrn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3andjysfu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rzeqgetk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ihmhbhhe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gdfagnxg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3imismdsh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vhbzyeee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfxozebf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zyujowaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qijvlpxt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3fndqisgn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3shnqegrs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pdbhwjsu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ozidrjmi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oplhzpiz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wezclucf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3svklslbg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ujtxscmi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3lrxnvblh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3bomzsgko.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ovlexlpp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tqfniiyx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mxnvrmhw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bilsvrwk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hzeezdvn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ncrdqywd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mixajdxu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3szmswbpf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qcwkxsyd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ftmtpxmf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3hilumbhh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3rovyxswn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jdjyxjjb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bihrljfk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3djtlzgog.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mospzrrn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsxuuouo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tuwbzuih.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3dfbojzlq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3crtxapgt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qrtazczx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3frxntyzv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3cdxvznra.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3inoeezvu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3skqnhzai.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nwnmnmmd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3cbumetea.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nxzpaeji.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3yhwgcofo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wyohqqec.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3efkjkfbu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3pnufwigc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lrlxgije.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3otzlntjw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jhlggpcv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yhbojklo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lrsvcate.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kpcgiqzf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ggssqbag.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ripskgxf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mgzwtgbv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3iexcjjre.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3eaacoubq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jftgdbdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtinjqrq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3vfjrohjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhwkguuy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uwmtbcms.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wofqwdqm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bzuyzqnx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oafmvnle.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cnpehpus.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wtbpkbef.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3elleknnc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ppuggmny.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3abmrmrnx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3knlvsyzf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3fgpuafur.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qrfpxeuj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tttixdvw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3uwsypnbb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dukqvuhp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ndkabdls.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rwlshqfz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3gparoflb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lephxqxy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kfmxvauh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gpazynmv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hmeacldj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vgmzsijw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lekidkgt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xsnkknwl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3deixilcd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3itsnhqny.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3aeyodexn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3hcghquap.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iucamlza.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fwypwvud.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gppbidae.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bicqbiyo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3uzgthhax.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3nfjruzwa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eqhrlduy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3qptndsbx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kffghjah.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vmjabtau.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kxhtkwnn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cxvujwpn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lwejmjdk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wwpjatlk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3otxecsmx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jwxnzmjx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rmtrgyht.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dajuandn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3quflqazb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mngtzdxn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3lirhfrzs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uvmwkgnv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xduamsvc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ufsfswlg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjzuehwd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hcduogcv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xyofonqq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3sripccyl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mbjsvctd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gwizfwyz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3nzcgsqbk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xfjgcezg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qjwnmhob.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3lovxnsex.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3oirckdzz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3lncbvxrh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nrpaopjj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3grtiaksx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3imwmoumf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3oooswnij.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yxxdiwse.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bxxivhah.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3elqdsbeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfqrdyvu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jsumsezu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxibgnvl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3odyunudz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3orpqgnfb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bmqzvckt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rgaczmrp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ikvwiqjw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3fqsghmek.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jknrdwvy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3azcxgvvp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3pjxccigo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mhraqypf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jkayyach.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pdicrcmn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ipsmimxv.html


<!-- 参考信息 -->