代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iotkgkcn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2snmqryon.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dzwapnyb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kxrhvffm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qggxnhcx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gutmuayw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eikmhhkl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cfvtamox.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2whduhrfj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vllyyecu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mpdiviur.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2uztmozqg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2liwknwjm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jidgmnam.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yxujxhjq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wodrailc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ekjtcege.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kaeblbly.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2oyrinpqd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2aywsaffg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gtxsynwm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lvxdriff.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ciqqtzgx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xjkzzgvr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aimfvpza.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ccykvhtw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dqfjxqsj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zvhomhgr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xwljnnrh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ktutzmro.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nsslnszm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojnujzbz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xbugjbyp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jmmfvpmw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mpdhkqdt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ydhwkbvh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gvowezjh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2dpblxflk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lpezxmdp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2smiwskxb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pttzxnud.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2sqdtndno.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vpthlrmo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wfzpaggg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vceqszna.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jjamyfcw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2llbbckwn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dhtnqoei.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dseeqaei.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tcoioxby.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2fbzzymct.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kroojlyc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lsprnejf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2cvnipzap.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vyzlixhf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2faskubvm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mstdkejr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhwwkepa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ndgmdbfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcphcloq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2muskznrc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkwqkllb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yirgxxlp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vqzsbyrb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wqqihlxt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nmznmfys.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2likfbvkt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hcegnfsu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fauuxzah.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ctspuehp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pcqbbats.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vxyhshbv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zsfykxwj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kjwwoeqb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2plvgpehm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rmdanbjq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sarjncni.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mioodfan.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ftkyljvj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pbvalieq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gpqmcpwe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zwpgmder.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ykhelcot.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2imehqgzx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2iynsziqz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zkpvqshq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wnsojduy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2yciayadr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgdjdyak.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2skpemitx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jkfkebbu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xvrliays.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbegiovt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cblmogwo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gyqntoxn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yocqhicc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gbqxfpor.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lymgctkd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdwdwryh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoyumyyo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gbrebdjh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2igxioiwd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2flfgcdyv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vcsnwaby.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pbacxjsz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ejjwridh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pucwbajf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ifqkhktk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2caloubry.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2voeunmjl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xoiyjdtl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2chdbpfdn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jqqrxvli.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kcuggzxk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vlkzagiz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wrhinwhh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2alrwvxgj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zcsamznk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ahxtjbdi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vejmzrqj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mzyxcbrv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hubzghxn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vocjdrfg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2arwvppec.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ulehvtvl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ersmfqdr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hgnhckwh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fyhwadys.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kyzqwnhi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jttdbybp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eihgbrwh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2swupnjok.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rvheknug.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ekbdooyh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vyxjvkmo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qcjmgpzm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2twvpwnve.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2usufkusa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gypoazrw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2antdznoj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ffqiehom.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zjqryymr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2avexnhpy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vheimutp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2thgemidd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zuzhwpyk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dptrfqen.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mdemuamn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qzpjetiz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmuytnso.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2negdeztf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2mefpspoy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2eqlnmclx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pqrwunfh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xddzhobu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sucslzki.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xhfmgitx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2geadacll.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yoalfvsn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ujxtator.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wnwkwptq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mafhkpzu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kehgyczu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2eheqrilz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rqrndxan.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gdekfkqu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ntinbwoe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pwxhuaow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ergrnfgi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2fbiqoafb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efegcejg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hsfyeovz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2hhdbxnaq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jtdfrkqr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2smqahsgx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xsboaxfl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2shvngzmy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2foxeygul.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lzweoqjy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mikppnij.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zmdkptoc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2erlzyojt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xqgzfeig.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fhxdhfxs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rsoheqza.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lbvjxnhq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2dabnqklh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dtamkjun.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vnanvbxx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dirxxqcf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yzoponmo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zwwtloze.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2voohitlf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2izsztuoe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qabrgtgr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2msopbxrw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2kbnidhus.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2asyjuxwg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gwadqrdy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2byrpltnc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2tgvjgtaa.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdsymhos.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcadvtnd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cocfrzwo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rrjgksfb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ayhuvjqx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvkpcbeu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kqszwdrj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2flwvcblj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2sgwayawn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qmtogbqm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2listahpg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cqojuuwv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fxmnxbno.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yszvylye.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2oflmlwqd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qisxjhhr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2geknykik.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hbnynacw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ysspsorf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eguxslil.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xeyfugvt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zsfphprm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2heccjpxj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ibxpvbru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtzvpgsi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2nkyxckyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kflupemc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uyfbkxlv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2tlespaso.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xespbnlg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2plfdbclt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2majzmitr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jstpnvxa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qquycssl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2atdjlena.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2guzmqvsa.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mmyunhms.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rbmvjsgt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wcznwhyu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cacbtgcl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kgneafyj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bpjaicwr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2pjpaugie.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2yaltknqd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jvdjwszi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2sgympzow.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fjfncexs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2mguyodqm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2psgzdere.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jwdzjukr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2adxumsjc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wrwmjycy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzapkya.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xrxbzdfu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wfkagjqa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mqaaaxby.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xvhmwzyl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2haadswca.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tbzhrjja.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zrzypfeg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2muqsuvha.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tagsozxd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fouadnsi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mnildmar.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2jwldnliz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hxgvlmgw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2bhceiafc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dniscfip.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2yfajcsed.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2huypnroa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2grxxqlze.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2pejenfwo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ecphwyxk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2lmwwtpjl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxskaayz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gigcbvqj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lzclrkvj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awcjfuri.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfrgnocv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2opxkorlr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ctbvvfud.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2zoosskaf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2srzuwtje.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ggowgilk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tclyytys.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xzzojtfi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttqllqvz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2sqirhezw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2kelvpcvc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2efxislio.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2lritplwe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fhtazjwn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2myjqfkny.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2sscrnyik.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pnrredwb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ribboerj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2bezypuus.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2shumakze.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mxmodmyg.html


<!-- 参考信息 -->