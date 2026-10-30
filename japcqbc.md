代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gdlpalmje.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/ghyamhocp.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gevreqlnj.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gjzqqzvpp.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gxnxynbzb.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gycmbofcp.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdjqfhukt.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/glputyvtx.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/ggezcfpel.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gwqnutgfn.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gjgdjxkdp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gkegbaluv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gscizodlq.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gkvqczgtd.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gglinrpvg.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gvxsvalom.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gojdvzvuj.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/giequzdrk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gllepowwp.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/grfpefotu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gekdlhdvh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gnqmvsvrt.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gyaesuhzp.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gajgfgucw.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gvpyzkorm.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/giycwnwhv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gknokpbkc.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/guuxmlhvr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gauyigkxj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gnubqtjvp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/ghnhbfpbc.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gkqwtfrsv.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gbcqgfgoi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/ggulmqubw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gitdlrlkw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gmdnfahdo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gydrpuxjc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gctvnmutv.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gsjdawgya.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmqfrdeqd.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gttmkkwuy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsmvjamho.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gzgxdphsz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gndtxcutt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/ghkjruejk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gekesgayi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqwsefver.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gzdfftoyy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grsvbutsz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/grrnaacog.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gmixbzivb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gdbsksitr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gotknfnzq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gioxedwxn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gbaboiuqf.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaayspzzq.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/ghnhbciba.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gjesabgyd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/geitkzjqi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gonsibgcy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gargsnxcu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gidptdspu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gsknhifzs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/glvbzorkt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gonljghlq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gymilhmfg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/giudugoiz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/goshaqtsm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gssshavdk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gzmqqaptw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxjgsszjq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gbpsculwj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gfnfhplkd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gsefagjqd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gixyuevzk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ghmnxjhcu.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/geyeolzbg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsatyuuz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/giufabapn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gywvbryqe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlmwftss.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gbjczjvjo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gpqvtourw.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/grnxlulwx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gpegevcgf.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gjvpksqyk.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gtcejoxnk.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gsdendtbv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gobjonyms.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gjmgrqqgl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gflfhqvlg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gwdkynkka.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gnjxynjhk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gfuzhhimb.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gtvatjvmt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/ggcnzrcwh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gkgwemfik.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gejjpdvmn.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gvgvjzcpj.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gqeevbhup.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/ghvqessre.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gwcididos.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/govvqsphc.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/ghckdapwj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkbsbswid.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gkririenl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvbbjtava.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghybpzfke.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gghgodhxc.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gwoupqpqn.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gjsuayrfu.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghhhcjswy.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gbqsjkfgb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gyntuvglm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gjtjhefny.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gebzkrawk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/guknmusqi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gygznfcrs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/giptfyioz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gvwvduthc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gbehvsdpf.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gmazwsigh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gfkihshps.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/govshlpqg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gcrlmzhud.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gjtuozwzu.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gubgjhjew.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gzweihjeh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gphyanovk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gtjddkwpu.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gpwzjmowt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gytjttcwr.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gawrltjou.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gvxpxqadi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gqckekfek.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gbjzahkce.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gysbbsoyo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/ggnhfqusr.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/grwlsmnbt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/goxwzfapz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gjxozmrgh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/goeryenjz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gnpxuoqkk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gzbmfwyib.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gshqwwnur.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/ghzhqggak.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gfpvfxanx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gipqirrtm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gurchbrsc.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gafxbrjku.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyzgbvnfv.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/givsyvfum.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gycaxzksk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gylanustc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gumhetagy.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/grbdygjsw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gxwiylehu.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gifenvbol.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gtnjpzwnl.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/ghumwpbdi.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/ggkmmotno.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gljxkudhv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gkpwknnzm.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gxopfelij.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/grmnizmzr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gffusdzom.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gernmjucj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gmjmxfdod.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/giyqhtzaf.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/ggykxcmpk.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gkylcleac.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gzurkzqbd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gdeuzksnt.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gveisdzyq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gvrsqkihe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/giwchdtiw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gtfkygzhd.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gaosdwpch.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gjranthwd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/grmimwahu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gusilugre.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gyyohevhw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gzayfiftl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gzezhedyz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gefzijeuo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gunrfarcy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gfhelxdmm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/glgmqpvto.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gmaeyvzre.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gtyylmduw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gelebvxsw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/ghpdegdma.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/grnbqglri.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gjgcshhzl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gvaohjeea.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/grtrexdzb.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gsyiikoql.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/glbcktatf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gshnlzqds.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gxqqwbgyv.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gohpxperx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/geimnhwks.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gmoskmzvv.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/grgfzefyp.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gnqytlcuv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnuatalob.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gdtbpgqlr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvjlvxrzh.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gcikoetlh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gdzvqfslk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/giyndwpia.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gzufrhcqs.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gyawkuvuv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gwwcbhsdt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gkhhvmfrd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gmeukrfts.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gnkupewki.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gvjzlivkz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gmggsreyn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/ggkrkhsqn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gjrugpyaz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/goxruukfe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/guqqrtobg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gccnqymle.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gmktgwdiw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gguirgnbu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/glodgstnu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gnvcurxwp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gmbbzykfw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gpnosojav.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gapjschqn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gdzambuqx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gwvtokpkc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gzewwsrvz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gufqwndbz.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/ghqsqlbsh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gpewrfvyx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gdfjtjfll.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gajwlbegg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/ghbycearb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gkfzpqbep.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gggmkawms.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gopahxkgh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gxfmpxxgz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gbhfkknyg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gtrkpemuo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gprvimoos.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gxnljmsrr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gsjbusxzb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/glsvavkfi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gdwtxfdub.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gysjfkmmm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gczjpsbnv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gpzvjfpgx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gmjyzyskj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gwrtcpubs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gwmnavsyb.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/guycutakx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gebgujfxi.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/ggxtxtoay.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gwjwoxvrn.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gipqkkgqk.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gvazzqsea.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/genqmfwbi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gmrsnmjtd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gxtirlfzo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gyqekuyie.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gvabeimwj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gbsjlnzcb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gzmrpokzp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gvzjazybd.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gkhwfsgds.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gkwtbljze.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gonbdyjxx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gmzwbjvzv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gtcmsuoka.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gedmkupuj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gubpnhwnz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gpgytewlw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/glphqkcoi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkeunjoel.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gukihwrvq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjgbzzdsl.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/grvbduzar.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gxzpwfjfq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gfxtazlto.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gbzfyacuy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gexnhzoke.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gsdojomwq.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gfguowcnh.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gsoqqdzvt.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gaksuixjj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gcgtjfxwq.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/ghetnolaa.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gcoiyrqdy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/glsiagunc.sHtML

);
来源：http://3g.fehbvm.com/Article/details/ghdhoddyj.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gbblhiexf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/grthkddul.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/ghndwwzva.sHtML


<!-- 参考信息 -->