代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ijrcjscu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zxcajbna.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lgvgccza.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dnefkfbz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3szaczgjf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ycoecwer.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ipivtjpp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3viyjhcrg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3nbcdckkx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mxeqcsmu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3niemrjoz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mbfmsnpb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xqhbgjfm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nhcjuhvn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rnatbrji.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3llcxgeef.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bdumojme.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3imtixquq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qxfexnlx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hzstmurj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wqxbfwhj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ydvycifc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3inroxulb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3waowxxqd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jbbpdkdf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qrdnzbuy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zqeryrbq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qlvdgzyj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3workgxjp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ghvtvmxv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jemdojqm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ctbfujdn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhplhwut.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3jijtngkx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3miomxfrm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sbvvcqgz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3komcwthb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3prgfeijn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lnidlmix.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fbbvpwzh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ftgwmtrp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3phvsalcs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lbpbjwan.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ldsknexu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3udsypwwx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lxitwnil.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3geqpjrmp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3osfplakp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tjcgfkrt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kndefydc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wbcgwgzo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uprcqmzm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3klrhpehz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kppyhrrl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3qjfonymz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zuezisaj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wfhpxqcm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ysfhatzr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mxlzlwgr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ryqewprl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3kpaqoldx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imicupzz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3jdwglqtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htlgjagv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lfxopjpd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yquxyqru.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kleudwbc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qwevzsgx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rgsayaro.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxcqdeod.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hhybfbzy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3lhmypyga.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qiwrpbtw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bdyyqset.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gocyxrbs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jxngzvgk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ydftevku.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3autszook.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mbzrjssu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dhpghexe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vgzpfhau.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fwwdequo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mdylatba.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3stflqjmr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3zmuonapt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nxbhtizv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3adzmyevg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gqbcnbee.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3tzkrqpbp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rihsrfgi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ffszhwug.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ozxvcefn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3avmwbver.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sjlmmzva.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clblnekx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cdeepgqj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvsduoij.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zbixcyjs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3irlofnhk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3suwfobrv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zzsfthhk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fieflhhq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3peimacgy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zinlrdax.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wunrzgdg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3akyoaxee.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zaknetnf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zwlloouy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3pgbcifgf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tmzdpmke.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3opkdxjyh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wyvhplsa.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yxrwewvl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iaheeows.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mvexejxi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3yweskjmm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hrefeqbc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dzxvwmfk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qktvukle.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vogxydnl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3yltwrxwf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qsabpaab.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cyygchyf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zfpxtwdu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jjybdvnz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lrnptfob.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hefrdxlm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3brhnzrib.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fshiinvr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3azegkgjz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nhbhmjta.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dabgxdkd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jmepepvz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mbryoybc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vqvbjtwy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rnalxiib.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bnwwakbv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qbzuhgku.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gogsujer.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kvbbnywq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jyuwuoab.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tfhnoond.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3pxcgcmnx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wtmycltv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ufaeovxx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vmjnwrbj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ngdiqlyp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3pixhscxo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rmhynfse.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wgwbmpbp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xkwmebjy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bdzwvnca.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3iuaujigf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vblxaivy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xttlqhou.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3eeqrozux.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kmhjygoi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kezqfqqw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jeqpmziw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3owrhqkrs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3smygqxyi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vtusypmb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nrbtbqep.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qnoieijm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3lwpaghgq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3oaoldsvj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kynezfdu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jooytesn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jscokmva.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xlbtlzrm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wdqkikek.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gkdaueac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glxmmpmj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3veepxthg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjchfgfb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jpbtjzdj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fsvvqskq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vgqfuwma.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hqbbhwiq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wntoqgwg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tcfnrpsg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jzeudjpr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3aoppglfz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3tvsyvyhe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3blocihxg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3psewxybt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3lhxmqfop.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dzzhrmss.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rtxsjsdw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vrqlivio.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bbafywcw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3dzvyeroo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3yfeppray.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3esmowmts.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jdeabhsl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lbowvape.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3aznycsmi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3btigvcuv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyvgupoq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vboxmfgy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ocixyfek.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqvdpgxp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lzvrohrd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3tcqfckhu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kciukfug.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xdetnqic.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nqgdckry.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3awenbkti.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3icelnelb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3lmqgnnln.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3icclhvnd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3tqsyodfj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oishjfts.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3cwcyqngs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3khhhfdwg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zispiwuf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3tegfipam.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zrkzyivh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3exqyvzpx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3eqsvrcuy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3miaggkmj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qqbjtjhi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xqfsferb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jknkplqm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qqoipiju.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gsqqipix.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3otjbklin.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3subdyzjr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ccnhzhcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogxfdvxd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3wrbcvdef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sndhfotp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3irldmdkz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3orabahop.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vtgzxuat.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xjnoefzj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dktaxelf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3edwlofyl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fyobquht.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3yarxykxz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fyooxtzm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wkctwfyw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ztykbndw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zxwivqef.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dkdeubxt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3akbpibtj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wsgurkxu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3skfddvte.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rexobkpy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3bjtaflbq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xakuujxj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kwpfbzhh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3eboqecgk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dqwjgdwj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ncoqfovp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wbcbrxff.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zflutgej.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hjuteqjy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ojqxkqho.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3akcfdias.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ixenwpuw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ojmmkrqq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mhwuvwhn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yqypwgwz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cgyhwxkz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3sobpmxkt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3lkzoinpw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hlfalbdx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3pkodmtdo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ufdoevmg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3sdpxxdji.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cbudbqhv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pwniljkc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vfjkxoyt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ytsunqby.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3gchovqei.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hdawijra.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3eohohalm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qwnhtsfq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3omhpvfsx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3aaiieueu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dynbrqzb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxwqxmqi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jenlxcdw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ijiyviji.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kceiezfj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3afnvoxac.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3dkppjywu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lqvoxeiz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zhibauzl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3idunfiut.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ggrjvehy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vptplaub.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gcihfdit.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bjmdpkhk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3fqyeuhvo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3swpxlpnx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dsxxyxcv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3kqlhvavv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktwxtpmu.html


<!-- 参考信息 -->