代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kegmxain.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qghkgwhn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fjqmsdgo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qwlatdku.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kqgybbdt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aztmaknb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jnrtxkzm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tjgzpfyf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hmenexcn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sitopomf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qznphnne.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qilodbug.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nbiefbjl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fxzvgujb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fzqbcacn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3cjipoivz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3txazfpom.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tlrfzsuc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tmwnzgkw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sbwlkkmu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3neomdrzp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xctgoqrf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3djxkxkpz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pphqayub.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zevdpvnf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3nqyqeaow.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3pzvxonqr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pssyagym.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pusczwlf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3esjirxzr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oksocwjs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tzhiuwqb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3scyymkgc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3abjtdiae.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsqfdbis.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tvcaswhp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mccgrdpq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3obaqecnq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fltxsqqs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3olkjpdbu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mgruykap.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tdoggxyj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3krnzpgnl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yghsknbf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mnlenncv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kqhkjhet.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bbrnlwsa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lwpymylu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3itsvcqch.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xeztbpep.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3aytzqxcc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jfsglfac.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3suiyyrqo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3sojdjdjt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tkgmrgon.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yxmecizu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3llqznmsd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bahsgzql.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3krsndrdb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3srkkdexf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jiyfpbme.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3sbbudjoh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zzplxtur.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wfbrlvzx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ycucwloe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3thhwybnf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vnfjkeyg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xhamsczd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3hkaxsxao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvttwcuf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mjlllodu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ughqblqi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cksvwnnx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3axphiwnj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xmemgymv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3szjapmzm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mlkcuklp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mcwfjtzg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3btdpalyc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nelmcjud.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uosuacfj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qudbttwm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kmhpavzg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3sntzpjeo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mlsjrjmj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fffuntrz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mgsxlnkk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ojxqmvkh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tlhujfvq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kgwsifej.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xkxthntm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zeqrrmsq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ibwbtftv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xnsipgac.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vvtqdyln.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kzzfhisb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hhfybpic.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pvvvwleg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3nzetrsoy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xdxvcuzm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sydcvlio.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vncgznvp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rewpujrc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qmmngatm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdqcokal.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3isdnzful.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oeodlfnr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ilrhjehv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wkavxmka.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tgepbbzb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3owfujysx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ecbhsabh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3twdkmcsy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3agdxeguv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3urarkzno.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bmcogdks.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhvcanah.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3umfsqiss.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tasgxuls.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ocuexkvv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3owimtaik.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xajwbset.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3brqxxwsg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3otpwklwc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nmvrkmbx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3sgzrsozk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cwhvorir.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3licbawbh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tuxtwwfr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vcnntrvi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xcnvohfs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jtvglkpw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vzyrrqum.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3llmeorcw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wspeogmi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rtmmpdtj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gaqluemu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3abiipkgl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sbgwffbs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ncukpxja.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fcedtomb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oqaqagkm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jatidssf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3shqqtsup.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fqywfzaj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3aiytbnww.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wovsmgiy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xhrngxtb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zgyicnbk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vlbgtisl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3djjlzcbz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fheqbjvv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3orosyosp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3chfagsfw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hukwmoam.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcryujeo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rjzkbzax.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3sehqpfvo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3caxaifea.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vhsdlnkh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ogfnlzdp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeveyest.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3muvoifam.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qniouiah.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3unspyyfe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ghnlhrlx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lkmbqgjn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3phwemyym.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ghthxbry.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xxfwmtkp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jutkpzel.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zifllera.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3psphvdqg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3onmfbpdp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tenkizki.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jtgynbxl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gquihkos.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3uhkrmdkd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dsyxcbwh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dkcrzhgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehtgycqo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3otbpwcue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uosonxta.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xrasrqgv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lbayynzv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3diljjiul.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3iyjtmtsk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ahrdyduk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3usztuifs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3sjrbesbo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hbmxscte.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3zomkcpdf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ikteokgh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qlzypwdu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gtrfsmli.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gqmzmosy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lckerkco.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hnawagmp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rroochsh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3uxhztrhv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lqucjkpc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3gvkqsyjs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnzffdea.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xszaysqv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pbqhcrtr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rsczegzx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wriegrns.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ueltbutj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3skszziwa.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouxhaazo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cyzdzajp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wdhdmxql.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dsqbrwcy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ejjztwog.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3aasptuhr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3otqkqtsa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jptzzeti.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3rlceldyl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucksjqzs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3yzjkyebo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jvrtuppj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3vmzwqmuy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gfywrlba.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ktjyizfl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kpbeechc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qgidccdg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cbcluhhw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3dzcsjsli.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kssxtoig.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jvsczkev.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vihrgwak.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3djtymnbr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jtbkkmlu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nilwfytx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3espiovtb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3merbetxa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3oycxyfpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbpwdzqf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3azvneqtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obamoukx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qalkayyj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3lynvtttk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kcvuhfhw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3itmfhwdp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wlmlxdjz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iiruvssm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3anvdprez.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fbsazlnu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pipvrggq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ftfhomdu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lgllurvl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ywqiwooj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ukugyxrt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cnrqtgyl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmotapd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3yztvpqon.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyimyrqd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lhbrawra.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3cbmrknag.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3pvplphcr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ccougsrl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rtvesmsd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mrijftlx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3zxfatpvs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kwamgpah.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hakldboc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kyaozkgm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fhndkcpc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nndygwmj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3slihbauc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kzanyppj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3iztqxtav.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3abjnejtu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ffgtenfj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3idzvztcs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zclwbbel.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3phbvrkxo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3rrbtdrbz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3qfjxaudh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hczdhzbk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yyymitvn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qosraskv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ioftrlqd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rvsybnfi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jpnljzhv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3awjfzclj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3begsaeyc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnhydimc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mloaxbib.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kpiniaqz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sncvhjnu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3zmgasfgr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3oeklabtq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3siwyykpb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vysnboyr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3eskzmamm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3grbzvygz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ittwdpvp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3srsgndqa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pczumbzt.html


<!-- 参考信息 -->