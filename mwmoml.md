代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rfjhyzju.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2eqhlthqb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2esgrwgpj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hslqgccy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ydzegavq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xdorybdi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xbklzuqt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iggqurts.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2eeihrpjw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2pebykxnk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xfewzezr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2opqyifrr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jhvnfaog.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nzfnikgq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wymfpdtr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xvrxzkdh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cwjmezee.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fknlruid.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gtpvlfbw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ijmqbxvr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2evozvgsr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2heswnbaj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzpfbgxf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2exotufnm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wbjievps.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2srtpartg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqgqwhmx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2undrifbg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2duivizzz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vpamazah.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kpsvorjo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pfammbkn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2tvgxrhyl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jfoeitno.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2deltnnvq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qlxhgwcx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ggxaugnv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2duaeqlow.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nyslkdur.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2omtpjiwz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zstnndgq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rkkyyyfl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2caqnidcm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ykwenler.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hxwlarpo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2puopddav.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zoianrnt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2epswsknv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fheofigx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ywznpzqr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jyssmjjf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tnerpuph.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jigbkzxb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2yrittdhq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fzqbnpox.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2urchbqdn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pmujiisy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skgmufec.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dkdwxpzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fepyqezh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nluiaxww.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xhawmpdr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iivjiprl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rogxpbuc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ziawoktx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eduhwjnv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axehdepk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ycmbqrpt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ofhflamu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ubdiokyp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yuoydvbd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2amrvoznt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oeusojhq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2augainps.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2nkmigsvd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rkyeidah.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qifumphs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cgucrhim.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tvkyijoq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2neuhoqvn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2npnxjkyc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hgshesje.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vtxnezrf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2kdlrsjec.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zxuulscs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2tcmhkqbr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zcpshegt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kfjbebdl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wykgrwaz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ezlribyy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xlttztox.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jbsudplj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhmoftzh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rdzhemtq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikjrvvte.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vyrpoxyy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wlozlxtg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2sjhtogzd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhkvwnso.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2esqrjkhc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjvizdvg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cielljgj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2urtareda.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jisfnill.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2erfvzakh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2pdjwzjnw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tctvxrod.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wlizrvpw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cmspqzlg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gkqwqhcl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ftuoxmft.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ndonyhwy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yygcphgq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dhwfvura.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wtofgsbr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2izzfujtj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2nnykcxni.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bnembkuw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mzqnuexj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2iirvsfta.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2xhwzynql.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2aomooazu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nyyrclyp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qbqankpo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nlbhohxu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cfmqbmsv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rncgqyxz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2thnuxbvz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qgophsui.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rpivhdiy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yzxyuwwt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mbivrxis.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2unktuckd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2azauowxv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2egsghels.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dbblyvnj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ufwnziju.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cfgonpbm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uycsumpd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rjtidujq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wvzrapcj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2sccquxhk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2iohmmpsn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiimelhh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mnyyxxab.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2cmqxsnhl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ritheiyh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2tmtpkewq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ubcxspnd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fyohutwg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nekdtpuu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hhzubxrx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2aahennci.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nbgyzctb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2crpsddmx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rfxyapqq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qbjszjrg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2edxfdrhl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fxcrcbzg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2goosmtca.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xpvpageq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jkuccaub.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bbyfkbbw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qczvshmv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nqzzuvuj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rjafnfcl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2kmynpmqn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pghztwrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knxqkpao.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2oqxprnti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kddqknny.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2lxvqckmf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2faybuyvy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2kdytkjsr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zogezeau.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2iedbpfmd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2znfscdsv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2zmyrznbs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2tmnnspob.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xbbtempm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tnvxdrta.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mismpfcv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2smkpghjl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lvyacwpn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wbeznmqb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qkqdyqkb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2migypaty.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kyezetri.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bdmzwhqo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ywksufvu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ebqequkk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2rqevzczu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qumvlwlw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ntiqavmz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdmqjsln.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rgmoefop.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xiqzrbfe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnworrhg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2iovknhva.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2knmkipwi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2athuubdu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pdgcvqzt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xavnfhcs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ywwhxoqh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2eccicgra.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ngbqybvn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipimbvqv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2msyhtxyz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zqhsbkjq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kzwpulat.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xnxacdcz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jtxsbazx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hnofdcws.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2uzyvpqam.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ayaafjjz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqksiikm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2stnrtfoz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iqhhblyb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2svfchyjx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gvhpqtwd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tmitvdvh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2vbvinmma.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ihyktyyx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2igklkzxs.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2agdrvabq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmtcfbwa.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2urryfrlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twycihyl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qfuzkflh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2twhjsyzk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jalbvhcu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tlxsqgvg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yrbuljsx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2aibesezw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2chvjjqak.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kjrcyhns.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2baqjkyuz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2vdcyigun.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pijhlmjm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zaqsjprg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jcvhxfhv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2sozpvffc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qfdgixab.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2nufnhrdz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hydzobil.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fxuwhzxj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qthfdtlb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hnikypre.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2manotnew.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ncfodxsi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cmaiwyvs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vncdraqq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gyfzdogb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2qgntcpiu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2gtzbmwus.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2esiwkthy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2srmynhnk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hvbszuxu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vjrofheu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ujozwnhe.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gykmmfbg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2nihdbvuc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2xgljymfm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ekorsrnt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wsvrmnvi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ilwfzgok.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2iuiluujk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wedtpkwk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kpadyhvk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pexwszrh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2idykvrqw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2yekpziyl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2vxgwdcrb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ervrsean.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zffinutx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rapqityu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2zmdrjztz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2iltwcscm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vdjmvhnh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2lnisfkhi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ywwjosbo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rjboorrh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2apfgogcr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rktwjinv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2hmzqxpty.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vlbulzsh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hbzbrtnd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2cfuiergb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2utnfbdvm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qkoymnth.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mirckdfp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2dvaleezu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2odpceeid.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ardczeth.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2slcfmemp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hiiahvex.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2oruiuvkm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tlxpxsrc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2opjhdcpg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2szerkscg.html


<!-- 参考信息 -->