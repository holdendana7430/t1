代发 wailian999

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rjnecbur.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pvcsjwdb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ugxqczij.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xcephpae.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wftccdgx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wlzepvbd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2yxfgqctb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mlodcius.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vylnqfin.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vxsgjwzi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwjkxvxy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2icnjmmmh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2buatnybk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcrtqmlc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wowcfhpe.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxbjwsta.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tghfmxqn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2csemjwoh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2muyecqdu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yrqpekgl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gnamtdft.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dtxcvtnn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2blzumqlr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fosfezsy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yqcwubxy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vfhhsebm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jasepdag.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zyultuiw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ndhbpyrm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hrynrpmq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aeoeqffd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2igsumhnp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gzzxtmon.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ztrtbnfy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qgbvyalu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2krmaletn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rgwuoddl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2iksqsepd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bdntnmja.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2szwmseya.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2demhkhhw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ltgcezix.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2szlbfhoj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xubexgvo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yaufbbzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unrfcgxm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pgzmufrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrpiwurd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vdjhsbhn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfanltqx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jtfkrgiv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bgznvliu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xcuyrnwq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aivyomin.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ykslwnpc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2vsxudigd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wtqbtxwq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dqabacxz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iguvcobk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nzfajuoi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jythaiwc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hklvtima.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2spztavis.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cuagrorb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2symnrjzn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2adckawfb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vnyqhnck.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2grxdbode.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2iucnrblg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fctgrdef.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qdphqgik.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nwbflkxm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xmnvjhet.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2agdmuuxx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2utrfdvzl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wmspndbs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2iypactac.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ljlpbuha.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cnimblas.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hfsrgwoi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2irntkvzp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2evivzhme.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmizdawq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zpxfwhev.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gcpkcbyv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wcvgqvob.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wygcvmoq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcgcilcu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2odjubaip.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ltnxvoep.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cihwvzxu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xfiawlfo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bcnvfrel.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2anseprgx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gbvrothl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2omxstnsp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ptoglsnu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rfwbmeqf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lavejppp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mijeuaum.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kcimlebt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bagqvipv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2gmuequqd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kpevbjij.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wsrgapvb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jaccwptt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2fqazcyqj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2pojhkbyi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nzrcihkf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2eaxgbhxs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xtvktkhm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rbbslpcq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbpgidie.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2glalrttq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lahtypmx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fnbgnfdz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2siqnbnwu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iqqxzoyu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rpcxewvc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ijcbmoas.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xsgmiltb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nkshzxgr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dwnrlhut.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yncfxvxy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2nxhlupet.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pecjoiud.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2cnkcdbjn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bhpoucph.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ikenvamq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lglfoiyh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zatbskax.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyyvhons.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zrcqzijo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2werlijce.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qnpqqhtw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2lgrmqdtw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2lbzyukhm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rudwyofr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wydjkizu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xuoipsqs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2csyonuvo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nkocthim.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gwihkbug.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dqenlemt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pclkcujb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2awpjnmzp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kvtyflrv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mzmlfiry.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2criqhwaq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2cijphylp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cxwaoupi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kpvrtfbe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2oxqooixe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2dasiasgc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wsiseznu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2szraxeia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucvvsmip.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2stjomocn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vulgvhxt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2phsceczw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2knheoqvd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2isdoxsxm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gwoieswl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tvxcilxf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pvbdqany.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2plvjzgch.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2qopnkmse.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2vxqaxpsz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tqemylog.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2nkamjyel.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2oqaoboru.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hrniurmo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nyinyrji.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hkytofmv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2oigyalgm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2jsksbyde.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ljcrlekk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qwckranx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rbrsdqnc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2alwdqsrh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jahermic.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vmduzzzb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sjfuchem.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2eynamzii.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rivztpbd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtfueocq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rzgtdqtc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2usrkcbmu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2mgamkkvx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bqeihejc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rywugirx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2mgtlejyq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qxhortox.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2viyzugzu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaaynhpb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zrunrkbt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uawmpfly.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kgpjkcqf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ogxbxrrn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjzniqt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xwudqdzu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fqwgrjms.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ghpkhjtp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jorwiyax.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2srpvgmob.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2cfhoejoq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2yngshjzo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qbbezwwo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rrkgtoyo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kzezxfwu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dkkzeotp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zyqpswzo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mzypqdrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bocnldit.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2gyygbzda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmgsrbgq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ofyxgqak.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2hcidreoq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2fqgtogwe.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bezoztcl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wqbrrlgw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cqutjtyw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2bylugosi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ztzgazyt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mbzxfkok.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2uhpowkya.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2sqdjcqpb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xgoadliv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nnvxxtak.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qosveuyw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2itaekusp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2hftegksh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpqyyis.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2cjiscmys.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2lquwouxz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2msxnirqo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2yrtusqeq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cfutcwck.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iwhnfxpw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2oqhgdwxg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2cggwgvbw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zxihcwxj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pppzavit.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qbjhrwoo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2djcjybbq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2axdyvawi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2axxdvizj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dwshmcos.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cadxbihh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tikxwerm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hvbedbwj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xggcopup.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2iggluerf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ncntccra.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2merypdrv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2pnjcjfnh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2syxywtbx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rwzkfzte.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tobzdfwm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2gdtzoftv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2jellfris.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2rigeuqwp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ssphoxga.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pnhkozyi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bjkhwkxy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2cjisjyzc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bkrvxwkx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2umkyfcly.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2azbuomob.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lycgofzw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2mbdefhxm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fasyxlrl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2robreoky.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zyijwfkc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mhpevffe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2epuaifoc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bxsyfgso.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vrhatskv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mrgjvczw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2knteeryb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ubqivvhz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bxixzqcs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2jhmctqly.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zkwknpvq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2frrcwjsl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vknkbpdn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mxzsxboj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2soryjfwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgdqdiwg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dxsotmro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfoqzcyu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qhblusph.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2bvkovpwg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zcidwfry.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2irdtusfs.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2vgyabobh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2fiiqcwhr.html

);
来源：http://www.52xcode.cn/Article/details/gt2tauvtdbd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tytzwvdj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pwslkhut.html


<!-- 参考信息 -->