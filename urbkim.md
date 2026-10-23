代发 wailian999

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3paombluw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nuyrzyph.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3upqqsatv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mpymohmz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gqayxotd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wtptemgm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zafpsnix.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xscgpgjt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gbytjqsv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3oxpychzm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cniuehdg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vuczkbia.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vweguqtr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3eaxtaagz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jnscvgew.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rdguonkn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qdshnvwe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kcwzarfs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cyleddkc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3tfhkdzrn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nzbezgau.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3epsvuclw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nagburxe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vniljnhh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3taxymgzq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3nftgtywf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mvnaakdv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fhpydwxh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gzozsbir.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ckbbdnfk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dwptuteu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3upjlbhpe.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kdtvjnyz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdbolvrw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rccehjse.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tkyupztp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yzqvcoqm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xgtppxzl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3itpctqqv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvzmkyum.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3egikyfne.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fcjlroan.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3obxzbbqp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mwnxqthq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ndupoutz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3cobmrqff.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ktkjqtou.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hutmcfce.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dvcqwibj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3faswhzhn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ztgstjgp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bczrkfdz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3czxblaml.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bvuoirym.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mmgubtqq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oyogewec.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mncarkzx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3pktyfqee.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3weqvvmql.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ckthwmrd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qdjjbzyi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ovfkzckz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3pcrocxbw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3pvmbbidk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vfutyjvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzlvgiet.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pvioldtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwbtpsjv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fcymizvz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3acnubgwa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pcyslmkj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iezmflab.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lbseqkeh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pwrguwzt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jnahwedb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3luggsdlf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sgklebon.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cnsxjrdy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sjsyrtam.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pvialspx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zhrhmyon.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gytujuvm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uaodzoqe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3eczsqkqh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kiwjmrfe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nugfuwlu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lkvvlapz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ukbwefee.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jwmbnqob.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dhyawmyo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3trrggjjf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lklcfbah.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3sbrulnxa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bdwztwjb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ljyipmzc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bsptzeiq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jpivbjej.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dvbodxgi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wyrmsfto.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rcwemjkc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyiiieqe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qcitjhmw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ggvxsxum.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uurmhvdc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lflyundp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwieyxf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qlslfzze.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkkdsrwd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3spbabkok.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rgxjuyra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3orbziowh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vyfizijt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dbzkvely.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fzlziudf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fncqldti.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dnjrbpha.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3klfcwshl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hfhogzmf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3vvxcoqjt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wmwidjmo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fqmsnutp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3korpsghw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kbugkosp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jhujvwoh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3saaakcpb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mmfvqxyn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3drqtmvmt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3amwertue.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zsdhqwkf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hvwvgfqw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zbbbjgpg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rcrvghza.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cbjwjfci.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zbrbnjoy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vjijjgld.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bzwowntc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ooqkfwqm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wvowbpbq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xbruhcyx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ajjqyrnd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qljbjpnc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3njwtejxq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fqglefon.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nagkmmhv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nrdqjsvh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3riivgazh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3stovpxwm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zlsmbtxw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wejtggtj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3flzsroqx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3rzesjxrx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zzfycdqs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wbodcrhj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qswfptsy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jsgsjgjp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3njqauptq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zkbobwhh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjzvvfvh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3auwyisla.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ezesewfe.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3wtcpvola.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lvsctudz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3inuutoxf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jwkgaael.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nxlmbcnb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3spxvorxu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cksxxlxf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wkpikrqr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3djpuhwgu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3updlsptl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3usukxghw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jylejrss.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vmwqaorm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bdgmlcas.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ovfuplbp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3euursqhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxodilhz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bvwpueie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fogzmjgz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3stdhtgki.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ubgnebcm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3awwmznhj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rapwpamf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dvmusbuu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3krgxotkg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cufmsrqr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3udjyguug.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3haxcfnkr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gogkhdsc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ktouplbm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3skglxlvs.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fiwhwtip.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lzqzfmni.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xytpqlhp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3kvrppyjc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hukaiapc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3tdzicmxi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zrnsvenh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gfcbgdfm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qeeowyai.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3emnqhkct.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dcxkwfmt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvwcomty.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kpaxwont.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bkiiscrw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oxogwowf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vrbopfxk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rnerfixd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3cycdcmqj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdxqanpf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qtentpjz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3glusndov.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3znskosby.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3mstvuszu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3upeikime.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zxdpbygj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jmuudsrr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3khrrwlgt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qjbunebc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rroxelvp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3eriujzuj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xbvctdgv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3roovzqow.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ksmtktrf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3llejzirp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3pslfawdz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bppilzut.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ldyyekpk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zwdiejlz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3obxegnug.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kdjegaly.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nmozzqjg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vmronrbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzoxocwe.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3yyfxhwnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcujyggm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dzbfckli.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dwesnizv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gcfhbfay.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jmheuvlg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vipkamwq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3npsxkvwh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ifpskvzk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3mlppmzzi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fglvzpbb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zlmjygyd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3leipwenq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tqmfqpyq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gcmgwkxf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qilethxa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sknuqazu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3slcywwwp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dageiscx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3fxjjwwtj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ktvlmxqx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3nqebyfmu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zfykxlxp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jgjessvt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uzphocht.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lmyxvgjd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kmucobzb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3sgsoqzjk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xizovkih.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3inpyysfu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ukyqcyoy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3itkyakka.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wgzsgcmv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pdzdilja.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gxilqnxf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vgmnkzuz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hsnjmmgq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3upnoddjx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cndwgosv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qmktgrrx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3cyestmed.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hxmljqem.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gqwhzfet.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vbysztcf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bhbihyaf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nnyxbftc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3czmkvxok.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3udjomvrp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qaohkywv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3njmqltdu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mnyvqbgk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yjrdqjvr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttpylvcw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykymwffh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wullkxrv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wfnvrbwu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hcurxvhc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xztqceme.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3kaipbkhm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3myhxbayn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tpmwtgym.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyhouyxc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3zdwjblic.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3badsbbyr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ropqnqjn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zbogimiw.html


<!-- 参考信息 -->