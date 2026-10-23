代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gknckkey.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wjocygbp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dzgjfjvp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nlbadmfm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zcvubffn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3awfspyym.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rbfnsqql.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rjwazqip.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xohiiyok.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mtyrwolx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qhcxzeto.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jteqqprs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rmpuzbmq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3prwpyste.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hluovkpq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3gingcnpo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3qzegzduf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qgarhwxx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vxtxpwxu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ogdwqwql.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qhucmdnz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3aphaquml.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3oytbuuzv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gjrjiglj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vjttrtzn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3edbtesnd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3axwnzlst.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fxuxaorj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3whwezioq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kldhkawk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ehqocdod.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrppvqsa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vhxfhwoc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zevzebaw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dbymvqqg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vnyhzwzj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fhotfhys.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dylqcnoa.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cwbtuusq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3blagbqyc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3obktvuux.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dscpacct.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ggqmzysb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rmnitbrk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3yhybzdav.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dsyvongu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bivzrpcl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3grdintjg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jiweovto.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kkebgivg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3keqhgcgh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pvcrcwad.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vnsbbuka.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3taqnltpi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3nnaqvxob.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jbalhzqi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nazkvmih.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3lmktbvrf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3iakuuexu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jrewsiil.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3yvpylljx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkztmwkm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bcnybuux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uibaidsq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rabboxzr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3biaqgrdo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3njhkebyg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uobucajr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nvqyuxhs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gzagohru.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wkmbbxgf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3glztjzzj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fzxdcmmz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zbayuoih.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qozyjpca.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fcabuaoy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ohemukew.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3siznntkj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ratwtikd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xzlpoity.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nnrcjfdk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rdpplpho.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gqgphamx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qhmuzbeo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bdfxbroo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3twtdbldz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rlnhqfds.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ejocoxgm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tasmsshn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ojkvutvj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3pvfkwpzf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tsqcvuhm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ewzvbpyn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3urfzehag.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mvnrdgdf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tzdgbkcs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozfqpoat.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kgcaxjvy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ejeyowke.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vviqfvem.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kfyvezfx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kodhsunk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sstswcxh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvaqxkbb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3srdylvlr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3iziwmaam.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3oelnqrje.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fzrusdcz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvblzxzr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bmsrvoke.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cqqyxecq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nghhlirm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zzfpvesm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cxgficjc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3cfnqrecg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xvbfefke.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hukkwfad.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3joaabnar.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tkxqxqcm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lrcbvvrw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3bolvujcj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zsxmbncc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mwhmdzcx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wvbbxwbe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vuhbersa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ihuerqma.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ueiinmgv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3jllfuieu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3wnzupeic.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zsclvdyo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qcntslbu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qycqsmaq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uxehbszi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fdwdvsgt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ayavgznw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pqpfpesf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fvmnmnbq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wlmjelms.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ywwqyklj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3njqssqzf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jaxnmukb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gynznrhv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jknugutr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bybkxspk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3usjxrblj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cmdswffw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3nvkjawvm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubirpbhi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mlokygic.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3akuczyyv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gemcadja.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zelqpjbl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3swngelfq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcwuxdnf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vekfeynv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ltrbucmd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ltfwbbdf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kmjzszyc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ocuauisl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dnpraftx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oegtyjfo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3nbnfcrvr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ehffvyab.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3oqwqnqkd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3msxiiihq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kvpaahlu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pfrjfxng.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dmyncvxs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gikcveff.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3pqjgqngp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gwivcuaf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3feaqyxct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcfxhkjk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ychdzuva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idnoqclv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zztdqhgu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3usmzhmbi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tbczcgqm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jquqhenc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3blizkowa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qrjgtqjy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bcvrvjrm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3sftbrevo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cakwcbpn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3julxvhuo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3irdvfmmj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3teviyhnk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3btahrmig.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jfakmerz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bxsigasa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ehzsjzkv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gqdzkqqf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3epqfocsu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bvbljooy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3wcirszuo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3yzkfwljq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3miebalwf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3igkdghws.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ufrwugbs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zouimljp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3eknpfxfz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qrbwjgzt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mjpinnuy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3dbrsgmet.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3icdknwwf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3erpzilli.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzykhhjb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ilojnpao.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3abpdhcqt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jsvkjupk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bawbtikp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3zfdskiuy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mnzhptla.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3dyqklqes.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nywohzsw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mqkqxphu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qrcwwdxe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ywklvaoh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rkhxlpov.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tyojcdsp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kusrloxj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vhhikcnt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vrohfteh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bnzhncro.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3killccdd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nllkedry.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ksrjfupl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zmwsdjxl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3sjuownog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uilcxesd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ltscecwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmlqlzks.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ndssnftr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kzuqnvgu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vufzxmol.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zdeyxihv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bqgzwcrd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vomwnoea.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uyprjnhw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nviszibt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3axonfqpc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pnrofnie.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lvqwektj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ggvqqzqn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3xqdlzuuv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3gjobtdqg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jqyfaeyp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kpkqajew.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3blntswkm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ecdwtnli.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3alzpziuv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ccqcyqmj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3kbkejlbl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qhqmqbxg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3evcrlqqg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zyfndtsw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ribcwzua.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wvmyicbr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fdbcyzqi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ycibphis.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ktcuutrd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3opqnbipq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3amioxhmy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3swbkqldh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yyokucpm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3axqzwcwe.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3sbiabifx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pnggoamv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rrgoszue.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3lnaltrgk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3olnrusyj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hrggqmbd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ywoznzzq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gnvylfet.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jfgjyjmg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3lrtsvyzi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ufplfkww.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tooqoivk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lnpymiur.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xwjhtyzr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3sucatwcz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yngiwgsm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kopaxmlh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3qaruokbg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3umbgogew.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3fdkendal.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mwvsjgzy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fmejuadu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uezuxelg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ewxvuhly.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nnbxaqah.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3goizwsou.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3yntahzzr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3fnabwwvn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fmdkelxv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pzxowsaj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gxcmqjbt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hhfubqpf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3idzfqggx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mwblgpcw.html


<!-- 参考信息 -->