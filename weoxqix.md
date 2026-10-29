代发 wailian999

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gylfugxjz.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtoqxjzki.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbxykaoav.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gahqxzsmw.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gsozguxxz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/ggyfwcibd.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/ghvveieif.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gwrtdhsgw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gikznabjn.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/goahhlyad.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gcngmczht.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gynmxlixf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/giffwkzmg.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gnomrxbxs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gmvpgmyjm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gkokalgwp.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gfdfhobej.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/guendazed.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gzqqpecji.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gzuozxzfy.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gjnemoxfv.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gcvnyvszz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gvjezdckf.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrhrquzu.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/giaecwaws.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gorlcyxuu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gwskvtadb.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gywwpqbkh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gfghwomak.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gomujhiew.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gxktaiyfo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gjhinhkek.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gbkafoiui.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvmthobnk.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gmtyyuxdu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfhddarit.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gsingykde.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gsdmhmsbq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gcnzhadsm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gnpckbyzv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ggrmtftrc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwrpthsam.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gijbjceac.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gsmcpqonw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpkphqbiw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/ghoounxzb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gtgmfcamb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/giozuowln.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gbjgfvclk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/guqnsdxkw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gvfzvugie.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyutagkdz.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gaaewkzuk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gnjkurpus.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gfnkbklcy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gqjdjmqui.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gozzylsiz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gfpauibfx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/grinjrewp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gffontaxx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gvqroswut.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gzayecypu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/ggtzljwbx.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/ghifsofoq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gbhpsoouq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gjizyrjuv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gzjdpgmoa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gshnyervx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gdwdketim.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gavpbrtqi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gqpnbirnq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/grjxdkmlp.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gmxszlxfx.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gjhzystag.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gerlmftcc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gihhcydvd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gicieetbv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gubsdoctf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gptdkavui.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gkrcqzkfy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gmvqaoyei.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gpawcclge.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gpzyviixh.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/glgysblnn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gcupbesbf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gxylrhshz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gpsfvrlss.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gcjyfuisz.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gakwyfcxr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gwoxxzchy.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/ggkamgfdg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gxwgpplhz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/guxhwiuxt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gjdryettw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gbpaosrfv.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/grcziuqob.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gmxhvdgxe.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/glvhlrdnw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gkqjhtszr.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gloqkqdeh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gaoknbbed.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gfzjakjyt.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gkkrhwcbf.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnnhsccim.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdownqast.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gmajsxqey.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gvdsulhbn.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/giixcnhlr.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gmyicgvrc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gdariqeiw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gpehrwaeo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gsfnedjnj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gaswjwric.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gaxceihyv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gqxmvpzfj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gaqrqkrge.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gjulrpzjx.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/glmgizpku.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gzndbsfjz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gflkvzgno.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gomngixrr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gjcnovlof.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gksejbqur.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/ghwqlaiii.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gqxlldfqu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gctnrwnfy.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gmgcngaqa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/ggmtgkdpl.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gucejukbu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gwtifumwf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gzvqzrckx.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gcgckvnmu.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gcmepdbzc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gigxbusqk.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gloccuzid.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gczxmlhfo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gfuckbjnj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gfewamcmd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gkhtcvaij.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gfjrfplqa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gjwxqtjtb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gzvdwpsrl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gauphyvhr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gpmevqmgz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggscgajqy.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gdplcpeuu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gctasnprc.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gmorlvsuc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gjtdectkn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gnthdjivv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/glhyrfidb.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gbmhlhdcy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gqvzpcxcv.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gkppcxqvu.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gmonluoep.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gebxwxqgt.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/goxkrwpbh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gagrbapac.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gytspxzro.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gkzesujqq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/goeymikij.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gnsbjbaau.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gqmrgkzxp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gbexpoagm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/glhnlsrls.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gdbdbwfeg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gjrrllxuw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gexafxioa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gnlxjrxjf.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gksyrtjfc.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/glqffvmlp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/goltktzky.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gktzvjczv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqcaqjwm.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/geirailpo.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gptenaean.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gefmflfvt.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/geapolvez.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gnxkinkll.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/ghwzuvxim.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/giszlejvn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gazehspbp.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gahjwzhvh.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gcbtztfje.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gfmuehwuu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gggfkjitl.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gbcqdevfp.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gbsugvqps.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gtxzmzlnr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/glgldyfzj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gitlzjchz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gqbibtojo.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gvqrjzyfb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/grhwugmgl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gmtwaqayp.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gnaiuzvno.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/guezsolgx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/grplqkuys.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/grkqqyyyg.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/ggrfmbpcl.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gnwmgfdjh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzigxnajx.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gdwtggbyp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdyihbrxp.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gdrdpxgxk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gxunykmsw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/grlvoiehu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/grgwdzwav.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gkrwdyptf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gybrzouvp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gvbzujzau.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gmosujnen.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/giyxzdaes.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/ghuadjagk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/ggmdgstea.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/ggqgehqap.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/glmmllpgy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gvqkiwzoj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gtinphvil.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gyfrlnwqd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gdiwumamn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gkxzhtvlb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gimqflerw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gvsfhklrj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gzlslnect.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gylcpdarr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gkpaxpuuy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gpanmulha.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gsguugotp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gficyaduj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gphnfylwz.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gmcemcphc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gqfxkmfgq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gryhgvxdq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/guzbynrlp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gryqukddm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gmhypbdeg.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gwbfonwev.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gihobfnwl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gkodmirlr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gjksdwljo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gzlflylni.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gclaytfol.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gxnonglru.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gcpkeijuf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gcsrzuboo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gnqkqdvgb.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gafcrmqlm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gbkmkmkjx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gipejqkuh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gnkesiram.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqqzwhcjc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gmrtxziit.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gdywwkkme.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/grwazcjdq.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gfpudfokp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/ggydlcsqg.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gnpvgwcbv.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gvbgfdrrj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gjpvzyrms.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gpumcblqp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/guxjwqqac.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gojukxglr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gmtmhyvrl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/ggdhsnhcs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gqzkedulo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gsdytatfu.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/guhodicmo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gcanxylyf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvuknqtpa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gweqdnrmo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gpojmmpdc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gemnwupgf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gssoyhwea.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/ggsyhjqhi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gajyhelpf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdtmugwjn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gpychcnni.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gymdccsid.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gmbnflloo.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gldzgmhyl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gaypcdavn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gvatuihti.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gxheplihh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gnexktxhh.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gzppiazez.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/ggqtcdwej.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gpkctmril.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/ghelsabmo.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/ggtyzxdio.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/ggsbrylgo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gfkbmsmht.sHtML

);
来源：http://blog.fehbvm.com/Article/details/glmsmurbq.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gyfolehly.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gxjznidol.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/geoenxrit.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gbtgbduuc.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gptdmloat.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gmijtrgxd.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gwfdzosms.sHtML


<!-- 参考信息 -->