代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tgpvrxfk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3phhdjxxx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rkypzfoi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3tqpjxwxa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xzorimib.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xancvdnu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yoijhjpx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zoyhbxly.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3iwhmcmet.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qharnlas.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ernytitq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fkvwlfce.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ladjmpuo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3pmfklihn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kzbtuaja.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cazgoghr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jyvhqcof.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zczzuhsm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qvqwdqkq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3aemmkhfw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3srhacbhk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3fkjevpgh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mzorvqrp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xwlsrsqe.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sgtzchhr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxetihmo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3byrqqilm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yortttsn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ccnbqiqw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wqtcwhqt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jenilvyg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ghweroej.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vbgrmfwa.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3doaalxft.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ruyxpmho.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3eohmscch.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3okfjklgr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3yraasvcf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bmjjwztq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ezwoiity.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bkcyvlbx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3plnrfygq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bkzypnau.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fjxydrom.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fickwidz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gtrrtsct.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zxlyqpme.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdyyykh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jiiaqafy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ngklnuoq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gxjwkfmh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mvwmkaxc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pfzhdmag.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3loyjftoh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wpllfuna.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qtxjosxb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3hnujvxjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbgkbder.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3keeffhye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lztzbbmi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jxbuxeqe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ssyvrhil.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jkjxpscx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jcpzqtbr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rxgbshfm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yaufemgl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dkyjlgjy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nctjysnm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wfwpdojq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3egculgzn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gllvovdr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rpmjuyix.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kzvxbbyc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3odvfnnhf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3esmlbeah.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aigybhec.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bnfaqvvh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cntxxrlm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qkeyocwo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zpadrijn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mfxpsbks.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yxxxvhun.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3icfvylni.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ydexdjkx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hdaybfry.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cccltkuz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lmhuvrpn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bpykbyet.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wornvezp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkddcdpm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nrewybwc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3woccsmea.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wbbxibwc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3emrqcjgd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3psshppzc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qrhanjpb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3agmabzke.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qapgkxbq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3asafsdks.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lrjazobi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmkdiuxs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3reuiqaoq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nupxmqkd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfkmdnz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ygvodyou.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rhqqsnmx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3luejbgps.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lecjjfht.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uznrfdgm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kldyvynj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dcafaide.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3cppfzqvn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yjmxituy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qfirgals.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hzygxrfm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qyvblgsl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3gdmugmbb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3rxckrvep.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3toqwzrmq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xrvkrukf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dozfqkbg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ufngkibt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vkewfwus.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zlpsphoq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tpirdrgz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3rvsmneej.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fmunsokj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ylzdhdwa.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lpdzhwwg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rssotbfd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bywpwcvy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bldpvruh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gixqiwpd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3iuwdejrd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3usjajnnf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jjkwcflq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dbrfmfvu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qoobrssl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3koxqzsme.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cerfkgyd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mtfyflqh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yhfxpbdi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lylxgosg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ognatfmc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wmdjtdby.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qubymcpx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xfjrawpf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tqmgnalw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ygvnvhvn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtsrhtfq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lggzajzu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3mnkjmpwy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rryxqxbh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jhotjrhv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pcirrear.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hpibnsne.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zkgjvocr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3suhpwyqr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vvpvvdaj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kswooobm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3svkkaxyt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3teavfefx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zsuuolar.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kouisgjp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3exgaodtg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hpdxsxkg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3azwxnbuq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3csiklemz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nudmmrhn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gdlkjael.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xizxabqq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gyjzsnax.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3inertmdn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3smdokgek.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3eyitgint.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gsxihnvo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ozdscliw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3icjcqugg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ipayysah.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wvdonlts.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cubtuwmm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3iajfdmop.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3innsxmtg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3csshnsat.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hpmfnqmy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ukaousau.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vkcmdljo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kaqmwioq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xaxyijyu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ujbyjfzz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gigkvfip.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qgzlhbxl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gkocrzar.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zjtfuctn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gmtsnoid.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3oofpmfum.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lsoztvdw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ukulygnr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3seijlyjy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3dtwabjqd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nyksraoj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qzfpeyhy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bwmevscm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wxhkmhgj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3orglzarv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ruvahnso.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnfaycwa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pmlxarje.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uzopnayg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3uzvsjvlk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pgozzkwn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3emtotskk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rgaccnau.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3dwafwhhe.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ndwbbfmf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mybuqqbh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nfnxujrr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dgmimsaz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qljqgqpt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dohjgtuc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3anzhdxux.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3pcwzieus.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3uqrudwvr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tpulmxph.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dcmizaoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcfxbkql.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zfzbszok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekpstfec.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3apichfbj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bwkvgwqw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ioqtnnmr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yriynqos.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pqudyvne.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3irivdcqa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3gatrvuge.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3csxalhyf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jovjtdip.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3yjrksyqu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ehynycgm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3huzyulkv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3shyxaikf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3njslhfcm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ugykwhvu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ubirhnxp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3tfawjste.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nmwdndpu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zfdvtsyr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lqcnyvcm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fzlzrtnc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fmlwnkpa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3minhavsm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3zpdhvqkj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3modplbqy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3famvkvdy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3zwodoolc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qpnppszz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vuvqtqoe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gtfmvtep.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3isavaafm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3intmssrf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3quxvxrdp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dtgtpozf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hzvgvyxp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kljvwjqu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3sxnopguu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tnblncrn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wbijiyld.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ioptrpzw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3giwtsuqb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3efxbzyow.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hneweuex.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3mgntokdl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3gwrufoji.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vdlxzbdq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yhkxjtkq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxozgnru.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xeqcxmqk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3afbyifvc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3skejittq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nxkffpcx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3otdofdhh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyjtscvq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3fbntvlvu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hzgrjhwc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pdiydryi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bornbrij.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mdvpusve.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ukhoyqwi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3nyvzvvnk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hulkhqsx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3luplbhwd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3puyizusv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pcamaoxs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jlfpjvjd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3prydsiju.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3covlzagx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3eszmsbbg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nrjmxxhb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lqldkqux.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ttzepgrn.html


<!-- 参考信息 -->