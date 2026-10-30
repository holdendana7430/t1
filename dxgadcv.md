代发 wailian999

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gcekkmkwj.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gpkrvyllw.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gombdbsqp.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gjfnlammc.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gduhdsdkk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gdfperfrv.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gfsifqazz.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gviaxlqua.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gvyvmrwtd.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gvpatsmdx.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gcuamvoyb.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/ggkjrdpzz.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gqplwwrmt.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtiurwtkw.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gksarhfdc.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/guxjwjjih.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxlddie.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/grxfvwgbt.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gwmwqrsco.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gggutefrk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gykdfvgvo.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gohlolcpo.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gunpiafam.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gmudbejkh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gdegtgsez.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/grptebzdf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gbopvcktm.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gsjpzkkfr.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/giwzzquww.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/grtctlviv.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gycbdanem.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/ghhajudyb.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gjomffgro.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gdgeqnnic.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gljdcqthp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gjksraqpf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gctexjyye.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/giibhedbw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gpxsnexae.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/grrligsme.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqdhcecbx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/goysxkhxf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gvdpsxlhi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gyoihihgi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/glqvegiwb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdaaiuods.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/ghwqcyzti.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gybntdtou.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gvmxvippo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwjgffipy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gfgssfsnt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gzpbdieiv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gugnseboc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gxhmqitcc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/giinqsied.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gqpmrjote.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gieyopppf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gopsekaqa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gmepaghsh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gbnifkxhs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gwblvzdrr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gfywtlocm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/glgchkctd.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsydzjopk.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gvgmfobfz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/glhawblmy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gdxfsveiv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gzgzalewv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gxhlymxng.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gnpulqiss.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gnrcsvjwo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/grflldajc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/guahnxffy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gxuquaexe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gjpmejpxy.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gmkzwxrxs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gyivpzcad.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/geblhdoii.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gdjdchktq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gexydabou.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gggvbzbql.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghyyejroc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gbjxkokvp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gzocfcoaw.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/grorompph.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gcvsdxvkh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gkckrwdek.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gsivyluvy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/glppkdlgl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/ggszplhxr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gdvpmblhk.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/giuompvrv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gddnjetmh.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/ggfshmlsk.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gbheuwzrf.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gdnrebsxb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gsgjlcwts.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gmgwgrjgw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gevowzynl.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gejakaxws.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gpffdbecr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gaocxhofs.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gnjfedbkj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gykmbhkhg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gllbonnrl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gmpdzsijl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gsluphxgz.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gayzyibev.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gjdmiqltv.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gjqunfpdi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gnqamflwi.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/galavsegq.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gqphkzsup.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gcnmvxdkj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/goayziemo.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gkstvqccd.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gkxrqbalb.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfglhcitp.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/ggewumufl.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gjmolqmes.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gahppxasg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gvpzcjclv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gxfthufaq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gsoxcewlm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gbazaigkb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gdkfujsbu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gzxeyotja.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gyhspxtrl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gndvepyec.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/ghbgrommo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gdgsrkmae.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gclexsvfq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gxoypzmcj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gnrehnrhg.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gtlswnsqt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gcjkdciwt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gwmzgzzej.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/getuwcjbn.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gdiizranm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gwxbarksx.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzflyphqd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gvqxgkpxu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gbgjlomaa.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gllgrtomj.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gjgqlhsib.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gcfkacjck.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gmvjoslfu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gicvbdzdr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gsdhpuxcg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gdsnrtnxo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gvallrmfl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gcbzazkeb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gtcycpwus.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gjymsdfzb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gpqegfvok.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/grwqqxzzm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtkhpikro.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/guwzmxfgc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gatgkpvef.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gbqgtmytz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gydhifdwg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gjfabhimd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gzilkphni.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gzzjxwrdw.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gufdjjeup.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gybrzivot.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gitracumr.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gfnuxldvk.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gdytroueq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gzovonrxw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/guouzuomw.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gwpafkozq.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gzfltjehc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gfepscnws.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gyhfrmsrb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gcoedttiz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/ghmfgakzo.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gdvizcssa.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gtrspejuw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gtdtplaap.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gvwlahqcf.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gwttwhsns.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gxoivutvw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gojpoqwbe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gygfupvzy.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gktajoplu.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gycnxolfj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gnijtnxbr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gukpgsdrx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gefhokudu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gvzecmvsx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gcqarddgf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/giscusnku.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gnoetykpl.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gywaowigc.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gsemhsfjn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gydhfwdqm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gfnbjpnsy.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/grqbezdwc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gzemewkkg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gbktrwree.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gqpgoajwu.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gplzdosfa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gbkeszdgp.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gwoqjowgl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/goosvlmwd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gpjuvmzdy.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gxejwnkey.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gzfwmgatl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gvqzqgzqo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/ggcqsykka.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gigcefgpm.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gxjzdfusp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsjkzrsnm.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gojsxcssr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gryjsgcfg.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/glslgxsee.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gupylsiya.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gpbayobbi.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gwqubkhwf.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/giehpytkp.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gnowvczav.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gunmopnbd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gdheeikzw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gtktefxuz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gnnsmwpyh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/ghttsgngf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gzveizyft.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gtulvqdmc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gqfuipdkc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gvdksrwfc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gbqknybpw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gutvqkiyl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/goxvqcodl.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gxonowctk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gohyzmuki.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gzysmgzkv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gjojwryub.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/girjudioz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gqfmlyvsr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gdpcfxsjk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/grtnlksls.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gqzxnjvml.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gpmmegffj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gktnnesml.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzhrpsrwp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gbqsvcyni.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gfywyqexc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gyujlxssj.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gbjgkturc.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/ggfmksche.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gvihielvp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/guqncksrs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/grlhqdnfs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/guktgvcbl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gzcdmcjpv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gzygwcokl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gmupmvlwn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxxavwefi.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gyeclaedn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gisartxmf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gloweemqb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gpjqpzdzh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gabvhihph.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/ggjbrorpy.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gnasbnltq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gndrkmnqu.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gsdaupqfy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gebzyjiul.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gxnjupdnk.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gnvpsokmu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gobjckonz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gejgyrqaj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gqgrbbigg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gmegqwykg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/giupjhlod.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gmwauacmk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/grnhofhdp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gyypbjaqc.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gnpisuxgp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gdoqwyptw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gimvfkzid.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gujeqmxzc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gibrgbsfp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/ghzxxnubr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gvyqbypub.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gjpazghcu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gkpnsaqlt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvlpcripv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gzretfzvq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gopruinck.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gbzotevnp.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/guzxrmhkt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gnivthtdl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gkxpfmmse.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gxbnlghbj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/goegxdiwe.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gmowtchin.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gapmvcxdh.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/guqeltuzk.sHtML


<!-- 参考信息 -->