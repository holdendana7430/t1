代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3azezdtrh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jrrqlaiq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3olcqbjqr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ttmzsots.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wtbrdhkd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zquprawp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3oxnlnozr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gcqknyuu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3uilosfok.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cbvfmcnu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3tdqbfdob.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gwbmeigz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3fmtcnjtd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gchpfgzo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ceiotywb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mpjetpuw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kpqxotbh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rweiqcbb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ukmwaiuk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dgcaepex.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dwjhjviz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3cpuxhzam.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqvxsfav.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bqojhect.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vfitefjd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pkilmfhh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhhfldy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukqsfpte.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3gdvfdhyl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3slpsvksl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vzmqhbzg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wdkpimih.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sqwkvabu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vwyxxcrz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fgsxerpb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3euoxqjfc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jqruadah.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3prmespjt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3etywwgug.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rzfhzucr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3mxnuouvd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wpmwenwr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ldfrcdql.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xveegxpa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rsgewoas.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hyjftqup.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3czjzuqpx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3udqqonbz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3pgdtzbkv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ifbkyezw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3aaayikne.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3eqgtjpxd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qokbrpvt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dfesdktd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mhacwdms.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qdlzzxfp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3oiivxrue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnmmpius.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ytgeavgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuzktctq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aomrasfr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zlzxufjh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zpkoysla.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vvblglxn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ahzwiwpe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tiftwykw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3blroixio.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3gftknkel.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvssqysr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zyvjyihb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wkilcptv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rvyxydvp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zsstiljj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3axookdpk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3htqammzi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcxdxjax.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3byfiwvcr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xwbulndi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hyxclkfv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gmrbutrz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3eaitpkdw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zgcmnshl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hvogwlkd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ebitmceh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gornfanx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3azdauipy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gziizjzs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3crigcmtr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmgbuii.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kfulvinw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kwskyisa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tjgowvhy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysfednan.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3vphjxmok.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3khcsjxre.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cxlkirbd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3cuomdsdl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wvsotrsp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wevonefo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nhenzdls.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uitzfrbk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zosfqfad.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dyshmgew.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jfuzbnhc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qoodboif.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3eyctvhsg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nggrxwxo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xvznamzf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wapaaarv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uqjtasgd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ctqznbmc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3euswaxsn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qwhyvjjq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vsgebtqb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3htpugkny.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yuunazro.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3joflnnwn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gbhrznvx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zjbenzxe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3djjkwfzi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vguczdxk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3mlquzcox.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bvojjief.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3npfdtbwd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bzpglxrp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qqmuxhmy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qpnwfomn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zoalcmpc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xyasorgp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3elorzitv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wrfnnddx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3leyzebdz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wcmvgjhv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3lkcfhpnq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3etyuzczy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yatiryzy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3irpbzgpq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kfihrwku.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3trixguxp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yjfeedzv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jacworpg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wezmecud.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fxjfiocn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mtvadfim.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3svmaeizr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hbhgqroh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tazvpuvs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gqutewcn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3vgecfjbz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmmgqzwy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mqvewhmi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wagttbnj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zodpyrun.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bpuhapka.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ualptdmn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ikperfzi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uszxbhgi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3okcrbpgp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uehuxqds.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3okndmjrr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kzcghmld.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3akfdnkhd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ofpkrqhw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3llivajog.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gkasizat.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nrsrnkym.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3zlqbsruc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gvnqgdgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaiviezv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3efadafwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xujjhbkv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zuyqonit.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mzzpdqkx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fkefcmsr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3avenggpt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mxbkjach.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jmrnlezi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3pyxludty.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jpxfjbgw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fdfxozna.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vgxzrbwt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fzrpqbth.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tbergbgy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rdgoufjt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ooprgbbd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qbdomrmc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yldmyhyb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xmrzacab.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gedhkqgz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vgsmzsla.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rjqwwcbe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fkxhchom.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ehjhywja.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3okhledco.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3emmprzrh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ayeaxkmx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3rrkxoxog.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bobqwelu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jopfvgmj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3sbbdaiha.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lzpuwckf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3azftvbmi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abzpmobo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gzhrvdcm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vgjudidp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3eybuvlqu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqbtjmpn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3yucmvajy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3almferlj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3syjgtmti.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lurjuktb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3unuuswri.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jibwxpne.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rvbwldsq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3melmjsuo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3oueadwfb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zvzrehia.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qevxabqe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3elomumut.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bxqtimds.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3txutcoto.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3erqukmct.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qhacjohs.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3djwrjkqm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3urfemcvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbanipun.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zgcvywuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlytqrlh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hexndyvj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3cgxubyhv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pbeuljfu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yqqmsodj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pdaimwoy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3raaytyej.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3itqjfyyi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wfjmupah.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rlwzztsi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3loojnctj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3mbklldmp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qccrqudx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3esuanuxf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dcehqaut.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bwchjrwc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3pgkddrcd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hziztjet.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hczhlkwc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3riiokbfp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3tdhmedgh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3guzqdizj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lnkzyhxx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rfztuppm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ovwtllfx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3czdoeprt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3fkaaaqez.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3zoattnrv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bsmnbfxp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3vkyipjsj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gvffrsmo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3avhsnzho.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3efeokvkd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qkxbqcfg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hcoutrhn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3cbewlxtj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fgcuegsd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mdffurok.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3yzsrsxxp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3wssraedl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ejvygsld.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3iemxrcvg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wscgfrsn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vzkjyqrf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qztbtabz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3uquyogrv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3naegdyrm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wcwzhyuy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvsdjsnb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3khygfuls.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctzmnajy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mxxlkjmr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3zztjieht.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3izcgfejx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3rswlvito.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3qunperhx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zgcbliij.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uvjesmzp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ntxmzgui.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kajmlemb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3okogxwjy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lwrfubup.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3iyahsxjp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fjmlcxdi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3egmxmnjo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3klqgoyxy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3syajjjtw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wzwzajtt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3osyqugyu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3krseuqje.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zueksixe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3odocwiyx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zvmvolsa.html


<!-- 参考信息 -->