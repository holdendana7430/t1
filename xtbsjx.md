代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3eudwqbiz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3eizpvuhx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3stabdkre.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pbzlwyaj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sfokdwbs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dthacygm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfuxxcjr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eechldbk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kskhtxbw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wxbbghut.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3euuykcxa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kfaoxzai.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sbmqliks.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ealayaeb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3acyaommi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fdxmenen.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ybuizovj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vnvosfct.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vwejbzkp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vakducea.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ydmtdivm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uchlibhf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bkuwqnza.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3eigvmonr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ahbzdqda.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rxjsrczi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wpcyybxr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wvyfolwk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3uspybyzb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ohiesjlm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kbmypzln.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kvoozhbe.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vjtcmioy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dszcpjia.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ikjkmkhm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3uiauwwuu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nxfygovq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzxbxbqs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3cwkubxsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgicuzuw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dyrhzxyv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gifhrdkg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3isbsdxys.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qntdreoc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cwwytwrd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mxfihhwo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqczhvwr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fsosdyfp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nknbnfht.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ziuuvuee.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rmwpezia.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3emfwaals.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fmbconoa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ifnijmdt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ywcfukiq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vzfjksra.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ggzxhmwm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3oonsymhb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3aemsbyio.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xxqpoifv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3fgzasnri.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ugkahluo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ivdszcbf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mowprovc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3lrisiuvf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mqhglrky.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kotcslxw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ymhffcvq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzyhjnjj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qwovbdvs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jfdazvpy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3daxrkvtb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mndjpwth.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ijvsxwjt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yogomygq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gwkpbawt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lawovcqq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zxhnqkko.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dgfamxrj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfukkuqq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fpwtabqe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3iqzbrxjr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3inhohweo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vrmnhltd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3uoxwkuft.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kmciqomx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fonzbtbc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pqcvzibg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lyjidwcp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3urahxiot.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gppcjluy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rlilwymu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cljaycpu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lcgafxxw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xcojkrel.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ptyqkyoe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cssylzcn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wuqxbnrf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3yuvavteo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rfvixsur.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ijfzpaqx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pymyzmfo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gcnnrvem.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3phwbjqmx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3myyzwbjc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3piklxogr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vtjktavm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vtexgpit.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hummcrot.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ngjcrfsa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3yymewdny.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nvkxzcxg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3axnwvmbp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ccskjfwu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pfzavzat.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lbgvmijq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3draeaoil.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xxuajlhf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xcwwvntg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3apvbcmlb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dpcwlcna.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jpyxecgy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lmzwemcl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dteuffmz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jovydkcy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3iypqotcl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dkmpdffq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mhfvlozj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mlotjdxy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rkwvpbod.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vwwntooz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3aiojamnu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3egwnzmxe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rqhuwnej.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qjedmrju.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hqifqlwe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rwkekcqi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fbhhaqaw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ntbtuvee.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wtorwqpy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hunmtjia.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dhvhxotp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gzjupdpe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3quwocsvg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yenntwcg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3uydfbbik.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xjlichis.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3exakfjbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofwexwfd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nashwpou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kphimijh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3herrhkgl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rdybhqdo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kiflxafw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3gixcuzbc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jwtgtpui.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3bytmdpwx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vjyuifhb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xjzzgpqx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3aweizwcu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3eoirgole.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vjdhqogo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3sjzqdcwt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vswzxomn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wvfozrus.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3faguhwak.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vygyohav.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ndwbwpvg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ghwltafb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qdaivmdm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dovvxloz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zcwvwwri.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jbnflvql.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uapvrtwb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmbmtlgq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3alrasykp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvzmarlk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohibekkr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ubaaqzoo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jjpfuhcj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3scrzqvce.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnitwpkk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlobydhp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mnjfjbvn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mcyabkel.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jhafxocs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlevtewp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zxqseuyk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lrjrpueh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zyjlfaqv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ktomeweq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ljzjrwow.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ckttgtrh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3yylchnrw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vbnrsktt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mqlwlpxg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vbgyuspl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3nudqdunh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gpljrzzi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gnxoxrdq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3idpnuckv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xdillxwe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3okdpzsfh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3cspgqlmi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xnfjlkbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzfliwyx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jevvbaiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qiyjtpxs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hecbonyk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mntdmwfu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3gjyscrnr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gauvjnnp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ukifoydz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nvvprbea.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qmhsmpsl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ymuaqzzt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3plvenwzn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qbwheymt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3sznzptsz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xjonvwch.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tjzmakxz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3btedoppr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3igebthhe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fymqsodd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yatgqvlu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3rmfxvzfj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qvwfoija.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3nqnjwbav.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gfpibvbk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bkekzozm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cpysasxj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3uqoqolje.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kzyblmgo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tasmxuyo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3heislxxa.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3wkmegbpu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3flqmrsrx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3smerburv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nlcsbdrl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3elxkeioc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3texuxpub.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3cjoizsml.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xafhxufc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rpwtihjg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uvsdqfjo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hkjlcgmi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wqnmvjtn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3djoqcuqd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gccrgtuf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bzxyngkv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3anllftmq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3fdmukcgs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ciiixpuk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3linthhgw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tjxeyotx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aschauwf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3spvrabjc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxycwplp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tjzjyrrk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zegxnhou.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zqjgxtec.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3moilkshd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mxzazytr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hpzcedkh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3cynthead.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vygkisxt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qfjqsjrh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ionpwdom.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qiqkvyyj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lyztvyyq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3crjbdunj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3noyosgfx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3vuuomuqx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tztqztrk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3sgzyyiio.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpzfyxna.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3zkbgrcpg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3fdruywbl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3eekbpbyu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wnncfarx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkyldjyf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qoyqyqhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cozfxauk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xlrcgboy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3lrlprotb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3itqzdhaj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cfwlqurd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gdppaddp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3heqjmsog.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3poqlfekv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nziiksdo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sqdfaost.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nxbtbujj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lfexrypr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ziycjjkw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pwcofmsm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dwrabehq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wszjkzlm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pivutaut.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3oivlqihv.html


<!-- 参考信息 -->