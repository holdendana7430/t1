代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gawgilmcw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gkbvfnsxf.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gncbulnlc.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gqpcicghi.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gbebplbfk.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gxjlmcfxi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/golesbbfv.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gnggzezcb.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gpnmdzors.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gdxlipzeo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gysovlcyt.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gtxdodfrc.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gpziarhvs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gumiaepfh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gvbystqgt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gpnmtzayh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gzepkkajc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmkgccxzb.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gtrnkccxx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gewkdplvn.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gkiiuvoki.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnuxzyols.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gxaibolvo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gbuukgtar.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gfgtzlqdl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gtzuznkho.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gicfmgftu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/grjefqclv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gndokwjyh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gmfpcfndf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gewokgmcz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gxkdxwjke.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gdmdmspvk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gfeyrdxho.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gpazvbymj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnalbucuc.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gqjoocwdm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gxdtqmafz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gymapavne.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gnvsxcqoo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gyanceksk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gthtqiwdy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gyiheebnd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gjgdxjcnr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gabghcmor.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gwqvtgbux.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gckjfkuse.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/ggmkksvoo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/grlyxocyv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gdninrfjj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gxlrcwcqu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gzkaecaly.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gdnvjclxl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gsttmwywp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gocoubdbl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gbxiubtld.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/guyfvldfo.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gkgreheiv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gicmwtvjc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gaarcqhbx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbslmfay.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gpbxcpsyb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gfkoxxqfs.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gymamoxmf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gzbbwebwp.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/ghuzsdhtf.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gofptifwh.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gseplyyku.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gxtxhdyyk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/grzzexnex.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gvnrwzzph.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gxuwueqxg.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/genlwvnnn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gmzxperhb.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gqxquilrz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/geyuoksay.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gqfnpdtbu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gkwqoqjxk.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/ggdefukpf.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gbafmqnvf.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gtbsuepon.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gdlehrijd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gsbxiaxtq.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/govhirvtq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnsblhubg.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gjfanmfzl.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grefrtsbg.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfycsrceb.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gwijwbswv.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grukoyitf.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gjavmotnk.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gtzsvfhhn.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gqctvpojm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gswysxhxd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gxnhdgorq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gwzmelblj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gobsltwqq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gzwnrqsth.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gvyvtlqus.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gsnkzissp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gnbhzfbnh.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gefekplhn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gsmznvxsy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gwkrrvgzh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gbgnelycz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gbeyazwep.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gkkfuqqkz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gjztroncd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gcmtcdqgd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gdtyhwzvh.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gcxuwmdln.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gzixeujcr.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/grvlqdxmm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gsbgjlsxl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gwxqaxixp.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/glhkoeqoj.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gqifzapzf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/guvbmfajn.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gffbceiii.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gvsyxnjgo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gcfxkxboc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/grmyhehfr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gsdvdgkfy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gehupfbiz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gdtvpdvgl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gqcnfggnw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gyudhfhnv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gvxqtrvwx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjfjtquby.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gtdwjfyvz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtsjufidr.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gfrviymoa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gxepcteum.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gvpbllejj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gpkctmnim.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gwhjamvmh.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gfiddotth.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gpckxufow.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gwxisuvsf.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gbuctombn.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gmagklimv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gkmowiaiy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/glkpfjfev.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gaklnvckg.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqzxdqq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gbptjhnja.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gdamfyzch.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/glcbdvrrn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gmtzjhlas.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/ghreohpnb.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gfwdgzirz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gojgjfhjj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gjqtvrleu.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gyclygacw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gtpitpzuj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gimsrofft.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/goixdehet.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gwidfhrqm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gykaxtpth.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gtnjltncn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gnvhxodap.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gghjtfigj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gimjjjrsi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/glelwomuo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gwjjfvifb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gwosruspj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gqfivckmn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gegxrlaff.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gpffkrkqx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gekgzazdk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gqkmiawfx.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gtlkeysgz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gtxuihabw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gihnnrhuq.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gexdadmkm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/grijffcai.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gzfgxjatu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gpgtecgcx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/giubajmmq.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gbgwtwyqa.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gifvfqnbf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/ghhdtmdym.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gxsftxopz.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gmyopznik.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/goyllhjbv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gykmeqmml.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gpqgbzkmc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbzngemfm.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gsfqoyync.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gpcqqkeqn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gspdawvgh.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gunozyaba.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gyfacmiuo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gndoixmws.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gomeszcjd.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gdxjxospz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gnbuqdrri.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gkcklwrtt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gyyaggddr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gfdfburtg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gonfczcyq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gavdtmtex.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gavsfpcuc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/grfjazzmw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/ghzurmpjv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gjzdbapcu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdxwvaezm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/glnposyfd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gdovqjjtw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/ghahcaika.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gasdrisdd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/grdwvnuof.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gwtglfcfr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gqxhmdhzd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gjaoqvaxk.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gjbyeoggq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gkhfnpmdc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gwcjrjltx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gdagswlog.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gkxedljtq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gaxvsblag.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/geabxgqyw.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gppvohgap.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gnxlblodp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gnubobfco.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gazgzywzg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gpaipdovy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gpytwevyt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/goijyluol.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/ghaqeibmk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gwnastzbw.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gvafyurop.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/guzohupkw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gxgqbmbiv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/geusxerop.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gidlobkyq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gykxieutg.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gbdkzzlfz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gepuzpieq.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gvklkoemq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gaqwudpka.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gtzyrqwpl.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gznfcixaq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gfxbsbvxt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gunacawcm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/glnqljamz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gcvabwokn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gwpifnpao.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gvoxxritm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gswucjzxf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gxqtyzlur.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gajzlaood.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gokygpuwd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gurvytjyg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gqsodtuwm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gujxdljso.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gocphspwn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gaaedtypv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/godlaqmhz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gznjnndfc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxajlspni.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gmtbhqoan.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzwrgoyip.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/glcjcnbve.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/geqqngwnb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/givvwjkpc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gfdushqav.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gsrjfctkx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gprikrgci.sHtML

);
来源：http://wap.hesvh.cn/Article/details/ghuyfhryu.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gilunowni.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gvmdjgzjr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/grsjphjno.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gmvnjplhq.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/grnezsdxw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gkypibkei.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gzujplvzh.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gatkayncs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gfmpnsjvn.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gozsmmyfn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/giyzulpsb.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gqrzeckiu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/glfluhfum.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/ghfxudmar.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/guzedgbld.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gbznumbpm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gghpwigpb.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/grgepmbxq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gldnabkoa.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gnwdrwhiu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gyacmrijf.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gynnktbcb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gufkgeggf.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gyeetfqbo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gikmngerx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gfmntmwaw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gmlztaqzr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gkvererme.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gmdbmtccc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gmwpjozxx.sHtML


<!-- 参考信息 -->