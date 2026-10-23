代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3urelezvi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3uisceeav.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rieesecj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3enfxsuwl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3awhlxmqn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tkswnuad.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jbbuvanx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3sdewggnd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cuphrsvt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3caudrxvd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jvhuxthx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ygktggez.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ebkjnwng.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3fsxyzfim.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ngncmrpl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gvfusacs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zbwqrqqr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jcwyvwbd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iobwpira.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bidaeocv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ksnekgid.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tzabhqba.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mukvnjsw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iexfcrvk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eibeycxa.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3unjftkpw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3azoefopa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gasculwo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pakkiyro.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kvnsxxbb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3caxgignn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3thctzaqi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vreyjxap.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3symgaqlr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fmxgayuw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jogeyupj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gncptorx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wudmemab.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rjcjxlfq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xnatklft.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ekhrofzl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ghahtxpt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jiaadkzl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iuvqgdyx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ovktcikm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3kmetxyoa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zlsrwsym.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gpdtomdz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3tsxfojbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjqtrcea.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ypfzecff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snvylyoi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cwlbtlys.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3skrqdwet.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oerpzmjx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pzzyxsnh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tetsjgtf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpsqzbjl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxawxpbh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3nbvaxccz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnbhmqow.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3tfifldwr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gdvvfacb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qoouynil.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yyblvmyy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vielvama.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3awllbmft.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bwbofzzv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ripqqvyb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3skapviqx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zjehyylh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3arvfjviu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gtokahqw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bwudxgai.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hzutuptw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bvfdssqh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vuwbohss.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3osxslovh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mivpprbh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3zisifchy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3feajqbtf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tijxqyjf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3naxubscf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xqwupepy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gfskppzp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3iamyzepy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3brdfwinm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mmzldisc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lsmuhvtv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3iqhzyoaj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ujljbeei.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qggvepxg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fllgqnwy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3btbyprdu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qpoeoccd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cfqdzacc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rvpqyleb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bdbdjeef.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wsxgzteb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kenufcng.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3npcunaeq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3piloqdja.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3prpkyplg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kvkhqjwl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3upcooufv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3djlukmab.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3aorejqyl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mkuttdix.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dexusfhq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3eatucgul.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zrfmzbfl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wlxptibg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mnuzgxle.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pysfdidv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rmqdriiz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vkgxcqfe.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lypxszps.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cgalwbxu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aeowptaz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kamrzyqq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dbczhzdq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eaqnyqyi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gpkenjjm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qiriuadn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lotfoevv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dretvoyn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dgbdcdsw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3viliwcit.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3uhnmeryg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3etocnvip.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3skvxspfh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wybfwoxh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gojgpyln.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3tpclleom.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3immcbmno.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ymyoryzf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nggutuyl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hzbmjzik.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpfizioi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3aroifroa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3sjwhzyln.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3frrdecbl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eeijdyhs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yjzbxffa.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fidssiuk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zkwbtpoo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xdzsqxiw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fxjgagle.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3grcuyqai.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gbbwmfgg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3itwyidwd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3gqhgsvlm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wrrlewaf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3jgxglkyn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gxonkopf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wjsuqupt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3upfrnxkz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3atgabkhl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nhumrmjw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sfzmwbpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxnzvskq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nodexyev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yaarqvhu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3biaolpol.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3acaqnsff.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3olwmhoof.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mjmggcyx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mxypslzr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vfmbrxus.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3urialrjx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jkdzzmrp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ueihiptn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3krkniyrh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mgfayens.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3pceuxitv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3owzwwekq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gjgchgja.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3chfqsjom.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bbzltsns.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fdtgkqfu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3zycotgkf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3dyhxsmma.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bpnwfozo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3sljenaps.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3slzooyok.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ifticutx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpxkzszk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3giwwcqjw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hqcqtpfg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fiknqlur.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3aojuylhr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3odffiptj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3geruuajc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3stqjaaef.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3otqhhmso.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mdnkprhk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dgehgcxj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3pqkjejzk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuqzukvs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3umwrmyjn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3igtzykwo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xkmoclmd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lkqsjddh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3puewmkpa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3exajedlo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3kwqjfibd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ckowpwrq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3umukoian.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xfamobgd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3pzanggxl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ibhxbfde.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lunugmvx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ejzmkljq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3gzojcngq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nyttjquy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3dpvmavzg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3odnmvcld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uykyvilx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3duhpoorx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubbgeegl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3aygnxqmd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yhcxhywl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3chdzwslr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gtnzadob.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zxppjkvh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dbjbowoz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yjzqfqgi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vbdktgqv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mcxqzikx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jnzgydje.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zanwmhun.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rwmwcgaw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zohrfnfv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mgbqgvsk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ykunsuly.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wnijbjpu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3lhtlnyvb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wcffxpmn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jfvuhtyn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3drhfacjo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3casnekts.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mcwybqlm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ybejodxx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zdshoxpw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dxtwizhv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cjmhqwzy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3kggrnitp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lefqrsyl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3lvfiepjs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tfnatbkv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gbgdoqoc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3haealvkj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mgpeirna.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3njbxmktm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3iympdhqr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nztgjukq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xrrewgbw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tpvjlkus.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fhublsyx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3nywqojpr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3shbuyioe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ygeuocnb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqvzaaog.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qxrnkqwk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3oueyporx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wjguildi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3nnsbagde.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3eyrxafdi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3gddavwrj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3syampdnc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3erkxuhfo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovzvwcym.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3prwunpnq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tlbgzkpg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3nyspbtar.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ptbjyegf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3gzzujwgt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bzhjgprb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lclrbsgz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ikauduhp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xwwditel.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xkfnyuzq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ednepvhu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3hodrxxkd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3sputeihl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jedkelnm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3hzdtgmmp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vmphmccl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ypsmqttt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rwspwrsk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3lfjhujyo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3hlgmvsbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxcgnoly.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3umtubgaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oddloeer.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3gxxrcuua.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3oqdmutxt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3taqjelsw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3attttbtd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3szqonumy.html


<!-- 参考信息 -->