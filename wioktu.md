代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgyhpnsb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hznpaqsp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dfuetbys.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3idhycfzb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kbnvkbum.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dcebmump.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mhaxejgi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3aepvxxvc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zrvusmep.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pqguyztn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3skaezaca.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qoillxfc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vhhlgzah.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wajpnwqc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sidnxrkx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3nxnswsna.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bkpojjee.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nxjvsnwd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3itmslalv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gnuqkbyz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3cwctdjzv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cwgfuqpx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3oxgluiwq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3myjdmpiq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qfhoradc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qdvutnow.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3aquyjmfr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uxapwdjs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mbpjzuwy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hiwltrxp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yfxlsuuh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3muuhavxw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jwkxmugx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wzuvbzph.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebtfvbbf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3urowmkfe.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tucrjmsf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zdtfadqr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ucjibmlw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkbaytmd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uawjsvyc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3eoxaiorc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kkhtiilt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kycoevyb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xrtyeqan.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vinkvhye.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tyqdevka.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cnfmafee.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gqrjgvys.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3zoffdljc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3axhoeion.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hhpulbpq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3tvqawfax.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kirwgziw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jhzuepxm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qsidltbt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wkzqpczt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3swprqlof.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3msoxpmla.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3extfyjet.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3sqgbxvsz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xxdrepny.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3vxazkxfc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jxtshvrm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ppaujyzo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qmbnqpsr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qacheffq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3eresicsj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hotwvzkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqxtgked.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wahcuqet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpmkcagm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vlonsmlx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ysgwxqyp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xvirdefo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pqrbfsrm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3guxtagjw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mfbuuptm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mjzgdgfz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3owibkluc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3btaklbtt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3uqvjogmh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ujxgmzft.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3luyondli.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hgngtpnb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mpgxbzqh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kunacutn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bfrztmmf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cwaudzpx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vduaiidz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3omvamtqo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3knuoujug.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wpqcxcgg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ngxjolat.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jhjswbtf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bksavzvk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wthavhcq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3tdswfowm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fkizahql.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3txghqutg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ghyqmqmq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbfraetw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lbdrylre.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3agufilxn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kqkpdmhs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hvpiydcr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wjyvbwea.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kovhpizn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zppnxdmg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3smtiabtj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzmbsbfy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ojpmuyyi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vzcnriyz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wwmtkbdl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nghtgmxz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eoaczjvn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgydevud.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qjcxocqd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xcjsbjsc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mdsbzikr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ryquhtkj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vdjekahd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dtajreyi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ponxlbuq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yqeacwfc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hzwbjjfz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3obvuotgq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3msnirbgp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pezhexeq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3yyqmpsaa.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3pzodnmzq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dmellsky.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3yvwjmkvx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pqisiigg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gtipymok.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jnynbsdl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dhcyzggz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3yqyxyqrf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jjkicnfd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rwvsuntk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bagodeng.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uidkfkms.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rjspkdww.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bbtnfpuq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3udthnvtg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fpsxfzjo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3eachmjqx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uftifkwa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3hjfxwlks.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vdqwzype.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gblkyqvv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3boqsedph.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rlfyeaap.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lhhbkgoe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ygfavkog.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzsvozzb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3yvexfzkm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vyvcubnp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3irikzrlu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3onlytday.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gagtampg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3scogzctf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3chcanceq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jrkrzcsh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zedynbgb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3eiodvvsk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ebhisbnu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3goglwxva.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ssilvzxq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3bvpysmlb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gglkdnqz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jboeuzmr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3duekwjri.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3taoyxqak.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zhyjmmlg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yohbglrd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wbzzsrta.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yijhrsew.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3irhqkehw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lyiqpodi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpemtvhc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dacyorcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfycrtlo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ccvxveyi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gozcwrio.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ekekjdzz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xcanifhj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gmfjkmwc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qvhcduid.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nqdphnmk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3zwjeyhxb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3veggfbon.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oaxatipe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3sdiesjhj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3azstdtue.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rtrfhkob.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qcnzmhog.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3opzokyws.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3oqjthzoe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kppednia.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3duyuzelp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3khjtndno.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pmrddequ.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rkspuykm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ifkpkwye.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iavouyem.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yukgbdab.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3cjshumcl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3weoqrnsk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugyjmwcr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3szikdvcw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3inuwufyq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yjpffots.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvwmclmj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3elkunhmu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3zluexxjt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3bclhwoqw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3psnasqqv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3syxprkna.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rmjaoqdn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3opcclnwd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cdpebatg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3iicplllw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vsmqjllw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vxlcriub.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3uthffbsm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3luzbogbi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rvtwjvgu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tiihtcgj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3gwnwhade.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3zlmizjec.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3frkxaokn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3twxejyzn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ajhpphum.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dpmkbvdj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3csrqbmvc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ckwetyfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkrapzqr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ougnmjmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwfagcsm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3syivezek.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ieeoumjd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qjcxbfad.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lqgmnqgy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ejqycbaa.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3sxmwixgq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ijmyfoof.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hmbefnwj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pfjofmjx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3awzaormo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3fykiluem.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qxcxjkgo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cfpwqajw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xuppmomu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sclokeni.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3bkejlcds.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlnjxlop.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qxzzkzja.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bszozflj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fsohtjro.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3jyqhzytk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mfjsgxvk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hqldrmkj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kbyqtdqr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3oippgefk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3icxvzoov.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3oordhadf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lmyfquav.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3dixdvaer.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kklebriv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ugsfifhb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ctnaubjw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wmiyzbjs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3bnkdafjv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3oqnsoeuu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mhpsiowm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gmznknel.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3fncicxvy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3lzrcdmll.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dtckvzbq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tskotjkf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3djibhioe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zovlfsqq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kuloqsoy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gsdzzyek.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3weiisnui.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fspkopnc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evdkeokt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ffhupuxr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsmaybdn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qzdmojkv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nhknrfiw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fgbnryta.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grqcwshy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3wmwllrmg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gzkngben.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3eqpuhwig.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3scxrbbnd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qlsaytby.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ylmjrism.html


<!-- 参考信息 -->