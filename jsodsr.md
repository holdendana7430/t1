代发 wailian999

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3imdyjaka.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dklddfpm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pmxtczdj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nggedudg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qrhqfoww.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3blvhnlzc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ckfadibg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ywwrpwar.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iemzgewl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3cdybjnoo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jzqxkbkk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wyaggwpl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kyilpank.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lrmtxtrf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wdrrfnoa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3auzthxhe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rypkliwd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lbzyximu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zhlyuznp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3cqesynqv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bgskgkrl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lpejbdco.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xmhczyti.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xtlfpzxi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bioodrfx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nozahmje.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jrggsesw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3umtiatxj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cftdmkyz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jeerbads.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lrxskyxn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3urkwekyc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3umulfawq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zltqxwoe.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nttxglry.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ixmxevfr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3udjegghb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vbvkarpv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3wkuataqv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3deqmcvjm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3seskkpbh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pnrlqniz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3houbczqp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qmjuwqdh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ywshhmzi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yxnodfoe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mbgcttkd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mmvicuoj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3skhkrcoj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3sippcyfx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qylzsdbi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wsusouja.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vkjviqyr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3avsksldg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3sztusrko.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3pjtuelup.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3iudoznya.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3cknrafyq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3uzvwfzvh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hxchsusl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zfwssemq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3cnllpvtw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wuqsrsce.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hiusjhju.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3heaydlug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihgsulyx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3pibyjgzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bafenzzg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3awcxpttg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vdisvtxw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3itozaaaw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tasjysyn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3prkgspcx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3envgrtoh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3atxvtzqx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3amtzdqdw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wsgytaui.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3aeyqrmyr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hcmxnchg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3rzpowkeq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xaiqnbly.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mtvrurhu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hlluxipe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gdbwzdzf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bnrwryuk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nxrtglgx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3tekhddjv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3tuieookx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3oeewxutv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ibvvhqcb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cllydnnw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vxujzjlf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yzntiotq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mqzvvukn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vlxdgigl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ydutcpyg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cibbxqsq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqvqecaa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qgmkttcl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ojlyquuj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwrxwtds.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hbxtukgy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ndlsvrrb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vjlnmucb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ljmlftbt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oaamqaww.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qfrecexf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3elgpdlbg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3extldoib.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3xfaeywna.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3svwsdtak.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ozqmwjhg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnaopzja.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qttrkddd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jbgtsqkf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3znljfzgq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ygytkhua.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3unzctnjy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3yqfjsjom.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3uncixocn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nuqqhwtf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gpzuuyay.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zsohtdks.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ohdxiuiw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3onmnrvzr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbppjfq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ugtcrqje.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3wcyulacn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nlqpgxea.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qewmazgs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3aahzawbq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gsektcxg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3myfzuvrr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ybcryest.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gdzlemlk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vqzzwsny.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dlriends.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qtbzuqro.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3fjwclece.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ounrnutp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3raxodctz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hokaouhq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3utlijlbi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bocjicwx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ceanthru.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xyytastv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ggscdmau.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3farulqnl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nivllukm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jomoutuu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qcvfakth.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzgfpmzl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3cjtmgiar.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dmnuzaky.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgxkhzps.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ysbmnbtc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3shwdoivt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qyihaeiu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3qsyxrngg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3apmnczbs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtrfrlra.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3aouqmgzm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dkhfzuem.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gucxbeku.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3izwcateg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3esugjmev.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xtsoephc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bpkjwbwg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zqrffeif.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rghaxvti.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lbjzfrdo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sojluxjq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zjaijsow.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mvfidqwk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qojjrpfy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3okfqhvqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rabupmyn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ixpzffqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fggfpjyx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bjvatfsr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wfhhwrnn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vfjkarns.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qgpoqotg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3smbkwidg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3szdjpjwd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hjpqvzts.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3racqnzky.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3myjerbly.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3stljdwnd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xavkrcnj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3uhkqwxen.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oeujudmi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rhzlobpp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xlkgmmle.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3obfmxonf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3bbpllyag.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3kfbhmrko.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rzeqirly.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tgviktlb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ypciuebt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yxasdper.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ecvtssjo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jlefwvwi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xobdjxbx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rsncpdcu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qlpfpttq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3oryfyztr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3gnnplpil.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xgcluixe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjercoir.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gnmljhqx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3fciftwnq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xvwewoqg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gvxfqdmu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vssraynv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3sexizikf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3atfwnjnd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qefeapoy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pyrueiqo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qcvvghrh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3uwezogse.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3mpkkkqse.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qqoejxyu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktjqgqhm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ycbekjui.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fefwgcdv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3zuudrgws.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3toyvbshe.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qtiterpq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yjqmxwfi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3cbtrowaa.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3rjevupvr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3whldtgyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zopsgxyv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdihzxmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whbkvmfb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hzgqdrzm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3titidsrl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cihexcdh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kajwiuds.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xfttunzk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xsvnaogx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zdqmmsvq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dhfqmtdb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vpdiplfe.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3dpjafwdy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3pgcaaaqe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bshhusqc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gsvwhyvv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3eqzzhpjw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3twenmdiz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vwcfezha.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wcogenhl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3fgeprwdj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3vqyoojxd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3iyrvpddz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tukiazuu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tshfpaxy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3okdpfrzm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ztkrhole.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3dlgoakbi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xylojeev.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wxhxdusv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3feyzxncb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qiapyxxf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zcgpghgr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hpvwsamc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oepnicxu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qcnucaan.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mdtsvzmy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3epkfbile.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qnnoaphp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jmfnftgq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ljuwynzg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ruxwnszi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3werlyjty.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zwfxczas.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gusfimhi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3beuwpjbb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3idkpqcan.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nyfsuepy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jiihspkh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ocrlobrl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsplpfkw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mrnzpyqu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3nmrvpsez.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qhvbzhsc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3deobsxia.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3htvitmih.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dndxrukg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ypnwgalf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fybfqpuh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3juzniuvu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hveatczs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uixbkfov.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejgiakfh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3qdponqzz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3cbbndaab.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3kztdoanq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kcbhwctv.html


<!-- 参考信息 -->