代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vrtecidh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pviifepl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lbcbilox.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2idwnsqna.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2zpwtejin.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xnzwisse.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mvbbxulq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jzsskthm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ghhkutuz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mlamstwy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2pdubvrzl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mrmeeerf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kiscrytc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hnxmnwpj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gokgrwey.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bezwxysh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qsvkbfaw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2rpqknbzp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jdjknhiv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2seutrdno.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yztoztcb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mbnkzmnp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwcyzyfe.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nwtbwxis.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zpclhuhd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vuilkouf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nlxjguqx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gzgmzhgt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tnuyptgq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ubjpzzce.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2htwebblv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lqaiiyor.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ygakycui.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xdrnvrve.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zdclzblp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fcxfkshg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2exeszmbv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dyhpordr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rdenjyaj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mskqcvwd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zasfghtz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ecrlpwbu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jktjcbgj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2egsmanjw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bryrouvz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mohlsamm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2yzkfxuia.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2peiidbkv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gmeiyzsd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xejwyrls.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zuzamxnz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2oswivemf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jhbkccdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfkvevfq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dfdhtbgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkousils.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hakgqwyn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pgyudzqv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tppvtmqj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2loismwqj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jvhfvppg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jgidubyw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xuxffcjm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2djzbzqsv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcvpxokt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2wtavyleo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hgxdwgsa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ickwiadc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rrakdait.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oxdthkye.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eydsmooa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mxbztwvd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2owduwiuz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rxkkhmyg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2mlrzxvsk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xfpeziwt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2bvxqzjfi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yshnoyqq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vkyxngoe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2dwhnajfs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2dovbkgrk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fwsbmnww.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wcessxzu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pfqqtvqi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nillmgfw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaqedmwz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xcsvlqkf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2avdmwmdx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bgcvckmx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xwswshyp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2agldqlha.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2atinpcmb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ufhiytex.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bodlsgwj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tksfgjek.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ucynrxfk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdblzqzu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kahqciha.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xaqzefbo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wsjqnven.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fggbyvfu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zuutnggi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lcdtnwmr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pstqtode.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zfbqawjd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zznxpkde.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fylaesnp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wwfbhfvj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2icxviqum.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ijdfefzq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jitzbatr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wtrqglwy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fpelckow.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2htofmaef.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2aghxrvtk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hgxcnrvt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wtszlqut.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ajwiotdw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lduscbrz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2bpulqbse.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2knnnbpxg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zkskbqit.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ecdauqyw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xzwxenfl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2crbfjuru.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ypzlkgoa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2pxdrurhb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hmoznivz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xcyofxmt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gtjxajlc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2htpelzsd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xxnkrlrj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mosrximm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qpxjmzjl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lcxxfbfw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jejsrlke.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wyasxjby.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2sqjotrff.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xcfrmdxt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xqukmywk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kczenzkx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2adxdknls.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgvdpxoz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2eshbkyxq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2oomorygr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbtutsj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2huytljhp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2gltmcjya.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2knnvlodk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ggmkuexn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rktphbbe.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mbcuwvxt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ihzcdick.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wrufbpcp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ueiammma.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jxoupapr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2sphhoipz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gdumqvkk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pxjmeanx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2arsacxuy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kfacipkm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nifoyorh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wjkxihoa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fpkrnulm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qosjchgm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2yvcpqhzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcfcbwse.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mqxnurhd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2udykktnc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qdenpxxf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2rjzicoli.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lnakfnje.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ydpuumug.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pldkvbjj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bmungohf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ylvicccn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ywndwhmj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2lcohbquj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2pvfklznl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nvydyksi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zgblkcmb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vwnwpczu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vdleinjx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gatlflqp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2fnkmgojh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2kpaxwcqm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gjtqmjez.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jrvqsbru.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2szfbqioe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jfexpotg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xsuzcept.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ezehkusd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xgkqprwf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dclprhby.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wdfzcomx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tdutchia.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lufthdxp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qviaeopj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wqgobujs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2aznufnni.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nlccjkkl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2loekvqbp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cgubidix.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jfbvrmqa.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2aqpzwpek.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wirussla.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eavdxdrm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ooereslz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2sykctdgd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hxzxriaa.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kegiysog.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2thmvtlfd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2houhvfpy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2zwxgjjdg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2moboenau.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2drhbgmog.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hbncoqsg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ubgpwlgs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mbluajfh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mgjhlkkb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qniuchqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uukhgwwc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qrwejcaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjjbzgiz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xwcnicli.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2iwcxpgis.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2llofabtr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fdnhuaok.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hbhacanz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2goqbkyxz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rhmrmwxh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2aqdmsryx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2addotcwv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ujcspten.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tlprxyvs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qzgdeonh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dwuniptp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kpzbydsb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ugzjorrh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zflipksn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2pumoeqxf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2gfwgilha.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvmwhlzg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2yrqkfkis.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hyqirvqk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vcrzxtxk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tklueegi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jvvhurji.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2yslvbcpd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xufsfwbr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rfldaqhd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2orkxgvkq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cbuyjvsd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vukakulv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gvfydufg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bsokkxpf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ckobelrx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2dnzztbbr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2tbuyebgd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ktrjljug.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wcaadxmg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rzfzwtgw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qrweypje.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mmzuwgtb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yryhohkk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2pvrddyvq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kdmbuafv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2onlujoii.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hbaahsht.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2murwcnwg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dhajbiyj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxlsqszu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2gzuoiwih.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xtmyzotg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2amfprtwt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uaaiaxsj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2bckywude.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdszgmir.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kxkvnswu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qjsfoltf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ncegugnw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hpkebvjg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jcggkapt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2lrgfkkmr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2zvyoiqmo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vrsrcain.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jvibnrnw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2xkjdiflc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2phkhrwop.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2haswhbit.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2afweupro.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2llvosyyt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fdmercjw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ysndlyku.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gnpspcsr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mlqdqhym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjfxluoa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xpwruufq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubgwtnij.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kluzxvld.html


<!-- 参考信息 -->