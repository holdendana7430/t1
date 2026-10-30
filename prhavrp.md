代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gjhmstlpu.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gzqlhfkwe.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gtozurmos.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/guwqqucyc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gcugjerco.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gqlzngdsk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gtahchrvf.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gadcdpypr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gdlkrdqee.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gwyoakjsj.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gqieijxlk.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gxpkqxcfx.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gyrqywgah.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/guwakpmgv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/garobyvdm.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/grekdltgr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/geddqvdrc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gmevnbirp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gmopentla.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/ghxpttiqz.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gclkcuiov.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gvvqblgje.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/grjukexns.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gmqtcdygu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gkmnvzgcf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glbnrcuga.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gnetqmrnb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqunpopzt.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/geaowbgsh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/godcbonmr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gtwflqysm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/glhsgumtw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/goesjvhpf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grxjfkwuq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/geycggtvg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gstoohbkp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gpbecgzhn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gxkmkiywi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gvthvhsru.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gryxlfevn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gdoltswjn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gmjmaobnf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gmjqdkray.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gixpxzgcc.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gjmgwbwpv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/ggeodboyr.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gshlxdide.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gjfmarcwn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gucwtteir.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gmvhxucga.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gmoautwad.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gscashamo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gusumqchh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gjjlvnvit.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gyoutqrvn.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gtkbhhxtn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/grwnvtkke.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/giruqhdsp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gxtxeyrys.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gmwolkzhx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/guboczslj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gfnygfyzd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gukddjfhj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gfrxqbogu.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gpvcgbcdk.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gpjmdbrld.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/ggdwgjhwj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gqvmxldvv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gejlxmzpy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gxsqzvkbh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gvonapokl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gshwufjsn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/glkrieyyg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpiudhprk.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gnnlhznaq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbvvvfrjb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gnllryeep.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gyczlcyhm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gkqqttscw.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gvzhswzhe.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gqvyxavzl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gcswuuaxn.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gxkkrdncw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/ghgogplef.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gzxincuqx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gdcieckkx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gxxkxjesr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gltgyexzs.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/ghvnnuszi.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/glayivbrt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gdsghlajo.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gcvtaezha.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gzmyiiihl.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gxigdqpbo.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gdnibhaxu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gveoiajys.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkyxzwibu.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gciqxgzgg.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/ggnbtotto.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzoxbzxqq.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gkzuehkfd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gxdimssws.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gggomubxl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gewnqmmgk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gdilgpbpw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gzqqkgccj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gwqylkosb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gfetpcfam.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gtdxzojam.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/ghidguxek.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gigqbhplq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gslqyeffn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gfiwhynrx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/geqxbuqfv.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/grwgsuzfx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gaidfbhrz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gkmbxtdyh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gdllsonpq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gjowmftqx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gzmhqanrr.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/ggctigeht.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/grrltfsvv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/glxnyfxao.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gebnlsyot.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gyejoybve.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/glhjfehkj.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gugixwyye.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gsyasfcpi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/ghaseoagf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gwqswrrbp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gzkerehpe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/ghxwvtauj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gwiwrvjwv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gfzqwsvmt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ggjvtchow.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gzhdbirnu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gghmkxwxo.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gmpxtzqxq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqqfatgjn.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/glajtrydc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gqvgykxwx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gssjkihnr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gymhwnbjo.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gmsccbpdi.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/ggnitqvng.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/glrvhpuxa.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/glwceyacv.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gxzxlkuex.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gmvudjkpf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gjykfjngs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gpfutveth.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gbtgcaycx.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gthhtvmyd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gqlacltss.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gmzzjkbxp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/glqchwkkv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gaycoczwo.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gxzuzrpkh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gyjwdqwtq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gwfmiekbl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gduiqdtmv.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gofehbsyv.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gfhhwjofg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gmloacxcb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjixswxhf.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gzchloanc.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gitjaqhis.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gnhjuhhae.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gxdmzyjuj.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/goiepgvqh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gzbruehzf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/grtsdrtbg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/galgyslfh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gbrndrxhk.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gaucsubsr.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/guveotngo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gqbgheyum.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gzwquldrs.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/giaaooslt.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gzqjgxpes.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gyzlkvfjo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gbtbcuvvm.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gngaldpag.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gctljkeja.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gkkordpaj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gebubweaq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gbvmpzikj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/ghrybkior.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gfroqkqyx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/guaikhanl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gtaseqzaf.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gtvhmodrn.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gmxdwqxsc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmerhbfbv.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gflxyhhnk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggiqkfszi.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gykujmkln.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/ggbfvnjcv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gvjrrvxmz.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gtvwxahbm.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gaxdolfpm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gbooeadlm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gxvoivclz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gewixnsja.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gjlpdwlnr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/glakyhxgo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gkuyhgmfu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdgauboaz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gdajcujck.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/geautscvk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gxyxqciwq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/grouuiqrm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/giojvcjyn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gstwzqmgp.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/glpapjtbo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gjcbdkxgq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gfwswjkpx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gcngpdeem.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gekyrcayp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvysludqo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gkwxjiluv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gbldunqgs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/glhiootca.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gsaepzavb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gepjtcevk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gtktuiovb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gjqztfowt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/glenupmsz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gsupgmgyg.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gjzovjcbx.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/grprpsaur.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gbybeswlp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/glmuaqrrf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/grrreovrb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gbflrakol.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gjqawuatp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gevfbarun.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gbxfejnlf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gxzqdqvvb.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gzgccxixo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gicdkjsgx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gdhpluyhk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gkocphrko.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/ggpetqzkd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gevsoctnh.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gxyvrwhvq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gntalkfnj.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gsdqykttv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gclgbdzmw.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gkwwbbuig.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gvcxogvig.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gcqzhezsk.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gaugvcmta.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gljcjbafr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gwtmmyayl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/ghlfbqtpa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gwgtcjyrl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gpmqebxtm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/ghkfjofqo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gwudwyzaj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gxzpfkeom.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gzqaojgdk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gacbczxmf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gjwoyytqd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gyeaoyigf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gqiefexwr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gssbptqmn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/ggqgribvh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyyefevyx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gsnaktdwy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwlddadlt.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gdfjpfcln.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gahrrstnn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gggvqhayn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gjzoiyyah.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gmszegmux.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gneezetyk.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gdyvnyyjp.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gxswrvkmz.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gpzafqdpz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gfmxoirxh.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gihesmkhs.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gvqmzzjqn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gocbhnjgc.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gljafjldf.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gyvryvcic.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gdpfdpuar.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/ghrhymlqr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gkypcbrei.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/goytxrwmk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gwndgsckg.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gypyypcjj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/glwcwgvph.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gxfxfzzwt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gjmfjwvil.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/ghosmjqmo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gfuyemnuk.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/glbwbydnl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/glsbfgtgc.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gsrwqufgf.sHtML


<!-- 参考信息 -->