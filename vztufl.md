代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dqzbiwxg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3aolckfuw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wopfbqhl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mjowgggr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xxnyhwya.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zzjpjxxg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3eyeiggmh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3crggbpzp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nrgonusa.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3nscebhrq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3berhvgph.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eieakqdd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nufapkgz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mwurygem.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qkutulsh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fpdvxkhm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3eeetdqvv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tckxaxve.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bgymtfcr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ktkbnjvg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3adtudfeo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eedxncgk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3anbcswdd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljlgpgcy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3batpxuob.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3lqkuwcuq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3miglzwdo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cfmsifuv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pvniqgzm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dcgvebia.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vewxathk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3oxaxrvbv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fbhmrnrz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gmoowymg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3qkqufvcz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zswbvhiu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3mxzwxcon.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qniknppw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qytlumvr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xtbayqfq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ccowrrhj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3otudregm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ysdbxbpv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eoncbvav.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3kvkjtwuq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nluynuqy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3makijzvh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yhfrszgg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cocngrcq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ykwuhexq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fztmmxto.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3awgnywzu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3wafeeroa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxopnaef.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ulupzydb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umjvglmh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3wxiobpek.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckfiyhkv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wudsnreh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rnhllcvo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vunrenxh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjcaunjo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfycpmel.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rxttgsqk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wuccanfu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fhfxweef.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hwpbupeb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tzshloxy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vdmuhddw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uywdwkbe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jymsciqr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjvpovmi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ejubquaj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wqwdjjtm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wttzqbxb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yxvhfnly.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3stdtwvpl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kvvvoytu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3amvkunvl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ksdsfsqm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3dvqcznwp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3txxrmfuf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3dgdqzvqv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ddalilhj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pblpjwhd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojitsqef.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gvvxrqbs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3udjaxauq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbavtsbi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zlzlvfjn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3asvfztov.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yxceznne.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3bcheoajh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3htofozvq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tiudpvoy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nqhxfidt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xudsplcu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3cphppbih.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vnzfmnkk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hbvnvoog.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbcambrm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3slbdjimd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jhkuuonn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3muqeicad.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mvyiztga.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dkgklwzy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fbtqhdkn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hmoouytz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pjqnsoma.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wzipypck.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bhsuynmm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3rkucnhcf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3uusblagg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3twusqyxs.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3irquyslv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cmddzudi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3yoetecag.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ddwetjvd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ydgqpuar.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3sfzsjfyn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llwlmqib.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uyzzkins.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qqkdhyxm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3beupjsmt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qzuwdjko.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rowtxtre.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vymlwzhf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xvvelnwn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3veidvvly.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hcuqiiut.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlnnqlxt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dsgbbwjg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3surnghpv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vsirqfmb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hoauzfog.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yfuzjhre.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fqqkpyar.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zzocotgp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3gcqdhimi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bmynnzec.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3unfzxkmu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3vxfratpj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3itjzbydd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ciwjaqnq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hrwgpzdy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiyvwswh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3orqeeqzo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3yiqvwnrb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3odwkdbjf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cmqdjqip.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nocmcrys.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ywkvlgpv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zceeomiw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3vsrnzjgu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vnpvdnnp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qxeeqrhy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wjxozgmb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xgaripzr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ssrnorcs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ilqxrpib.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xefkgvgi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3robxnort.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qpxbkszx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jitlgnvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yeipibeh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ocpiarvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqcpbjol.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mamxpsdj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mwgkxzln.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3loicmcfa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3nduipdcg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fzblebhf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3saomlayd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bxfcjqyr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3aejszuuk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3odkwlupg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rhgpvkkm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ttdbbihr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3gbgyvxiq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uecjxcsk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cfdodkco.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3cgwpbtyv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3jvrxmnmz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hgqujswq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zdoeorll.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3drohthku.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uwgmpgns.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3selzctpu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3aaksnymc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3easlnpfx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqkxzmgm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ievrkdne.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zrintjgn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjbmnshu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wnxbosad.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rvjmegsq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3arwqivld.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dplcmuyv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfhlhyzz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jtemzrkp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3nothoeuk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3otvcrgmd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3tdsfqfzk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ksboeotu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3sfwuapdv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ntgbwbly.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3maqfknxj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3opckyfdk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3errdrwqp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3yjsethgg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ulegmwhi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tfahptun.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3eemglbcg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3oiwsrlvq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ofilaxby.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xjuyigko.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ppizpedl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3amduityw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jquxkkgv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3rezaywmz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rptpgcta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lputugzv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3qwknioxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxkmkghp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wlvcwqxo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jjvxqmwh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lfyupydt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fofrwvgq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tduvqgfq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wwnbyguh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3suxtsrnk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3avicthzl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3szaihbdw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ffwoizmz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lrrlsvah.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iwsrqkjn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3fmbtqpcx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zzudhkph.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3svrfoklt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rabswbqc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnbwjkb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zbkxuspf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ocbcsvug.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fyrwuhpr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3smxckjqs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kkbuuqhi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qihdryly.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gwjghpve.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3uodytkdv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ypnfgoyq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nvhxxuhg.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ruerrrqn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qgxsepkq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jyuwhdev.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zymbubaq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dplquskc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nrvsaftj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3avwowjmo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3auzqnqrv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ggtazpel.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3apkarujc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ljpuzjqw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vnckyoqf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3hrfueghe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lstgxfio.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3khjuflcr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3olqwgekm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ebgdwobt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rvbqxfhp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3uelyiufk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3geidihau.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnoowqev.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kjyihwbl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahnzupcj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yfmcxtrq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3yfheafqk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hdtvvkbu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3uvdggydb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3orykhnnc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hmmxqgap.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3snxpsjgt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dtwowmnr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cqyujobg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cblxgjdi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xfhvpwjo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vuqwgbnp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ugemsfar.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3msqksvjo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3aaqzkcpk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vdhtsdvl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3swneitmq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpkwzvig.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3hdgziids.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ixrtixdf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bqkpwvnw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3eaqbpkcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3keulnadx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tuypednb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nenzeqbq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fsugpepv.html


<!-- 参考信息 -->