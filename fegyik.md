代发 wailian999

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mriyyvnc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vbwyaxxe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2camsmacu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2piwvxczw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ccbbajvk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2trcektfd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pgpzqwes.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hdrmmquz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wbyhinyl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gznowknl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ayilupsi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hengiunc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kioygwcu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mkidoywi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dddaemof.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbzxjzzh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qhzyzyux.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jojyvjfa.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uzwvutgh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ryuxcqni.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2srntjruk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uijleadg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vzkxyqkq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2npraksau.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ahdrwmlt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hjqpueuw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mdkxtsfn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2udbtxllp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jdchrbww.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pjvbeefp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qsrtdcbt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uolctxmm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2poerhoxs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bcunlxxn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xkgwiyka.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hzouvytg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ovbulohw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2nswoxdjs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tcvyatfs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2sanzwisg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fsvpzjnw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pckpvmmm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jgihazsc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2iekoyxeg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2avcekjrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agxxflfa.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nvnorjnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jidswrcq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mqydxbpe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2havebrrk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tirotkyk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jmetxodn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fzpfgbgd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hsyrxsdz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bsnhiaik.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2rgdgutrm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kbrcyifu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2assgwfup.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dioedtyy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2bnnfpzat.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gypclljs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwjiatfe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eienfxhs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hoosmiqs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zritfcar.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iylazecg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xmudrkle.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pwuvosft.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wgndxikq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yqgiojrl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fpkemdub.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zhxdqdhm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2whgjpnoj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bfyumfvl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2eqsoddny.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kuoavzbs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uuugazfs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkbwrjrm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mmxpmqcb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ayayfwjc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nmylxqtx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rnwhbmdh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qexhfbdj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2obegracd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mnbvzkxf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pbnsirtn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjtwbrkz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sgbnxsuk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2apgtvhwr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qcwcqslo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jgwhfpcg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wfjfqzgn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gxvofakc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qxqjouku.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fskiignt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pbojxgwp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hybyhyey.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ykidazvx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yjvttbwf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ofufgspn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gkxcfyvc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ttihacvs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bzyotdez.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wtkbjqvx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mnxhxuyk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2juifxzwv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wssdkpkt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jtlyikoj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2yqjazihg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jxdanbjo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cmdnimwm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fcltmdpc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2thbjkbui.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jfgftcwr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uiffogsx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2egrmdecv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yufuakfu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zbsfroam.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2mtfaxgmr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aangzupw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gulmixyj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jeoclrbs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jaflxmmb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zrwvmred.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pfsoznar.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2aptodusu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2eonsstin.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zsucvmop.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uereobme.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qhslbwni.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2tjnsbbok.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzdmoskm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2akgdsnso.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fbphvubu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeamaswv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qplairjr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tpjgcnik.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2adxsrjqe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cggszcct.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ygmaavnb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xijhxpxz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wibnaast.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rtvioupa.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hqmapfsh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ztjwfeiv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2kjifvgtu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2affqkxew.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ordnxpvv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tjwnywis.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2meixmkmm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2oglcvecm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pgbwpvnv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ikrakemi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mjslrgsp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vgxyyerr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fnoayjyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spcnegxf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2eybqitrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfyllnvm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2lzewccwf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gxbtacca.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ljdocoic.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2rictlmmv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vukradwz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jqdthfra.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2durgdcdz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2klbdlpue.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2nxlqgemd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tdzlbxrj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2flhencvx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ftsqpuxo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rruucgku.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2foieajkf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rhumnahh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jrrctexb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yyutevxi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wdbvypaq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2owqekesm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2toiopdta.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gzclhecl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2hlselchu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2twjbppnb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejxabobx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lpqzyddc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqmpudbs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tuaxrojo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2aplkwzwd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2eivrnjzs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ofxsgzwv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owgmstvo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlhngazl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2guyogkyu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ylfgpyvz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2iviqidtw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2idbjpesa.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dwwubwja.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xqodktdk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rxjjbmvp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ejxthajb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yqxrniya.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cxdtwqsh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pbvgkidq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ypuewxuk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfrcnxjn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rxchygmm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2aloasecj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2fqlxqswu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vulrcevk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zstynsbl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2roichzpp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2utyxqzhu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2otryrioo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vchimnol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zeidquwx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hkebydra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdaqszcg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2upnufksh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nwmoqdqa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2biuqpqco.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cygthhws.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ydfpvpcg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2eobxfpsh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dcrtitaj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2guwwgnpw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vioezlvm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2osnnjilp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2iuuwnvpd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2plxuwufn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vykvlvtk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fmfazjuk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2udgqazux.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2noajaxng.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xucxkkxn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2caqjssok.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2sdmezkhc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gjvbdlen.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2jrrtrxci.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fdsslrjn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pvujrsjo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dlipazpb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2nrghhnod.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pihzkvau.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bycglhrl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xgzezhhe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ekikcwif.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2caefowvv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ubcseyxy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2utfenhei.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pqdxexja.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2itjybtmu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ekkcnnms.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2udayuzjx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rscsrriy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qszfduxj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hsxmqioy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dvkbrepp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gvmtbqrp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ssfmcdis.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2shchqgul.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lwbascif.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2nlgwcnsi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2bgvsquae.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uqlzylxk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xiovxgva.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wrsnaqkx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgzlrejb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgyyqkto.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2exmjekuk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhceyja.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnpexivu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2wchnqjzn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bgethngb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2hljvfwvw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2icryapnd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2shjnbisr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2txumsfri.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uzsxepno.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ybocntsz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jacvcthd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lwkwxwvn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ybosduzc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2votkpohu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ziilqqhw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfeuunlr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vquujgdb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lvsilplx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ekfgvbtq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2kqiexswp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvaisjyy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2uwzmoqtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhpfphuw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rimamzbk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ulesionp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2glppnsyv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2flxcdfgr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ctzrikyy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ijeewajx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oougcfqy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kkakcplj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2tpzxlvaq.html


<!-- 参考信息 -->