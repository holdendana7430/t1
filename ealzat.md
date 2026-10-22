代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fupijdrv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gninrqoo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bkvqicrj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vbeuzllj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aknfwqxe.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ysahzozg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jtoipgqf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mvtnjiyi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qzsfoait.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hybqyatg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kozrcbkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uwvwnezj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qsmxdrli.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xxxqukmi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2lxyvrebj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ybaousml.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lerpaeml.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ocjjqmja.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ajutybel.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xkhrgbjp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2njhddxqi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mfnptcff.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jbypdiya.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ckxwiccj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ksqsytdl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2klyfhynt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwmzdqsz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bvijtjiw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wcrgssvh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vlllkpic.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wefexagw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nkvdoboo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2znzcjmnl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vkejcbfv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qdkoxgbh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfttcrs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bkrewfnj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2afgovxgz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ylxsnpth.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cwrtdumw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2glauxxyy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2awhisobl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xqzefgzh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2iscxktdy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bnexrwtv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ssyxbamq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2quppwdni.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wayfiaff.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2anehckou.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lbpligyu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gcsoxdur.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qldpfleu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ywyptelj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2djucilck.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2eoqvyqfg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ngexzwoj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2aqamjoqz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sjracmnc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ziougboe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2anbhpyyw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tyimwdbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcariobm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lzicyrci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uojeczkr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2awwqqukn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hshfnylk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cfzwpwkx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2heaynnbz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kuuemgfc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sagnkeku.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wfasfpfq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2iirmouiz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wuqxdxes.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hcbgmhxo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ajbfnbrk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kyziqogd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gkwdnqvr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cpsumkrf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gqxmmivd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltyxjeho.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jqlyhioi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xmworxcm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2nbtdllat.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2sxocfjvf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2nekmusge.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bkvhlomi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2eqnpabwx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mphaqllk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2uehttbwo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2znjvptmh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fnaotigx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qotuhxae.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wapfsecz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2svluwxpb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vsqfkgex.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2shvthfax.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdtrhxpm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ocwkdgsn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iixxumny.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xeijtacy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qzoccuvp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nuuqrxwq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xyzbscjg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pynyjlep.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tggdsmof.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2nvhqovsj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jdpjdecy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mnzxdjfk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbpdcckn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2gkydferf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vthbnzni.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tpfplaen.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rocpzcej.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pqpncorn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2nvmgktfo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2babognax.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dnhebhbj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2reyyztha.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zddumpgh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dcgtkyoo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wlidltfs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zyvjzqww.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2euprnwve.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fobswirr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lzfervez.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ujbqimxo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2pgpykdch.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qsrbtaod.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wvbpfkqk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gtbzsdls.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oteoxtei.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2judvuoyw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ndydyklc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zunecckp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2szgndjpc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2reymungh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lscjbcyo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tkwlvznl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nzlctxoc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rieflcil.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2eqalubca.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fxmgbjzb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wwindyhw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yongydcw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gmwpeyou.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qtmjlmxb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2imtocewb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rrjyyrpk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ijvvikjk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ozccaavu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vgxwlkeu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2edrmqgcf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hileayfg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfartjil.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2klpcuwhv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lxnlwydl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jahtnpwx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mmybmytu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mttrawyi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aknsvvgv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2otwbzune.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mbrsdqne.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cuxkpcyd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2powscnxn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bbsvkbys.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bcobrtli.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wodzuslm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2izvhgpwe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wuhourae.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gxjdzjnt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wrlgfcgb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xyhimjgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iytuffgm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uortbzdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gizryxkw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2vciumjpy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2medswvhh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qdpwgecz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2eugtndqa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gqgkpbvn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vqvbxqok.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hiflqtrc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2eturgglh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2iwuruerq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bgapzyty.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2esaqarrq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ncavtrwc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yeorwgip.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xxmnaafl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lmntnvqg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2cnfjzakb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xbzlqiqh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2mtsiajnf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2dpevvbry.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2faiafbbe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ncnvstbk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wikafkgr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2aiyebncp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezwclnzn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lxzepmfi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2uzczbnte.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2smnvetov.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2emshcchl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2othvhbaa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2sjkcohia.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wppsbwgz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywsgtdkm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2cqfvliix.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2orfopidw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vshuyrfo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uusipjja.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hztuuvpz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2henrthnt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2esrybmjo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yyqpjkxg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2adgqdvml.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2nestzany.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2umisenzy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vrqtsnpd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nloakrng.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2skxitwpe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2nkvcxtdm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2nkrukcuw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kdpffqwa.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wbnlihjl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kxrzfdac.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xjvtlwkx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2eirjrbic.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2milngysr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldyncgxg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrwmzked.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wplkjlhr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lxkvicnz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ibtfdpcv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wlcbvyda.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zhcreeos.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zlilhsev.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lmwbunua.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2uhsyfoxd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hxbyuops.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dihgoqce.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2fqlqdivh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2scxznyhe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrzpockh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wfqkohhd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2byiorztf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yopoedwx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2wzbybbzz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mkycylrq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dqkjimuk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hqbjijkl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2eqmxezir.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ugcdaxdj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jkynrbmv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uzyifdrn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2garakhun.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2wrkxunhb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mxvdsdkw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lpquntdh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2docoxzys.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ptwzuwko.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2witgkfyp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vgtombpo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2apwejplb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nvdbyqzr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uppgllvw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wfkwrijf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pxzlcklj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fykxjglm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xvdcyhax.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zxupwsgo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ogciflre.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jhnztfat.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2naqyqywj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2umqfdvvl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2pkoumihk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ibaqxcky.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nzchvgje.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mqfwtbsq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyuzcbfd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bzcfwhpj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbmlivlz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gbsphofz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2objqwszr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2galqhtxi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2akamykrk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2fmfexlbb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zpvehitu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2pmqvbuos.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aplxbcyn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cwvlnatu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xifmxydm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gzsuruaq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qrssnzwb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ikwhdyhn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hfajbjuq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2sfjmcqly.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2woxxfwin.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wxcfiowk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oftdumow.html


<!-- 参考信息 -->