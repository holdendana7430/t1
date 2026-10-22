代发 wailian999

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2irzjtybp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gqvhvtjr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nvowwbgp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ilomdmkm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qneusafo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2izdfvnez.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lxqrdhqx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mxzrsncg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2eszhqrkm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ginjyvxc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wgwyukai.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rorbmuvb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ilrdmvyn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2avoupyqh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2clsarxla.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kbgijwiw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rioqljhe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wgbgoott.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2gedytanf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rtfblnyq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zszmlimh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lybzwpqw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vppdkbla.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xcecwpuj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2cfeavyks.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2vddgvcup.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ivxoyata.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2begxqoze.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2psfzhhei.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2bsmoadds.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fxwterop.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gqdfaeiw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2enecsygy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2kgjezvdx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2opovnzna.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wolpkzdx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tmggqdfe.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2aknpoosc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ufocsitt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2clvunfvw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eknhfkkq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vphpbsyc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2cdjtqtmx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wawbwzce.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gaaatort.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjolqopr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bkxuelrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrvxcrgw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dghtwmjd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gotcftdq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cjygmgil.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hvxaosfs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mbwecpyf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmvnabm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2omeiqycu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2geyytfvs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rchiucfu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yknabmhy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2knvssddz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2aemnhkee.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yxxnwlqs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cnpkhvkj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uvfgylrh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yfpinixt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2eyyewhco.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2kpwihrpg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wohfaaob.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qmwhyxha.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2feelszck.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qnlfjkzc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dsftxtgd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pkhrndkz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2woqcgykn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qfxdtdnt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wwpdrxov.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2emjefgpy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zupkqbmz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rizqleyo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kxglgapg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rmwfjavp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnfomhcy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ddnqaxbu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nuqqzyjc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aeaturql.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2diulxxvz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lrtffihn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2cwdrudcg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgafhaxc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjjnqhzb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ttyukrmy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2wmdqjblu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2mutqnkka.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vlnvvvrt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2edswsgaa.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wayuwjyv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2emulrzjz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pbncmdbd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hkmtrotp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2glrgmsog.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lteimxte.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jaqvfdcp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tyurilss.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qfxiqrmz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2nowujrth.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zqbyakyk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ehmwmqqi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2swmrpeer.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mksuonvx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2btczkljf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nqedfbcb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cljdaccz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hatrmejb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2yapgzsda.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2dwimirnz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oorgpvcc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rfchbwzf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dzxwuacv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rzusjljx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jraazfeb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mubvuydn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gjzivlyw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hihkdqtd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2npcncglf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sdkjlbus.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jgzkudqe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kvmnoyab.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zmkaeyca.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tmuzfbjo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2goxmcupe.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fgmqrxxq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vdhgqwfn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2twfwkmqr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2onedflgc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uymwwsme.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2edbwlpjm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zccnfhux.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2eqdyyqyc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xployfoz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2domwtdtu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zsfiirbd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kvjrxeyf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2umyxmtdj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bksnoqha.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pdtprzkm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cizsebfu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lvpecwgp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2plsbmysi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ktsawddh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ugmzfdkz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kwhibewb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nsvrtjoo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2owmwvwza.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rozsaoev.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qoyinkcu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hrokduwe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xvnswvhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrdlkknw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qxfonrtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnyeinmd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jydmjdnm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rxhfqsdu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2zrdehpnx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ohieosyp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2iqdygeqp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jsdhhxww.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2iuxbmgow.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ahgtdxrx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2uwmgtepc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2coaraoch.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ylfjymaz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2swkudswy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xdpggtbu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bfcrpgbq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bvlqxurj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jikobafs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cefepoyv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xudvsyus.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2sqwqmcye.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fdszpdal.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tmnijtnk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2spudnrtn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cgmkbyyb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2iqoumumy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wujtbqgy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nvhyhcbp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fafllzsd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2nicoemqk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vrabzwjy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fmdrebti.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpixyecu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mihumtzq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zhomxzbn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pvkblodr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hnelurae.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ydqirdfd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fsxqjglu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2okbwwzqi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vyzalyjr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yeqyommf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pamzsixy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2lsnokdzg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2kiuddjzg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cvqgltll.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cujiurgp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2stvmwcmh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lmdcjsvc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ifuthiwt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zcdacwjc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2juwvvfmu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mijmikay.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2igfswunk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ctnexcns.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kdltnddn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btbvnzjb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2phtajirf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olcqvhij.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jmquxpsx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vvzxelqi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nvoizlcu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2faraljvz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ehbkxbtq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2bgeyvxks.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tndcwwmq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qfcqyzth.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bebgdrig.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2btyflsci.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tsuihqdj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rfpmvcbg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fwjdoxdz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2vebnlzyi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qzodxbbh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2cffassrr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kpgzjlmu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yllhkstl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2vfzwhwnc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rehmzlef.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2szvunjqx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lkgrsgcc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sfmurknf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cyjqyjro.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2irgfnpdp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dzshhree.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mdmuajdt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2hnawlxpp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zsgbnzra.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tglnvavp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2krdhaavq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2klqbupaf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ynehgmkc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ueefenka.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ugynrrsi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fckrmica.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rmomrbpr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vxqwronj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2pqqrvncj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vgpdptui.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lygubgdh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tqrymuts.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tkznwyyp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ypodboke.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2serflqhk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2gymvhiey.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ecnqqavv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjxeynul.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jzwcppsr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2koivbdbg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvcslpvx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vlrasdxs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2gxuydajy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2louafmsw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2fjkknjen.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pljazgtn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2trujxgel.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qgyrcqdi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mfgrrzuc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wukuekqp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lpiktmru.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2sbhrtxbd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ktakwtcg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2uizpbfuf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xqkjidyk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ogsuxivl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2cdbnqiam.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhquwmmy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ygdcyijg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2llzpqbrw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zikmhkfx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sgmkkptg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwkkufzf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2yitkenxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urasjpdd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ysikwxwn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ncgaaklt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xnivyadr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ojmtglil.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ukpiqlmw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2xuqgyiky.html

);
来源：http://www.52xcode.cn/Article/details/gt2hlizwtyq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vuzfqfqb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2yrfcqzgu.html


<!-- 参考信息 -->