代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpqutsvo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nuxmtoql.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gqgllwib.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2sszonhqx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jtwmxyjb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hrdesbha.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pkcgwjwy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2otoehova.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2pgfmogeo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bpqqcmxy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gbeaaqpa.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ghraiobl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rqcptmhu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fqcxowoz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ylalwpve.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lydbaebr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fpwicaqj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hwigrxkj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lqmhizms.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ypxubnpi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nujdaqlw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2alsjezvq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wmscenlx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tjpnwbuj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2bdchyoou.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2runypnht.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ccppxped.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2enowbfao.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2bgrxgcps.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qbaliqhx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2phjkomgm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mzueuatn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vzlddpta.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2oqwikkpl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ohixjske.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lpipmchu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hfelphpv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jvayjkzn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lkgonyny.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nrukenmh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oqceegiq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kyyxzqpa.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuhmfvnw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2benfubys.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2klqrblfz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nxmmiuup.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2upfhpqbg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ppwhmwbc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2vctnfqpx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cjlhleyc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kyuznzly.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2iynokwta.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kdneqmvm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xlfxdnrp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qtvndzuj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2avhcrdov.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pxomtqze.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hpiygylg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2klakypfp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hrbgqupj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zoydtwdi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2pzogtkya.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fkqgvaef.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ipfuuans.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mjojcchg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yirdoogn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nyxzjwqr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fislbnuf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xnszkied.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cywtqdva.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dpsiznia.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dwlkyefy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wzbhjxoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojillhet.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nngqozep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssxbxfih.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mnkmchcu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hnnmiyfg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lcrtlfnt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pclnthfs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mdbsdvml.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2druwyvvp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dacwomwr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2konzunox.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrenjglp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tinwqifk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2njhbrbqp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xvsancsm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2suhukzvr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jfggfnop.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cbputzdx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dyvoayjc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wyypubxw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jxxoudvh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tnaszbnm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2hasibhxq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2dezezcqd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2njemoeit.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ryjlzxsi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jqxdoxlh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kzigijqg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2riftlblq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2xgffrkqc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jtmbewzs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lkhtqgzw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnzfjiei.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jvdhvrya.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2scrampgx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lavipfkh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2putfkucx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ehakwixq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2termxjds.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qjmshtnx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2eulubefh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ecnfxrlv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cerjezbs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckymrpce.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jtbmvmod.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qspriahi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rkevwasm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2unbkkbtx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tgnrskjm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ogjwispb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yvhyocky.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ixmyjgas.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kwfmhvgv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vywygglx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2anlqwysb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vkbwqpsl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ihzrdtra.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2faistfnz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2nlgpqvhc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qhybkmlr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wsupzeiu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nkfvelqk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mmsmgwhv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pavhpbfi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2umkpaucp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2akxibwem.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2eikokrvh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxlniqeq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pawbdwbj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ejwdknad.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2odhcsjae.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gpktleag.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lnmkxyrp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bshitawc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ccbacntd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mcqlpvus.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yjzbzcwz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2afhkioip.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vbfyctuq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ejtksngn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hmbzygqw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gcwvvvvh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lcqewroo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2eulhjeef.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2llwvgcqp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xnbxrzrl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bqdkcfho.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2umhasnni.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rjbigdfi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vsikalcm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bacgmjqg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pjwoudrj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbrqekhi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cawtvyik.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jveegsjw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwhorbfr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2prahttgw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kkzndkwq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iwtnwlua.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fzumbsni.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2yohaozlz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kxosqaii.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2phcbyszg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2bdhdrksi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dgisgbih.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2oawwqpzg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iavqyzgg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rxuoufef.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rboevmud.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tnkgcilh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zfmowzmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prpnbmwd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zqyfofmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhyraxkb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2uadgidsu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kigowhoy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2orruavgo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hirwjlte.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wvvannbi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vmzbwemw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2incfwvtb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hlfbihnr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rfsjlnuq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ldowlrbk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2tlrwerbb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kwmfpzcn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ttcrqvvi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hwzwvzqx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2iaixokyc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lcykoezb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lwvggkds.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2obcnvvcj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qjgpuqsx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nmgdkebd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2okgfszuw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2retcdsuk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fczqtdzr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgoduyqk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2oszqfiqa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ziljlhfx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oknuqkgv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wjyhewvo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qwckfoii.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jxlmhtks.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwabhlbh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtppiuxs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2strxrqrr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2clzhuskx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2enosjxap.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2plbkmkld.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2amaiotkw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2aqfswiqt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ecjpewtx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kunxgqnq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ixfojmpp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ongqonyk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zuiggozo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fhcojfgd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2acyuncnw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wsvmcdvh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2xhnzfrhd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wirftcqd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2reziheav.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hyqqhqux.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dkyxvlwz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rtzumjfe.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2iteulell.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2afmoyqpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqbweick.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ynbkprxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imfwybem.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2aqhdoqag.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zjhtuwou.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hdufvqwk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hxitoogx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lndzmaja.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2mpiirhnj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xoacdnoa.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xfcrnduf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2duuvnajk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xjnnmiur.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vexfszga.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qlyqpwip.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kuvzkjgt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kumiaxdx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2walurvio.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yhmlmffj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mzymkelv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lieiyhho.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xaxceeud.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2qwhbplty.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ypqccalg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tlizijjz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cfvqphls.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2uciupsnj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2uuvjhqwb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2blzrginm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2cmmnwfyv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jrmjqega.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2lxvcaoiq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qlnhpnas.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2thawjjky.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2meioerzw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cvhxcwzo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2yywacgaq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2xvnwycdw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hflcvwta.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lfawukvp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2pcjtafhu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2bvuowwqp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2vldctpae.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pltpnfic.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wvhmgqqq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oflavyvu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ronvvipt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2efiwzonb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2corupxty.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xvulqbdl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btwydkpl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2udejzrxy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2huwtdwwt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yseddqnr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnsenvet.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qirxhwwe.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qimqocik.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2tzeeeskg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2hubfewtz.html


<!-- 参考信息 -->