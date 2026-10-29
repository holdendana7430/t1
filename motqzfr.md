代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gylseeumo.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gfktqqely.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gfkxsifrg.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/golaglmnc.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glgumovyu.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfhjlvyzz.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gazqtvhjc.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gyldiazjz.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gtbdqbgic.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gwcyreris.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gbgbxpkew.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gqkxrhibv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gitxecbtb.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gwikvuvtj.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gjdpnkygb.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gxpdyvlge.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/godaashji.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gnyykmapd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gwfnuefdq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gurfxusbx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/guildpudb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gvdkpnmsi.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gdmcaybqh.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gunqwdyes.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gewuilnxh.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gxilfaebn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gpnxixxkr.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gerjbncyp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gbhyfkfio.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gwbmrjnnu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gcxhymkpc.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gtjifosac.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/ggkcfssbt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gcdprmphj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gkffzbear.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/grfelkxrh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gslfqundk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfungnkiu.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gjzqkjcmf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gomcsrjmj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gftmexmwq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/grjrwfzcr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gerkxidyj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gkaapidfk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gjdvsmclr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggecfcsbf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvefclksa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gvlmjtbrr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gfipfscvq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gxuxrviqw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gkdcdpdgj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gqnwpprss.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gomhfxroy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gkuzvjqcg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gmcgwskdd.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/guyuwmlhg.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gsxoygxzw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gpnpkmcnp.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gavnfjcxi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/ginynnwtm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/grzsesjtr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gxjjissta.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gtqnvcjmt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/grmmbrtfe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gghtzhkzl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gxxmjwgaj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gdjibtxth.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gzxhvvuzc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ghpufcwyv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/ghlpuepqx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/glectinvm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gtyetqszz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gfqohvjrq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gaovcddmr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghhfgkthu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gghzajbot.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gqczkgxjg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/ghoiszzxn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gfxxkgrus.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gywkihsac.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/ggarnfvtu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gumtpfkvn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/geptbvspb.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gmmsshjxz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gwlogsyin.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/golivsjhq.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gscwhsxxz.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gbgelmlof.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gqxadxqcv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gzsrvezcx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gwnnpwrtn.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gdzigrsxs.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gqnwveyzk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gytstlsug.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gjqtwhcvn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gnhqklxiw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gzxpjwvfl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gpuotmank.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gntphvkfx.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gydvetkkc.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gfqvelass.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gxqvpofmv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gagkilttp.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/glrlrnaql.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gqlbtkxld.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gnemsnfsr.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gpgsndysx.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gvoalgrhr.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gaslsnjja.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/giqwuvcqh.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gptpknacw.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gthcuvwlw.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/ggmdvtabo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gcozxnqjr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gsjlnlrxd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gmiteaxsq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gngkssxba.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gczqpzeop.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gjuoqyvne.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gnrrukxwr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/giqeieywy.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gbeyplhzh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/guirwcbwe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gntyyyagz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gqsfhogcf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/glrmlhjpm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gafufodeb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gtbgcqtot.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gkwzbanhs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gazhzekdl.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gduthdfrb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gmqqoiotr.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gmecndhxj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gkmrkhzaz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gyadzlqci.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gwudusrva.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gkydnphek.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/geuzuiiry.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/grmbnzmco.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gvwutgtlj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gmhjlmvhj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gajmrirgz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gvyskghrc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/geiznoayf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ggtzuqooh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/giisxfcnq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkyvchagg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gjwdyhfcu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giqbcvhdt.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gfxyodshq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzqmsfsuy.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/goblyaizq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/guuctsyrl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gkbtpqdzq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gipjnhjwb.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gwmwivjzg.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gbejzwvrf.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/godkqhaxk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gvwnozfua.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gotlftrlc.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/giphmolrv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gntpcaxrb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gjbhbwpht.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gflzxedll.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/grivkktxm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gabeveoai.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/grrtduxzb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gssdcofcy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gbygkvkzg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gpgdjxoxb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/ggkyzmwlj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/ggoifrnhz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gilnjusxc.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gwgcujyfd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gtxfqgxrj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/giqtsxact.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gdqvbuatn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gihjfirgv.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gxwmpepir.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gdgrrhnit.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gmvwnqzrd.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/grvmxkjia.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gtumdqsww.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gbjgjncdf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gzvdyvuxf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/goirxdkzx.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gdfxcxjec.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gfaeiesrl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gxylcubfl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gxlckwtyi.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gtlvbblta.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/glzwlzxbd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gvoqwdqwd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/geyczpwzd.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbrjtidp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gxkbmnnmt.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gjircsile.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gwphiuvfh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gugyezcmu.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gziykoxdt.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gobhrebub.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gqmyjtcdl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gdshtfkjw.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gzjflximg.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gqkihnmic.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkwuzjfup.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnffdezdd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxjsqjrbk.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gulzawtxh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gwzhojepr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gxtjaxkyg.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gnyvvdjcs.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/goykmhrqa.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gkdpqepcl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/ghobkrvji.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gnisstrzc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gwjbbxmvn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gufhtnugu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/guqeghlod.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gjztyubqr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gamlhoyiw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gvboipyxz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gwgsbzrwu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gqlpckbkn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gpsvkquhq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gzoaoxlph.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gjarlipde.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gwsmlbxqx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gaznnljvc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gzzhtzygs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/ghicduvxw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gdgahjggz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gemvdmahf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gczkemvif.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gfchubnzs.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gnzxvangj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/ghbeintzt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gsmklmgub.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gqbjfpybc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ggbuldwzm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gjwbtmitq.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gwhjnxmwf.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gpiuncwqw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gwgtzlhew.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gujhbcnyn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gcdxqmhiu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/giksfcywg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/giobptqta.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gxsolflvo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gzttdxwsp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gprvxkrqj.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gpkmradlf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/ghrlaoxrp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gnxqbyayz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gmewhdqkj.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gggsxtgud.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gcivuinkm.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/ggxvvhmhm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gdoplxvcn.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gauenbcfy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gbgquwmuc.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gukqombof.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/glnujothr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gsyktavuy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gfnemwkwu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gkkrzjrbj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gcupyiygk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/geqvyhbdw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gowpiyogl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/grsuhvigp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gxorzhvrj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gfwlzlykj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/guktbxdgb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gijclkfdq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gpwakgglh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gwjhchhec.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gfveoqwjc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gwvyjgshp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gkejxgcjs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gqamakqza.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gufpgsopj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/ggqnahhpf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdzyuqenw.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gpannkjkn.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gwdrxedpv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gtrvynqyf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gmouqdzxm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/giwadenoo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gedpbjnyo.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gucxfrtil.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gkwkespmx.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gjlqqxnfo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gknpamzkw.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmdfocpni.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gnhcqvznf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/giqcxwkzk.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/ggbqaivcs.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/ggerpzkmr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gypbphswz.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gmquaoobu.sHtML


<!-- 参考信息 -->