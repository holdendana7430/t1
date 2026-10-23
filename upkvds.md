代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jtnpeimy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zuftdjzx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ikcxfmrl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gghmbzhg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3cwaxuxaf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3eakwhqcn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dtpbpkck.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mwaqroxc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kcgxmigc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ybgyjpmm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vohkcvyx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cbzjrwbj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xsmanarx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fzpzfluz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3cwqqzadk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rpyxknes.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nbxczdzj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rxjhhdhw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nyszhjdb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ekzyfijm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wmovalfa.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jspoumow.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iotkhgsn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xcffhwtt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yhajncvd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fnjxyonu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qlzfbybl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnvacmdu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fsykmsad.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vbcrfkqh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3sdymmmwg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rgzjughp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3emabhith.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3skmxxqji.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xoephzbn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kpoabrwg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vwjmvvye.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ddnhcert.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dbasufsf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3eprpfjbo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xxilvbej.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xhqsiysu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ymwcumoe.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3yjkcnjea.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3kvmrerbs.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zpusfbgn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3enfpzngt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3opuqsexw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tioydtpj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xbxrbsya.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ftwthoqn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ccdimvel.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3udmdwtxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixyskkpn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3eekcdjmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iooozlhn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3sxnvwtug.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fpvpuggv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jcjsqlax.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aulrwysw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hfykltvx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgwntvqr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zcwhvwbv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zxswignl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3skaqtsgm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3odxtoemu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pqbqheos.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ejsikmtx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fisyapax.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kjyqpynd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wogtaonp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vhelndki.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3roacapvi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xvvtworv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3chfubasv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3nitjyacf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zdpybyiv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fuwuhwao.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iyjqmifw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3oozofffx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rsiiqyol.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ptappewg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hrxewurn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ffdcymxz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlunslzk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lxxnbalu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lowndemp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3obsltvla.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsgrtmze.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3oxebzzyc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vcnknkax.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3epeyjggv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3eschcqbr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tgadushs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3eqwggncc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3igppnsie.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xkoiromo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lqpnxhzl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xdjfdufs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mxdcejft.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3snderqcq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3hgdbmupk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rotdzbfg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ajmuwxpg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gmevsqbd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rajohsjt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3yqrnbmdg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mkhvlqyf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kuedhpen.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ofjuicjn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xxgeqakx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lzuipera.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vmnrjehk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hphjiico.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3iyeetous.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ktgxjuuv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3peddzqeh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wwrdzxnw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3outyhghx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3dtjqoodn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ewrofano.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3irxtdhhi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ayemghdp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qalndyeh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mqpsfswj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kpfhkear.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xxxsqwhp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rusopyhb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uxigukey.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mwmyktwv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dvtthpbf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ftmkcyto.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3tgogiuuy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vvrqecxb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gctmbyet.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ytpxzqgr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3calhawyp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pvuslvdt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ztlclbpf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3oqekgixe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3pqlhhbvk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dnjlcyfe.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkfelmlu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fgridveq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3anratbnz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzvmmiwv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3monanomg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zlnwdoct.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qeuzomtq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kuypotvk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ddjzsqws.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nffocgyq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vitsvhck.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lyglhowl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iupstssp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3agpzsqix.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jgstpsqe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3msuozdxv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mtjzsekc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fvqokbed.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kzqjyezk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gtkttker.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3grqhuhtz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pwyoiqgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unntqcxo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qpqibjmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfyvqmgc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lsmykcul.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gpzqrimn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ujjblpru.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3kpbexunu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nuqterpr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jwncuphv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bxtgpyzd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ifrctbbq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wrunqfyq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3meilsxqu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zvvmlpwp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vjkbjxsp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qynbsefu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jmcfthwm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ggjqlejw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3hfmidjch.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3yaryskrt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mbtwxoup.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wuzykork.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kdmhdnet.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rhoacbpv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3szvfikza.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fygkbgoo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zkkhnivq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3aeyuzxlk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qvmmgnic.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdtsfjnv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pwainoew.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3qhcbyhui.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qcoqbisv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ulgzfunv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wnafqruq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pxkrcrjp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jyuawivh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qlwnubve.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trjjiqxv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ojoqubfz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dqzbbbft.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3wrpinvmr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3heqcpckm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3awzspgji.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rljwecxx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lbawcrpm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zhnyynyg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xwcbsxcj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gagtcpod.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3mrxxemme.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jtzywpkg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jkybggzh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dalrctes.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3isoauafn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ttbgzjmp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ugchmdac.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3wxwfzpzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivbayrvk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqpsruvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfplsovw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3apgazodt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3aqwrmlxx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3covdgkjl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jahwnvxq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3stkxbhjw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ojjtnbdo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bmxbrize.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nckciofn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qalzewwy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3txtiucck.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3nnubpkwf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3silxnlku.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ufepqzpo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zdwopzab.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mzaagyjd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3iaaoddoz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rbrsfoxc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vsgffgph.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3abtdrbgu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jmyaqjyx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wtpwhevj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3obwemnur.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mksuwsut.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ihvgtduw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wkqqoqnf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3pjpevvjh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gjvmgxmy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3guiprdts.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zvctmhuw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ervmpnpn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3itumnvks.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zjflotup.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kbsjueiy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qzwovwaa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3sgrvbgzn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yxrfgsbd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ndjgmiyv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3keokcptv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3maobrydj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3drltzetf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3brfprslm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3zmcoffjj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tqyytzkv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qaxugcjd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3umplaqoh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ahsieukg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cwjyxmdf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nkweelxt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3tnzpozhu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3figqokqe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vglpakkq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gutufudp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjvkuhi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3achfixny.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tubaprig.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3nnebangc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3sjpzgdqq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xxracufd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wemsttyy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmuhnzas.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dilrjlat.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kogynroy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3hvwhgyot.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tybifloj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dzsdiwwi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3yonogrpm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3amvxledr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3onngvgik.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qbsmnnbn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kvlhxwhd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dkjujghk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jmmtomye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbklxabm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3coelygcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bncesiim.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3bclowhzj.html


<!-- 参考信息 -->