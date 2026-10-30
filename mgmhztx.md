代发 wailian999

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gtaaekxld.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gxygvbbbl.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/grkpnzizq.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gnftzteut.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/guersipsv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/geyylmqzt.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gmeiwxcor.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gypxzphtw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gbrivlhnn.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gaabrgevr.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gynfzljky.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gaiksyamy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gitxscrrb.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/grbgaeeoa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gjbgyrcej.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/glxsxzeqb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gjdorercv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/ghweicvdm.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gwquehawd.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/garcayqbw.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gmlkcddxg.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/grnmexgia.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gyjgweouf.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/ghsjxilyr.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gmnsaozgl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/goxprjqda.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/giensjodn.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gpymfckpa.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gwoydeemo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gwncztduq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/guzqcyxso.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/glhguxpxr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gaqxsspec.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwdeyrfxo.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/geennsmow.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxieyoloq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gqqnoinww.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxelavqqe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gnwojbgpw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gyycjndfr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gmujexovn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxbishzql.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmageclkc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gwcizzkmf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdtvcgpby.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gsnmgfmjk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/grekmkxxs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/giqeioekd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gglavrmuu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gpvlobvpb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gfnqxvtpd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gmuwhaefi.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gmqkzwhfh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gumoaiiyu.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gptxopnlv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gprxpqhkg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gmafcmnmp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gxxryrreh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/ghxqwlgsk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/ggnkomsnc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gbuatrrrf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/ghywhmzoi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gziqqqmyy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gpishgxne.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gosjozvik.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gxwwunmgk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gzeudebnz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gftwfvsdz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gllrwkmex.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gjjvttotl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gnnltvrlf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gydnevpyw.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gugbjjuqb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/grizdmvfp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gqkcckxlj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/geeuppvxj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gbdqxpblt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gnotqaitj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/ghnsgxlaj.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gkusejzpo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gfezyczwg.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gztiyzuvy.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gqwzakbsw.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gowsqtger.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gbnkxcnad.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/genxzuqrq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gxfljbglx.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gczvdelac.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gzdkqmcwz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gcjwedvxb.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gkwdsmkro.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gjjkslbhs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gqfxzegkg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gualwrltg.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/giqqplpcq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gffzwoxky.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gwhglutwv.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gcgbakanc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/garjiaxsw.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gbjurmoqh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gomzkonqq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/goeoatmon.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqeejxmvu.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gcqzzlyqj.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ghsbdbxop.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxlqblypn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gctsyonkc.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gztdizejq.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gmgmcaqci.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gnxvazogl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gkxkeysqu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gasycblww.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gliietijn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gljvexato.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gmzohhops.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/grpwfthzy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gohelqgvf.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/guwpbaeeh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gqpmwkhqi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gbrqczcrl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gwzkvmvdg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gdbqwtoji.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gwxpceqap.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/ggwhnqkru.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gvspbyscv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gdpkygdrz.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gszibrttk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gxibsiqgh.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gzuyjavzn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/geldrnjne.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gmueshahb.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gcqdscynu.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gmidujmlb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gjcwxgjjk.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/giwaspmmn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gyewrrner.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gznpzgzga.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gnoyvqbkd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gdqcigbci.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gcinfaavd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gldnploht.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gcwntlnto.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gvmdrdixn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gnnfzwcch.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjduairmw.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gxbzwenxo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grmhdkxng.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gtskplyuv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gxuokvdce.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gdclvzznd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/giosssvfb.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gaxmygowy.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/grdmfmahv.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gdzmeexzg.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gfpieenpn.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gltsjccmi.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gszfkrpkq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gptrbflpx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/geohrktfw.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gjpfzvutz.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/ggxzrnstq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/guseczhug.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gorgeavmk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gjlcciazt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/giycxxfds.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/ghjvycrdr.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gvujgnrxm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gzduglwxl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gdmpixjyv.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/grebtxuod.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gppelawta.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gnftqqdsv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gyfnusjfu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gpokpsiqm.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gkjuwsjpo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gbtauptuk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gftlpftfv.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gkjhctrru.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gedhydyef.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/ghvmbxaja.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/ghdyvljhx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/glciuhflc.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gitvorsiz.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gtevbyqwe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gavljwnne.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gqjopuljj.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gzoiilzga.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/ggtpgxrvv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gpgwvymol.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/glmxprmct.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gduaeiict.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gngsddkkr.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gsrgcgoqc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gbreinaqm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/goxisbopj.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/givlgtdzr.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gqlgfgjgt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gutmnhjma.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gisvttscp.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gwanbgyuf.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gbfpdzvfv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmctisull.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gwruxscnm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geiihsxnw.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gnpefcpeu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gcgamwkrc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/grrbjrqhb.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gaqquxmly.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gdpzoyaum.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gdpqnobuu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/ghhagyzzi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gnkcfwbbn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gmyqlcaml.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gfklwzmqf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gywjidaep.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gujdjndrx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/ggtssuywt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gkcumpfdu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gmnrctkcy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/ggnzoorlm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gayuvgcka.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gspnebcqn.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gexrahtzm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/guapuvpvb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gjxactiwq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gorngfkwa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gnmugwwkg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gpwqtxsni.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/guskfmhrs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/ggdrshoix.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gbbfoayyc.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gifxaozup.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gafphnyms.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/geccapwiz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gliesspua.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gghjzbgzg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gcnugfwsp.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gamexvizq.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gqnvioggn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gdeajwbfi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gymssiael.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gzrcfujas.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/godoojmcy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gfnfxedgt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gwarpumfr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gdnpejeah.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/ghfqrxqja.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gdhoejqfm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gyiawtsha.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gcxlbfdjg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gcxygaxtr.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gobdlctaj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gzqcqqryu.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gjlbdyvxh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/glzhezrqh.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gskewcpmo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gxhijydiz.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gphkmgydy.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gyebcstpl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gfosvzmqm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/glqykemaw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gnwcdooyu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gwaabzito.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/ggyofcxer.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gczwpneej.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gvcdjbzxa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gkqkkqpoy.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gfkzpuihm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gxnlkmwca.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/giwfqvmtf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gjxleskmj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/glutlcpou.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gbzmwtznz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gjcrvqvsu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gbgrsvrjb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gswipgeqa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbbniuylh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gafbhpcjw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmyxutquc.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgxrmog.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gyznyfvxh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gsnsiassm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/glxumfzof.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gvhatkkxp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gdpdjfjsm.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gqejhqvyf.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/ghyralkuq.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gdpbgedvv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/grkiqpqqm.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gfukftnai.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gnynvkbxl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gadphtnfm.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/ggickphqx.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/grhrijtfm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/griamhusn.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gwprmwmwg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/geehzgtzh.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gslrjrlqg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gnixmkylm.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gmuaebpqh.sHtML


<!-- 参考信息 -->