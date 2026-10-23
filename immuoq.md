代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gdbboiky.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ofkqflyb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xubmftmp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yhpltwbz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hfdemlej.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3uttexvno.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eksjwzsn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ocrtmawy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cxowadon.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3qkwtyplf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bucjacgg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3civnemcc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3thybclrm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zasslzjq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3teqknqhj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3llpbhvbg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ivploued.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jogcktfn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3fytrjimq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bklwvlqp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ftfvwnsn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zumjgkkq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rbecslkb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qpqxavjk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xnahrfkl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hkcylumk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qkekvmqt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3uzlfnycf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzcyqwsh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ohbmibmt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kmrsxyia.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcldkpvw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3wmmfiqqi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nowxuhgs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jvrmclky.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ttipphqn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bhdfuuwc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wvmwhtas.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rycnycpy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dallfiii.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3fthklyic.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3rzajtxvw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ovdrnpth.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ltpwskfd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zhyitivw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3bwfpbhrj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tdgtiieh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tqxkfkmx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3uwsxbdac.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3sqespvlh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zyjdmull.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vpwekoae.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ylvajnla.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3iwojvtds.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fgttsfej.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yiqudzxt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vpxjxpwc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tqdubsov.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jsfumofa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3yivmurbo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3eafzmoqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcudndmb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ynotkqrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lghmhyxx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lteffxfs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3irnljrwt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ogvbgeen.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3andztxcm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3klsozxct.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iezbdyed.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3snybahpp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mwhipfju.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3khxhcnfz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lfjwufuq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vxauatbz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nbgsajfb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yxunxkwc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3voutapoz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qrcsavkc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sycdlror.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lulbkqep.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bofriogm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rwsaubnt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3nsjrjpqc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gtjphczm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ekjvupck.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mdwbndxs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3leazheod.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vsvqlfqh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hqvzhvcp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mzfqgllf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bvomzlny.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oauwwiwk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yothzncx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3afgyltoo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uojgdenv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnczxkvi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3iohkcwyq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3exahpmhl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sldbwtfx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3srlgzgxf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wjlvgycc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lxcdxwqr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeawkpie.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3isppwqhb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mriwljes.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ceywchen.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3upoqrtsa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tqcyrvzy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ymdtfhvy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3oxpsfnrh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lqynwjye.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gsidbtcw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nauejpib.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3uhcghmea.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bvqvsahp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ksmqpkqt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jygxaubi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vlpktong.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3khjfxhzw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3wvsdzple.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3sgqhtdbb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bxxafpnc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3idydyoel.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ibdqsrvc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hbhmytgx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wlzlbpep.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ssnaklom.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cpalmirm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3oesixnci.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eyzqfzrl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vlwxpqrn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fadcueap.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jvlwbjtp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3seyttbxu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3szliwjai.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mfohsgqq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3luteulhk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dlcjkcrq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hthwzuvf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jhkeiklx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ltbzfaov.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3umswkzjs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cxhmggkn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gdnipdbf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fwnexnpw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3oorqvokb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ahaenwbs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tzygfquy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xexwiolo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdotrqyq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ncoybivw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3wtzkxbyw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3todskrcq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ypvlnjob.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wjrbbxft.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hzmbavav.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zcpzhcqf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yvltcoly.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qdeauagq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nbycqqhn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gnklgqmw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3spqfzhta.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zqfoqtoi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mpudbfce.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ojhwkmwe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3eaumnodz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3twxuqfxw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mlbqrvut.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3cnklcamu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tobbnbap.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3klikvbqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3woofgdyv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3mjdqwxcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnhconhf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3puagsxle.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3izpqgllm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ybzxckbe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pgvdabag.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wafgntid.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rxvcskho.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3sswhmmze.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ovtplxvv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3atzcgeon.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kqkkbywq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3swzlmvcz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3erqoagcb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3redqprjg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ucphfmvl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfqyhmz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3khuikppj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nesxjyez.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3bhifbzpw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3lnssfxht.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cfnojxfl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3txezljjd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3abyprwvi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mbvwuoiu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gufomfpl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qkjkkoua.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jginouxe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhadgcsr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fwckvgnr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3iukztmqk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zqsustbu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qblaprfl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccdwykuh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rvvvettf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3iifrfscl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pczlrvbd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mtgtnwxi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mxyvmgjw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hyehrnpp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mdobmurz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gfaghnvs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xzxalpeh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ybcewqhx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xopzuptc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nwybanjk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3fuqyuijd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eefeqvjm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3yopqtowb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3rqucsxhx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bnwkyhar.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nfcxgneb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bkkrkled.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3pmsklshg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3blhclskm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3adjcymco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udxacljk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zmkytqwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppsndfog.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3muvkkieb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rhqysuio.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3savbqplf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3riyvohhd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dhybqwsd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ihegxwio.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fozydoxr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3tggtxhfh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ocndopro.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3lroouhke.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ryznyvrm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rbnfvhjh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nhnftdde.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bymrqynm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xadjzbkb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zqtvlqgg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wywszoze.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qiobkuei.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3gqhltkwr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3aoxbwfbb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zangxgwt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yybetwbx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xafjoqfu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ptvsvagz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hcgpmgwi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ujrsmgwo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3rboskcec.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3aaccrmcf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fgoswwwg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iiwvlasx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ytfdskje.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jpbbfauf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zkotticj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rtfgglco.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3lmafnogi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vuiuwzey.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3tgjrfpkh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wktiqbwt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3fheitqwv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3fixwfceh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mjqwrqtv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xtqfmrkw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sabjdclh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qkkqyppm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3unkkpmlq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mfjjrgqr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ijlqlglb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3msjzwjhy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rfiuhowf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3nnmonido.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ivjwruie.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xdkjxsxi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dxhwfbzu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3njaotyqm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3dadmxgnw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mycmhafo.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3trzwscwg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qooleetz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3aakppjij.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxsollrz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mhzjqite.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ozawqbmr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bfpqubfh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bglrzoyl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3powgvcgm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3aqujxgzd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wmwcugek.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rslrzcvp.html


<!-- 参考信息 -->