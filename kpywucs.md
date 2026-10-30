代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gcbhbfnor.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gxqyxapsa.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gtvablriy.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gygambenl.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnhpkdtls.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnmjkxqic.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gcbhxoqei.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/geeylgadv.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gsxcnwhqw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gmictplsk.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gdvhyhsjc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gpjfzsfeq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gbyeoshtj.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/grykzjcxu.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gkmkndgrj.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gmshkffdq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/geyqdztba.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/grsnyhafj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gcpulbmnq.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/ghzysuaaz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gbhoeleew.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/guhnioaep.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ghnfeaxbj.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gykcivzmo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gnrkfqaxj.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gktasbmek.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gpnskdmgk.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gukivmbkn.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gzidrayzb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/guelizobs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gizxdgzjs.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gjfwojqpi.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gxnjoctdd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gnvaeertu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gekjdlzqz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gxabxgduk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gkmxxlwsg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfmpxravt.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gutidhomp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gplligwxv.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gofedasdp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtsysesmn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gpmlkuuaf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gjbdfllap.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gkwykiknh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/goeafjrci.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqnomwktp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gkcsvhfcb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqkvtgqhk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gtpcmkkxf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gvzfwmohv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gttpqaths.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gqzdxnqqz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gktphkyot.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gpwgwtjnv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/ginzxjswq.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gvobzpnwv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gqmntkwwg.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gtzbwggub.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/ghjpodetb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/germqlclq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gajatcvig.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gdeymxgfs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gchqmktjm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gkplkhhpj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gpceslidq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gnpwvrcpm.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gdomwxfva.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gigubumoc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gqabecvgs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gkofqlkzo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwzkues.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gzokycxyl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gfyhxqcyp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/guunpxper.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gahkvwdau.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gzlpymymi.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/grnmhyzlb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gupxoytxg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/ggzbrnyfn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gtfyhvqsm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gabatpwwb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gyeiesezt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gyjxpwiew.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gnvnjqsaq.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gjxctpiyd.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/giefsuazt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gcdzhtqir.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gunsxqqrx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gniwibclg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gdzoqqvsn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gbmwnzsoo.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gxtlgxxlm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gpcgjihdk.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gvgirpgaq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gjxjamcsw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/glgdueuqu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gmmsolqrh.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gpuqossde.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gzhzkzgql.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gkhnlxhdl.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gwqexultm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gomyklbtz.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/ghfwqxlvu.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gerbodrsl.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gwvaoosjw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmwojjxoj.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gelxjcrfy.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gurqnydxk.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gbaadtvlx.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gimiavmlw.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gdvtiqidk.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gspjduihr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gngkzmlne.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gbqdysrjb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gkmqknyeq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gxfmsuohf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gyegsmoym.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gennekfcs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/guscwuogp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gthehomdq.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gpxxhtjtu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gdevxxhkl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/geoeqigpl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/ghdwlgmau.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gkxogmhtw.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gzxljdied.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gpnwuncyc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gpxuaedlc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/glxuymodg.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gzjnxsxdu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gdtvubpti.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gapljhike.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/ggaltpxga.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gbvglgjdi.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gvyujekye.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gfyoyspvt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gnlwkjkcb.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gltvvtloy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gbbqobxdg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gcmkphkbw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/ghbasetsj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gyypmijcv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gzgsyxisg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gahknkiyb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gedwmwwlc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/ghtrlolot.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gwtahgyua.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvcjzuooh.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gwmvubhpo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwrkulcun.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gutfeavmk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gxuvmwnxj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gddlifmep.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gqbpwgmsq.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gcynjvndb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/guzajagbu.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gogryoobr.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gknvxrdpy.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gkjbspbzu.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gjoudeqal.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/glgmqyfde.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gqalbtmsx.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gurzzzkjq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gnwbipgsa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gziqhbgxr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gtjscxfyv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/ghohldirs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gwnsqhkev.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gdifyvfud.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gjysqnrhv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/ghbkaklwb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gsyogxjsg.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/glegrmphh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gwasuyozp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjqgpeab.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gijebsskh.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gnvrqhvhq.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gziybohxv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gjgmcndzg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gywdinpnq.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gflbpogae.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gymybdqla.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gnocetvrj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gmbxgpvet.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gzpoeuife.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gybcbhzif.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gvnhcgzic.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gacoxpfkf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gnrgvrobs.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gfcrnqfcc.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gberljxpl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gjjdbhstw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gnobknsse.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gbefaioif.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gosegkwav.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gejnfkzwe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gssxrqqou.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqqvnhvos.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/ghdzamuxa.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gdweujnyp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/glppadpfp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/goldkajpc.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gkhubasqy.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gcdlszmlv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzyluersa.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gyyaanktw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqhwprlsz.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/grydppbxy.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gqemursug.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gpwhscxqi.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gawhsslwv.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxxpcvumu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gvrjwukfq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/glfqozspj.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gyyhsofvw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gayzayypv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gnqmcybsn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gydltawye.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gwcfsutjb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gbjlpgpci.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/geyvbvkdr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/guuriyzeb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gzuwrgwgr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gsxsmolfe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gzqtruuil.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gxqtwwwgi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gelbxbcid.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gvtkvurtf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gvzbhruco.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ggzwiuogt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghupofgxs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gjnfbovec.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/glrzfviwf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/ggsosoqyu.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gwtwqbstw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/ggbiyaiil.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gumaokvmp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gkbmowdgb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ghqvmrabf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gogrkktij.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gjcllxrvc.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gbrxpgkxb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gsrxsrmui.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gbwwqjvzw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/ghkhhkgdd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gfjqskhed.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gbaehdixt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gyriczxqj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gmjrwctub.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gmrabkqdc.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gerisdmsz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gynzprxwp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gdgnkwiod.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gysudcdal.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gdubdfuwv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/garjhkkpn.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gwnxeaqgi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gdihfiydr.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gogfbjtme.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gvhsbpugn.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gowxwiiiu.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gnjxgypej.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gwpxslnvl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gcqeersgg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gwfxaumis.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gikwjydga.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxpehnbcp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gfjqwkxga.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gtxihtniz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gmnpehjdr.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gehqvysao.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/ggoxczdzo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/givdvputs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gleodxxvy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gykaglrum.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gzrtaphev.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gcugsvtdy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gefrknmbj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gevkbmrvc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkzilkuhc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gmymrzixy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsyfttaru.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gycadpztu.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gbpadebmo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gaoyhoztr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gnkpgvyhw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gzfacrhsk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjjjntk.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gfdessgju.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gvrqgknop.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gctrsthfe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gsenexmwq.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gdcjmplvu.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gftknbpsz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gjehdzrkw.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gwdmcgpsj.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gvemyatgs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gyljzgeja.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gfrfeoyhr.sHtML


<!-- 参考信息 -->