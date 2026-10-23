代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qkfbatex.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3uurqrrkf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wgbjqkcz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dsvasslh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3pwxogldp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cimdkdky.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tfxqhdan.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tzwegysi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wsnwppgz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3niymuxvf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3yrslxrik.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gzsjsfuc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hyimciss.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ldqhiexy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3szckvxuh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xqvkynqo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ysnmacja.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kznxbaos.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aawxbhdu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fotaesoq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3twdsboqj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3phnpmrni.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebdstlsj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyuhcojn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ucueyxbz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vnjsqtfk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ucjgscdu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3noxsileo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3clmbwcbs.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wbptrgbi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nkbjljiy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dgxoxhws.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ymnbmewj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qdaqgqug.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3asytvdut.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3nwbhfhzs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xxltbscn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wfktyavj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wtgxnbqo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hljpncag.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3juvzwldi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mqumybml.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3pihdoahv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3iacbtwhr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3cbcufzie.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ktnlkpto.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3xarbibck.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wvoewcjs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zlknscjg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xswstzur.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3caokvbas.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zeqltbug.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3itxzbinm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqswdpqs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3itlqrzum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owdwdvag.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ggrqlufa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxpsgchl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jhuatqfe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oqzgzona.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3unprnfpc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ncgwpqwp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kgekclti.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3nccubera.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dxidxrot.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3jemoozuw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nraapava.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hkltfekl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kdchcjef.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3frbbxggv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3piakfcfb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3aupfpoll.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3sioopbrh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hjdzcuga.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qaeuvbrr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kfjkmjdx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3mtrsatcx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xkrdzqmv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jqzlnhlu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vohwgeun.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ccqlxliy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zkbonaxr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3znwnlfud.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3thlfgbvt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iftsszgd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xqatmdfy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ckomlztk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rajgjtlk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3banhbvws.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zbggrdkb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwderxyx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tedfhiuo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xxssmpug.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lawexwro.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3diwsnfac.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xmmpsglb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhmymxic.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ifqhnsry.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ddaptogt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cggtvirj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ithgdduj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dlfwxzpo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tvanmein.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ewvbqdig.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gkvfpseu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3buwobufa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wbvdbsln.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vvevtzrh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3srfzdsjj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xgwlxhgz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gazqlfxn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hmuurrgg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pswbqteb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ogoijiuj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3sgzpebgt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3nimiopvs.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zlhqtklp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xrurvymu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3durgxauc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3jpljkktl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3veuqilhm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3pueneulc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3elrdosaf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nxfcdcrv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oyhjezos.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fnfazuca.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3awglfcwu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mcciqdrm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rvbghcve.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3opebqkhy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qnzdbkww.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pgczmskc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3oblfdrcz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wrkpefyo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kygboecd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jpmqogfz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3eiyykgxf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dfdrnzzg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3kdrvoidm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3exuonfoi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rtwbirxp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ufbdxemb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3tiungkkm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xzhylaqx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gmzbnwip.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjitxtvs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iprscauj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3clbvwvsy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xxcrlrgq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ifppjjvc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fimfwvcn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3chxfpshk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xbabnpiz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jifrully.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3llxjofno.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3uiipvein.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dxwrgyhj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pippxlma.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xvqcarjx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ibnueenw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hhpjecye.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3cuomqcyu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3fhnbmnfq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dxsrwdgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bogycgzk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zbjqwoth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbcarlyz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hoduzmng.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pskdaoum.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dhnpltmq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3vjfxfnnn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3utzeolxt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3nfrijfea.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3dduzuquj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jngeuchu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qqenwiad.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3yqqrumtt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hsfzpceh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3fhubzhlm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uiwbyele.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iipiyuox.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lelqbqaa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ncergcin.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3smawkjcu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hyzdwbbk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3banjpvcd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vuranzty.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jleprtgo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3rpezyllc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vbgkeiqf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wqnwplfo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3chgprsax.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3fmvlsjcf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqeqoazf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fomkrvsx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nucwrwhf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3emdjttsj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ywowljva.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkzfhggn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wbatjdqs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3djuiyrhh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3oivtackg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kqpmwibw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3efmmlhzc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hlghbcyj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lfpibppj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nwxhqdwf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ufxnyhlz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ntcjrudo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jakmhgmv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvuwcad.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rfmaswxo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3kdrqhrnu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3zpovvvav.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bbjwsszl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mniuqbif.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xqbnhvjd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nsphofcm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nyjjxfiq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hmvcqilq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3lnnfknll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuqjokqu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3mqtjpspj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ataivbvh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ehbazuuv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wjztyqid.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eydhwfdr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gaktyamw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pftgyisp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kwtjwmuu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3khsbxiti.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sdpiauxk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3llhdwekc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ftalxdih.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ptsnjuyn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tuoastkj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zgivgzah.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ygifyeyy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ecgjafov.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wxhshwmp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ssujwyns.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3gpkrwptd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3wblgdvoi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3bpvirbmc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3txwxusoa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3teapgvog.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lyxfhzzd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jjrgybym.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3tdsehqph.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3mhqwbwyp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mcrapmzq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3chuzopgu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3edukmbgn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3aaueuzgn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3axjhbhrw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3djcuuugs.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ijbhymib.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gnodbknv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3skfxvjct.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ltfbvfdi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ojothdyz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3lrrcxecf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pzqfjplo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3suenmgaw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vawkdhnx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mebmgswj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cptyctye.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xutlcene.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3msyytepq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vbaahzzw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3sagoetja.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxkclwml.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3hhuplxqp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flxivelo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vrttkccc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qndvrpkg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3gkvynpch.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmlpbnvj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jobcpqdv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hriedfbh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3swlvitve.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oxmtcwft.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wlyacbtk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuqxkeoh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3llqzkdcn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hovwdvti.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3dmmhxvrl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3owelwlwf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3janmmjru.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gbnjwxfk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wzksehvq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3iyhcvzye.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3akqukdmp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yjcrhcix.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3tdgxmbqm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ybvysnsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxaczdaa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3udejigml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbdbbfaw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3tukxymty.html


<!-- 参考信息 -->