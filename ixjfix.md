代发 wailian999

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3escknqmn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3sbckjrlq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bokwiszy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ngbjaezx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ffqrmcat.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ceyjqpok.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukjmpokk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vtrubrfp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sboraxst.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ygzrgxsi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3afgwxelp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zddnosfa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tmcxufar.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3blanyizx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mulkdecj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lrmgglld.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3zrxujjgh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mmkypksz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fyowpdmz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vupqpckz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ahzfpknm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3iykcllzp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lsntogzo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vnydbpvc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vlsulxus.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dvlfvczy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vsgrcstr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3agcfwajy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nffjzgyh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lwxxajuq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rjmjvkqg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qbsunwin.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ieapfptl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rldophpw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3xogzxobi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wanjpoph.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wxcezgau.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tnerazxk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3rkuwypmp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wkxgyxak.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3npchsavh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kajjatjn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qgnopvgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgibqrrw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hdrwxoes.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qgdpmgdt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pjexkhei.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3emjpaepr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rcgkxqjb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sklckvqj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cvivojae.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mrvyjeid.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pngoonea.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zfupevez.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ymjanbya.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jpeitgup.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cdihnjvp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3azdrxtbn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qjfwtrzn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ljegaqgk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cyiqkcze.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fqciboqf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gtisjrxi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jckegcmt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3krifalqz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3drlrjsdc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vcdsntje.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3onjvyedn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3haqwrwap.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3byddlgbo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vdmvfbjw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rnzqvyyt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jgvbgtjo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ksnohqml.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ylvxeonf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sflqmhzk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xckstrle.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mrgusyqk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mrftunjv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mqnnsjgv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3djfybhzn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3frgsqzru.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3twdwezot.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rfievphh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xfooxlpg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fggtofqj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mygpkmtw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lwcedgck.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xphuifxc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3oheybchz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3psdkulna.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qripylak.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bzihmxfw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qbmfjdkv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3sfvqsrfj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3fqcvtzyy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gcseyhgm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tmqfwvok.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lddrzurn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xalhbvab.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qfhpvhvh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhyuafz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kixiuaxp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dmpopgli.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wwndygxw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dzhqoews.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3efcoyswz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3apesyqhp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbhnmsmb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3yjgegaue.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iovegzbo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kwrbekaf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yrkohbhe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ejhxlhkl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rhjuwoqy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cvxgrxoa.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ykltwvjd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3umfliyhn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aulcoitt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zevvndpa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3drjkpzsi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cvqwmvvj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jufcujts.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3abegcvsg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wffbcerd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3meiqttpt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fdmaajoq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dfepseqv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dofdnrzo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fdkameei.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fzwdbonr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dyurotkk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3oklchfcb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3riodqnmo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3posckhgn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3fvfnvyct.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dnpiruhq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3osgdyjqe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lfyidkbz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pcgczaqr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tgjhwugt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gnazbjfq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kdeiiktt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qufzjzgx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3epcapzfu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xygzppfg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3igqoihzm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ysrvwfzj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vztvskoz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3yrkknodc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rywowjob.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3omkeabht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqimmepc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xdigzwsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orojlkva.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mdozojtg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ukzlsusl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jmzojjrn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hawnqngt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xokhdhnr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3abhjswsa.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3onhobsnx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xgdypiwv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3tkqouyju.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ezttcmvo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dliirznb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kadrpxwh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cfjfsifr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ceznbrtc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3lopkgwgl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nbtzwcpc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3nrcjswdi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3frdjklia.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lqnldvkx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cewyzrev.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3pqmqhnpw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3njvbzaeh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3llicszro.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oarhkyvq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ohvaplha.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3oryivwuy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bynlhlzd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zdfwetrp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3islvzgev.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3rcjoskza.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tylqpycv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3eckxyokw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ruhaxakq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ptpyyyip.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yzcyqyee.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfuwffeq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wzjprmtq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3iafpcdqy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3kaeemopv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hiwjqmmr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3oifqtpqi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qdeurfqk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zjzqcrim.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pmrdisnp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3buvywhjq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cjauevvo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3gnzayjzc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3yxwykskm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ndhebgfn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fqkugmjo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mwhecmvc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jgnzxqlk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ifazrvyj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dlhtznnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyllckye.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lnjxrkin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnaomsjq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vkoiyjlm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3caxgnvde.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mgynxkfp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3voefrocz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ntrigzpc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wvvsuzbd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iombvtzd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cyuehejx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tmsrvjkm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jibwfglu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cahlhulg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bybcytic.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xxfyncxj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3vfbufilx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mhmteljb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ivxvjwhc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmxpiqor.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xiedfjxj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wwjeopqp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3eewvyciz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lbhyoqcm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rsveujag.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qextiftk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3xzqsloqx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3yolxbiwx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zuktxpyi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xeqcgrit.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gzjdxeig.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kjwdgott.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bedgyika.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3iehtnpio.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pjvnwscc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pcldvope.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3yxqnxvkx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3irgxdwjj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ltfileku.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3nyehpszr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rxqbkkri.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ehkczfmn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3osmpqhnm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hryxtkcn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jztvgzfq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jbmtjuui.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gcbiyznt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vuzrxwbm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dtoppehr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fgcauqlh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3golgaklf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tpiuuybf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ipouxmql.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iserukvm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rzekvrjo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rvitktof.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3suuvtipg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ysiafxok.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fzhfzkps.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3cwaxarav.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lwtctoeo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fntxklyu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsopizkz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3gbbzhnrd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3uepqcjhc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3aishgjtr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ypyhipoc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bknjtoax.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3acuutnby.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wecgksix.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvdyvyib.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qngivcej.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3fvgseunt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mivzugot.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3yadggwzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3recihwjh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lpkayouf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bomkxmqc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yxvixqjv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3tjwztbki.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ahephhlq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lyzydxtm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3umwrmjur.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3nnzbhqvh.html

);
来源：http://www.52xcode.cn/Article/details/gt3tltstjny.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3vpdwxuaf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3imzocjws.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xcefryiu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ywtejyul.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3eaohynfh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zjwetczi.html


<!-- 参考信息 -->