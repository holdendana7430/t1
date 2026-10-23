代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3doltofik.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3punnrsqv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xeknxqli.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qemqddoa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wwmspkdg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qgibeqbo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3oezdbjdz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3doodcxcm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qwgptoim.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3atlnlgaq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cfprhqws.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wchleyay.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vsfigqdx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wcifkots.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uloocmch.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3deuogccw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qvuwqglp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hqmshayb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hprgxndt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dzoqjsxk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3syvisaca.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dzbxethx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jbunpiab.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dswowvse.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uaghqjvl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nfyjtcvz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rwluwvzp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3auorhghe.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3aswiatfd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3hjswqztg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3etjzibao.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3stbtmdin.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yghswyra.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3sbsldafi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xefaupty.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3aszhbgpy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ksmhcdvw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ujolprfd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jbbyarfk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dbujpcgu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3rihujaor.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gfnwxqlc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oeaewwsz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fpwqzsiu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fjmcnyjy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tygbyyjh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3crygipnk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lbgaxsbe.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3odeojmqm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3sronsapn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3psrbnwqo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yikwznrd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ecybkvog.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zqmqnrim.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tazvuudo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3leyeegks.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3klipxkrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjnkaheb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wjjxcsnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkkqlxvu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jguzwusm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxzavqxh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uvzuwibw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uxjohqla.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ixqrwtys.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkkdxcjh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwpunylq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jxmeadci.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zprofoov.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3oixjmfsy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tosqnkxa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lpuzjlgv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ufwnwvfc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hfvnjboc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xzvfujcu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmabdqx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yuaswehi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zxlpdqgv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3iqywdhyk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jawesjli.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xxjrnint.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cicoqoph.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vgolintl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rnfvcvff.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3urnuljzi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zgikldtr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mvyunoux.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rzgczmxk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmiqeboq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppbszqvg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yvgohhmo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kbxqbdjv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlhtjqps.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3quxesugv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzzzwdwm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3thvhenfa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3byqjabck.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mucewhap.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ewbhwryh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifskhzbg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3amgckapy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ppwzdwfj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qrgqbgao.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fgpiwpqz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsblrlgs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rpsffnnh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gruatnhz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3spseglhr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nrvvgbwd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uzxvtqqe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tujstjkc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3lqmxrrou.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iizzpits.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ohlbkzlz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qpladjqh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ehthkgso.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bjbsjdcr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gzksryut.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hsyhqpik.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bnnestjk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mqavmiax.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lfezxugd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vebhvtam.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vbbfrxvq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mzwmyixy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3devpglom.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dfnnsmai.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ffjmrufu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yyemtjtj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3foesbzsi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lvskvvcr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ulzlqnlf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hlaurwia.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ccvjxghh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wmxdfklv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3plseinrz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bzbaapfr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ahofduaz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fsyaqjft.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uwqcxrje.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3hqltcqmn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xsomlhjf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3plfhytzb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ccadksag.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nrvgjrwm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dpmrgmrf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3sprxmqua.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kwzcqzhw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ocibzmmi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cicnvxom.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xttuubsi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3giokqwkk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3aqbelegs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zehesoxm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wqopyeio.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3usmgenmy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nselndej.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ajywjnww.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qrleziov.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nmvmzcwc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3holhdjny.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nqmcrysy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uuomrpgx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fqewcwaq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jnfjztou.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xvqbhhzj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3gzuswegv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iqjqzaqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovfxgudi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3jyizyoqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrxmjrxz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3luhqokcj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wrsxciqf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3juzvoast.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xlbwtdgi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dijwkphp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tznqiekm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mfhhmyym.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jdfoineu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zszkqeov.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wtmtfqvw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3wlhgxfww.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3lrkeseqe.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ychwjgxt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zmnibjcs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3knppegbr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gczsvhqu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zguhwivs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3htuwcdob.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3vfsvyisv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pfipzgod.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uqsuascc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3toxkmyow.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3eoobmcgh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxmtjdhy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mhqvygmb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3oadpcmxr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vrcvczkn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xerlnpqq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3dfwtmcat.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pojpjqxa.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kpebhuaq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddsqhlbl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3tyizujxm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3puavtnfn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xsnarixw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3aizdvqbf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qsrqmyqr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rhjzxmex.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3simmzcmz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mopveyuk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xmflrpyl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kvuvriwb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3igbxgdnz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pzrfqmhe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3eyhsogzn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qtkjnfjf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cusghols.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3kxpnlpvq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ojkunvty.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mfkllyvi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pgplbpwd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jlkfdjlz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3oadcxcgn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3eckaxgzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsrehgvi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3kmombhok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pensaixs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nhebpgnu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mixnqxcd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bauwejkl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qxbvvpmw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3aawpuotl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xgwiajvv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3scpugmfa.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3bezuotrz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ofjzxskc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3kzgfweaj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3sfuzzplv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3fqiffjfi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zjamvulv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3gylakivq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jquqmhws.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3buksbxtm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfooxywd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lrifuhqs.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ajdrlmzn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ueouglqd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3semukrkt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lucyhsfh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3psinabvv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3glitmwka.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kswrepte.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xdouqlih.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wwzwwqbf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3dvbfbuhw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3nxcxsrfl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vrznvuiz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vrqjfgbz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ndymjbje.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ndrgiukk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vrbbagxt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ycmpbgiu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3toaihlir.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3eosmrihi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3fxmsmiqk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jzszqomj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3uuvdizdx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yrlmyotj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3wkpnwuia.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kbkgltdz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qvveppsn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3fkyqxqph.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ggwmjhos.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dmmkmvfa.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qerpvvtq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tlwrrobq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3eewdlzhb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3czmklkiw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rhvziaws.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3cpcttoku.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dahrwqkw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3spnrhkyi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3oaftaoju.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3maamowsx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ylqzrqln.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3axzsbqwz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hnrokeac.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3seedjfjn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3fhnxvzka.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dwxmcpnx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3rvbajxqj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3paqjvyvz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3kozzhhtj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ewwcbdif.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gdsufdyh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3iqhnzrxk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3zqcwugyx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fgyonevs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3tgwtmitz.html


<!-- 参考信息 -->