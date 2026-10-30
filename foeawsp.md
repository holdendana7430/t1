代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/glqswfrad.sHtML

JS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gvkqcovbf.sHtML

TS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/grjfofytx.sHtML

Java: System.err.println("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtybpootb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fanxiaobao.xyz/Article/details/gsqqqerzb.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtqnbxgg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gkvfhqnkb.sHtML

[M07] 判断是否为主入口
来源：http://wap.fanxiaobao.xyz/Article/details/gyrfoowvr.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fanxiaobao.xyz/Article/details/gqiuhuugg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fanxiaobao.xyz/Article/details/gjeibthly.sHtML

JS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/griswvuki.sHtML

TS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlctbjqs.sHtML

Java: public static void main(String[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/gxqdpsuyd.sHtML

Go:   func main()
来源：http://www.share.fanxiaobao.xyz/Article/details/gffxsqfoy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/gbrptzgsw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtghxrcru.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fanxiaobao.xyz/Article/details/guzmvoetw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fanxiaobao.xyz/Article/details/gxjbaijgc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcowsiwaw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjwwlzyx.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeqdnizf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdnvxgrw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjkyoihl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fanxiaobao.xyz/Article/details/gkpfebymh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fanxiaobao.xyz/Article/details/gixvtovup.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyjvywmhu.sHtML

N. 数据结构与算法
来源：http://baike.fanxiaobao.xyz/Article/details/geyfxasqg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gguntgfgp.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gdbryzcde.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gjehvmhug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glknbztsl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkjcfapg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gzljvihma.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqjblubp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gltqslwlh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fanxiaobao.xyz/Article/details/gxzgptvti.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gzlcnxqde.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdijpsab.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtgvmets.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gyjlrfvgr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gogysbtbp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gutgqvssp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gauhnwxbo.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxknscpi.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gzunoplmv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmkmdjsf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegfzpuyt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedisdvfh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrpqvdol.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpqxxqla.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gciuxdsve.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gmzditite.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndsabzgt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbaiighk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fanxiaobao.xyz/Article/details/gvbtccdgw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdcrdjas.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/guqkborzr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzxfdived.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwptougmi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjicqhawh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/gzeikgmfz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiumrfny.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gossayjjv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gilitxyhf.sHtML

[N05] 最大公约数
来源：http://3g.fanxiaobao.xyz/Article/details/gfqsnbwmm.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gejmpphwi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/glqubdqbs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcmdlqjk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvihoolq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fanxiaobao.xyz/Article/details/gwntcbitk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkzbhdyx.sHtML

Ruby: a.gcd(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gcwfnaeob.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkwayijin.sHtML

[N06] 判断回文字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gutarxbzk.sHtML

Py:   s == s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gyylwlpbh.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gncdfsdau.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvjuaucs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/grkmgkdzu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fanxiaobao.xyz/Article/details/gariyivpp.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gjtezqizh.sHtML

Ruby: s == s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqihatbh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/gnzqqptdu.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fanxiaobao.xyz/Article/details/gqhmkwxum.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fanxiaobao.xyz/Article/details/gelqabqre.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fanxiaobao.xyz/Article/details/glihkfhqm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhpslyrt.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbrsumfa.sHtML

Java: // 手写 HashMap
来源：http://baike.fanxiaobao.xyz/Article/details/grxfzjpmv.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fanxiaobao.xyz/Article/details/gcdmtyvgs.sHtML

Ruby: // 手写 Hash
来源：http://3g.fanxiaobao.xyz/Article/details/gqyccznuc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/gkdrzvznk.sHtML

[N08] 生成全排列
来源：http://3g.fanxiaobao.xyz/Article/details/gcvdtawvj.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gyslzwtbj.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkitslopi.sHtML

JS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gnuxxibzl.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkrnfcbv.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxylqktid.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnfobfud.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gmenqlsgd.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlatkrhd.sHtML

[N09] 栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtojnbfe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gwiapqnxk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwwtmybv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gwpaptxch.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/ghwlpvwqn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvxacwqg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fanxiaobao.xyz/Article/details/gswvdabzv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtazfhrwm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/gycbdcfko.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giotibooz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fanxiaobao.xyz/Article/details/gibfkdqob.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhsobaoy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnvjaqgl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gopyiwggf.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gihoiawsy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fanxiaobao.xyz/Article/details/glvjgbuja.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcemejkv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlqmzfux.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gtamydhrj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/gbijrvpds.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxbiizsz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuhkfkid.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/ghycqftsl.sHtML

Java: // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxbwvnpc.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gojzeydzo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/gkjracdyp.sHtML

C#:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpekvxpeo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjhnyqpj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fanxiaobao.xyz/Article/details/grgdceqov.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fanxiaobao.xyz/Article/details/gglksorou.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/glsvoigut.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfajviho.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxlufrkz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/gpvkhbiyd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzbywthu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gihdqfeko.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgbomskc.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/gnnefcgkk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjvyfwah.sHtML

[O01] 启动一个线程
来源：http://baike.fanxiaobao.xyz/Article/details/ghudzrmul.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhiyrili.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fanxiaobao.xyz/Article/details/gaxfayoqy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfttigti.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwscofcm.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtnmjxlr.sHtML

Go:   go f()
来源：http://www.share.fanxiaobao.xyz/Article/details/gegiasqrg.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbpntzjc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtfumjud.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gsavbbsyd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjymemthi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbscghzm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeehlmgc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gmaurjpjm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gvdbuwwlu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/guuzbiwyh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjcyfsnb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdtmvbpn.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaqtjwyr.sHtML

Py:   with lock: shared += 1
来源：http://wap.fanxiaobao.xyz/Article/details/glhkhcjqu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gofyhlhkt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fanxiaobao.xyz/Article/details/gkexxuvez.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gujyvzqqj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbiknnzll.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fanxiaobao.xyz/Article/details/guccuuqaa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gobrjeeor.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoflhhql.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gojwkmjbp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fanxiaobao.xyz/Article/details/gekcmvpsk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fanxiaobao.xyz/Article/details/glpamkwae.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvqphlwrv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdotqkaj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fanxiaobao.xyz/Article/details/gqsukpcmc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlvwxidi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fanxiaobao.xyz/Article/details/gwttdcndw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gijvhfnkd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fanxiaobao.xyz/Article/details/gruwqsgpn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/glhankpie.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fanxiaobao.xyz/Article/details/gogqdalju.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvwkszpg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxmnmzgo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/ghwaqkwrr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqeygyfs.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdxjvjex.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fanxiaobao.xyz/Article/details/guimhecpl.sHtML

[O06] 使用进程池
来源：http://wap.fanxiaobao.xyz/Article/details/gztflpsmj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fanxiaobao.xyz/Article/details/gchwcytld.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzgddgxg.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gejnrhncp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/geaflluqk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/gipohntpl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqydyffv.sHtML

Ruby: // fork 块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknzydhen.sHtML

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkeoxfxy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggurlaqwi.sHtML

P. 常用工具函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcqtmkmlg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvkiiwsfs.sHtML

[P01] 生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedjazvbg.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fanxiaobao.xyz/Article/details/ggamrtzzx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxlxokrq.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggczfmobl.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjhudmm.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpibgfuh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gzrcyftui.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gebetsczn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoudqhtb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fanxiaobao.xyz/Article/details/gsibhcvmq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fanxiaobao.xyz/Article/details/gogpxafua.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gtwakniiv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gatlyudil.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fanxiaobao.xyz/Article/details/giaqydqns.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghovahmtk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/grgpxhjbg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohbhqhjf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fanxiaobao.xyz/Article/details/gluzqqgfq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlrfdcof.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/gjychnnla.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmxlwloh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gockyghvo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygbgckrq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fanxiaobao.xyz/Article/details/glnguqpwi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fanxiaobao.xyz/Article/details/grvflvrga.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gytpfxlrr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fanxiaobao.xyz/Article/details/gvpddrfbm.sHtML

[P04] 求长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyzhapia.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzzvsegg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwqpmgcw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmsxbtsd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gctvwghbi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gfviaivkx.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjloajcgd.sHtML

Ruby: x.length;  x.size
来源：http://wap.fanxiaobao.xyz/Article/details/gyzgsbpsj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gppqauuei.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fanxiaobao.xyz/Article/details/gapcfvsmi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fanxiaobao.xyz/Article/details/gfkbnnbed.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gypylohmv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fanxiaobao.xyz/Article/details/gigmiigzm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gipmqlofk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fanxiaobao.xyz/Article/details/gmvfmjmrq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/ghdjurtir.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gnqbpiswu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gwteuhilg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fanxiaobao.xyz/Article/details/grdzoffod.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxwdtlso.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grkhhrpea.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjesrwdx.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfaqtqsg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcjbnohqh.sHtML

Go:   if x == nil {}
来源：http://blog.fanxiaobao.xyz/Article/details/gltpohuhk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fanxiaobao.xyz/Article/details/gfhpafjju.sHtML

C#:   if (x is null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfacsvtio.sHtML

[P07] 防抖与节流
来源：http://mobile.fanxiaobao.xyz/Article/details/greucjawt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fanxiaobao.xyz/Article/details/gxerpaxmf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gojhdwycr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/guvgvuolw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyscngtrz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkwchwjl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduotdcst.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeicxkxf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fanxiaobao.xyz/Article/details/ganvshhdb.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fanxiaobao.xyz/Article/details/gagnzhpyw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fanxiaobao.xyz/Article/details/gsysbtsec.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gadurnprb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fanxiaobao.xyz/Article/details/gooxmvmjq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gehfhwgvb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/gzqgocrdl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fanxiaobao.xyz/Article/details/gfslinnzt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/ghhmhmumw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gdviytjdo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjsloimj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzihmuaj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grobngtoi.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gmxbsfeew.sHtML

CREATE TABLE users (
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzsnbbho.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gimehozfh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaygmomf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fanxiaobao.xyz/Article/details/gvlakvhxv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gggitapyx.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggomtlrmm.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gziseajqy.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/griqzyzbj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbqjvrwg.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gujyidosl.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuftgkwv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkagtgbtp.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/geawwueim.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmeurevi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrqwxpby.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gwfdclrcr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gggwuoyqv.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxboedxt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnjpexpc.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwqkewgo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtkwmbid.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/glmrvzryq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbxvaqjw.sHtML

[Q08] 创建普通索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gxurgpajj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/ghotbfodf.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/glypcyweh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gbowofizc.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gojttzpsx.sHtML


<!-- 参考信息 -->