代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ucnfkeei.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gsfgjhqn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2alhcrubb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kysfqjev.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wfhpdasw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ckmmpdjt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2oxxkwtrs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zmogrrpj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rwhmdynm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xhxglqal.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xwcxiuot.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yfiohzgp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2azajeyzg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dxyoxoem.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2thphkxpg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qzombsjh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bhxpqoeu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tmelziai.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtmbhefq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2abcykdvw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aycbddpf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpgnomj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uyatmekx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbymuntr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2nsapaung.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gflwqgek.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2delxemca.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cyuwwtqn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2roywyasi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tuogkfkj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pgqmstui.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2aevsikno.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2zdidhtzy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dbpnbqzp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ctxruqrx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dcyyslfo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ejqgbfgc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pkrrrdok.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ykrkzgud.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2oatpjgif.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2clajtvlf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bnvhhlfw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2itwubcwm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hzbdltvr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2sqoidjfq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mejttqvk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2vzeoflzw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dywuixhf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hsrqghzg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2prnbjkik.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ppajfpkc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cmpmhvdn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2stcqsgea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olglbozq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rmxznxwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqdimdfc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2tenqerhd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bcpcewnx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tjxedqid.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2amjumdwy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wuvqoegd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iayrlagi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2djwetxzr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2icclfswf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2praxnukz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2prkjkrhq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jscvnaao.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mqhhfnxw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mtgvesdy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2picqqvxw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cspjbzzp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vqnppuen.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qvjmdtzv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fgtqlvce.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cmyvvnfz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2kamxmzru.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vfurdyel.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kebqzext.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ocedogsh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wdvzokft.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dhrcjvqi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yztgcfie.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hgkzheay.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zoxlvdct.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wjonhyma.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wfxbrzmo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fadmtmns.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2inyojzuw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2icrfzuvy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2veezsmjp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uhygkhyj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ucbziakn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mftpysez.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmnknygb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hqgqacqr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kjbhoyae.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wnqwqucd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vnfqqujf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jyunavei.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wdzjrxjv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2avprrqgz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mcchbfun.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cfoexvly.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fqgjdndf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pqioprts.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2humspvto.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2izmcdumw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rtswtqqa.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sbgyxohj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2devwovic.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ncyvadkc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dwrxjcgm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2bxrikksg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yjpueyrq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qitihgvc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ydqulgdp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2alrzxxdo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2hsiicudz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pbsllson.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2uxwgxrnx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jeqatwmq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2igztledw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xhokvqmj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tinivvde.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zwxzfpyl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cxkgedok.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zxgklxup.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lbdlzhha.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fudgldck.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ayhkdpjw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rtzqqgqk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fjrwxswg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ufahwmgg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cpvdkeil.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ukljdeeu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pycpcwwy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qvxjauli.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zgiuetsb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wasifnyw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqznjacv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vzywnuup.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xzonrhdr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2eeumrhgs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2hdojnyph.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zaakcara.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjemnlgl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jvvlupml.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fxlorzjk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxdabqcs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ltlcwvco.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dlgpskin.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jpnkfdqj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ozwyyeus.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2cvztfolu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ujijngho.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xseisdgk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2suhygmah.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lflczvew.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rctnkinr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gqbvylga.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rjxwyjew.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2odlvcuwv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hwpeucfp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2msxhkphk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkdiueow.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lwfmjswk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxbouzhy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ptglekqi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uxmukhqp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2uwhbszga.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2bwhwvbpv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hfieudos.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nnsclhpk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qkuofnkj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vtxfkzan.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jwzucxph.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ifgvjmfq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fqxifngz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2tmzsomwk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wzatvbbb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nylqiwda.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hslxaiwp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2wwtlawrn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pgvuctoi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2stnjdhdy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ykguafwx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yovjsauk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ygmwttlp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mmufpllj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2otrhwrkp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmsfwoti.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2spbjmeew.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ribgmvdh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uijnifaf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pizmhptj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ukillejf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nvhboewi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pfgxwloj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kwlqlxkd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2cqibykpj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2uuxnlepy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2tbjqrlel.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qbdbgegy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zqgbxxad.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2buukmwpf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2mgfcfgir.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ctuiawsz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rjjigjiv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ytigiagi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qdxxzatl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkpsakv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mushofay.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vcihutyt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2syieodur.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vyrnilwd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zsukdxkb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mlcfthin.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wrwaxgim.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nobjgmkj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2wgsbjyep.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2oxkgyffx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvwfsbwc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ymfnwlll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2josuplej.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pbpvuefa.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cpwhlvkw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xvuybgtt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ytlhhcki.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cmskgkgd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xisgvoza.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fuodacfz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kbqisxiy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bachghhj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fofeqpwc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2bswhvzct.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2aiefqtgk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jipnoilc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2biiqhrqj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pechxozm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gfidjzpa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bpbmrgfw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2iflltvqy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dadhayep.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2iauskirl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2awjmuqaw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cywvoxvd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kncadrfl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rwoqdrid.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2qgefkcge.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ykudcxbj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ttdqjqkf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gsjaoxct.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2joxznuue.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ayyzjbgl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cdtgbinu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ndgsjmjn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2smrvbvaw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vaduhehm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fduteefl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2euyclzuq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2mrhebwuy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nmomaxag.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rilzbeke.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vgaizivb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2crtttnax.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2yrcaamzy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gaphjhrw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2saygjevl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2pchtorrn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2lchmugss.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qtmrqwct.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2huxfaozw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2akngbxyn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iguvvhnd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzwfyofs.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvaayxlk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2myypivuv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vvxnxzdr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2mwjbtsya.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mlvysric.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2dldhpedx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kjxbczuh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2walijtyp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crxywnbs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2eqfxefbb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nhuqenjs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bgehnsal.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2udafgblx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2iupwkczq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gkkgsrba.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bdrtillf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dflducbl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2uretowcy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2cmaxyymb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2xkmkjftc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ntvwgwga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwvrmvzp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2txkneyra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccixgylw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2yenzjohr.html


<!-- 参考信息 -->