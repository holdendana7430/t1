代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2euaxhizd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uwetxtil.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2etpkffbi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gqqvakvm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zukivser.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pityhumb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cugwktce.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2fpxenqxc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pwhqxbas.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2flpnrmwx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bfqiymhs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2scsvttfk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2qjymptzl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2eumvhhqn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mimnhxyb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xbtfovya.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vkiugcmh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rhnzaace.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fldkvdlq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2juhdugbu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gdjhrkdb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dempfifr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nsmpzvmm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2plwloclc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wbamzljf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yaytoztp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yxjmyjjo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ujkrvhtp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vkcuiwij.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2izlmifbo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqqslprd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xtfktwwb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vfztlhyl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lkmprdfa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2opzfbjoh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qwzyzirv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2asifwqmk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pzhasnmk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vfaysany.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2yqdsluzv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wssmgeyg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ddsuvryh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gbmovbii.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2npolkudv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cfsbwnfy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2aooeqweu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ohryudwe.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cckelqxa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nlkwmeao.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2sahfkrma.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bjnmgszl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eudahath.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2sjcvskkc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ijciilmy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nzvwcqba.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ercmqjkf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kbtsbhsr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2foswbilg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kvtwlpfb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ernslvna.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wuovyikd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llpnzjkq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kxoquzhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtzzocti.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ddphosoh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fanufjgf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dxtasyvb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vdluhuaw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hkxjmfik.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fhlpvxdw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eugjlpnt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rrlmcgum.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxaslfdr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ppxmteih.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cmzfvzqs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lyxwyxwe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zkycluch.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zzcqjdhr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lzapomfe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tyfyuvwy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wxqqlrce.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ijbraxmd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vpdodhgj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ctvcylzv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wlgcniaf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tnrtialy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ccjeikdr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2iiccdsqa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2uttxpprd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2mwxywdkz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ooopafjo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rkyxpqmi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vbbjkavm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kpmgznmn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ylphvwvw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nlkfiisd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fcztsxca.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gbrcvwgu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2luyyqxlp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fzmosbre.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2netibxtt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ucrnwtbe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zjzdhpii.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsbpuadp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wlkjrssr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rfhemdlj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lnnstiaz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jhuquggt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2lzehchey.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2njpxcsif.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ggdrjgyo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2amezdtyb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iklalhpf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zlrzqkia.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2cjevqsgu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jvqomsif.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bksdmynz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2huodkmag.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2akmzuhdy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ybpdnukx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ukjycpil.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mtfhkohy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2eiyaceam.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2krvmjaez.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zyojytig.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ktitnnbv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2oyuftevs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fvfifhvh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbiilolt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cttblmis.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ahwallpm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xkwwdvql.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ivlarebb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2szinikjn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vahqrwfx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2btcrpmoi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xyosmtbz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vztoyini.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wurbkpqi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2whvyenhq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2csfqwpad.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hlcygxnq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ocfzxpwo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bnbcoenq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dhoruasl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2woxttkvc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ekvdnkmv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytapuwxr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pxitjyuf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ysouumye.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wqypgtqs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ieyaeemt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vjofsnup.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2swwvmzlz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ienptcnk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fybknwjd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wpvymcvd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kdfyrdvp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2grgjyubw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xdoubkcp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rqhsefsz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2wfdeqblk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xxynyasi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hpvctbfc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mkltjfwf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mxzyobav.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wxtrqzla.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qlrmiarw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2faaymyli.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2oyccjacc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ssgxvphm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oeajqaag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2supbbsnv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2aujwfgko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfxaxago.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2usvydako.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xyqhcght.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mrjgzpbw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kcprkicf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ktyjsowv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vcwhkvbl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vdrnppfv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dnububwz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xcwkjysl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2igpzgkxq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2crumuaij.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2lrymzmyl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2stfamhue.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2peqyrgcp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2fpigzxtk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jkzxikok.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2esjqrkka.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dsrdrkfs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2urjcsybp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2eqfbsqmh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kpavzijp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qllxxtrv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tuoaufei.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tqjaourh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tnucdbpg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bkrfghfy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2icxuujrn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2enwregfp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2beduropt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ujjsicuz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2brouazrn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2eeoxsumv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2pjelnzzv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vdohlpru.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2eiakexgg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pizguyzj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hvqrukhv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2puxvricu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2csbrqvhz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qgrxumtx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tltmidws.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2webponby.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lztunzce.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vxzxjqty.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xuzvkhan.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jnujqvse.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2iuxlkhqr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2yxxdslke.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mmommguj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tcmjnmxe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ykjqlbnw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zsjyjcad.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qdfditbz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2zvblyish.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vaktauhu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fwyavfrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2optihnrn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eythtyif.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zakjhkhz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xhdtsozq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hgxblqeg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ixuihfls.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tbtlvcgh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2bajvpfzr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hbltpgym.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jxbgnkyt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ngihiroy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2orlyjgqm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ltqaaywn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ccothtnq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mtwxuytq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hqsigexr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ngonlflv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tsovihki.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2sfgtcnxx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2lkafulng.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2emebjtxj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dffbdrmq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wqpdiuab.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yssmlhqg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mzeeicup.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nvjgbgnl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2qbaezrvg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rhkoqlgv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nywpsrgy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2dqnidgwd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2niyocdmi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jigwvqtl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xmtvxfmw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wqgukvij.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tocfqrai.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ynemwvml.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zcyjfwlt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2owumbjzz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lzripfyd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qmoxpigo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2spxkpdcg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tphuowwt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2sqhnppon.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wlwsotjp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ysbtjpxl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2cmgrodvw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ruyydaca.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mdqjgfbi.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuaudlut.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2elpbyhbc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzoopyen.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xmbsibbl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yljlrpqz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2otnlficr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecnqauss.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qetazwqj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jsjizkwc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2eivswwka.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fyeitwlw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rahbzjye.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2grjcfgef.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lgzhbxai.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2smauixvq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2pbcyaciq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jgjtofnm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vzamqonl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cgljmsxb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wzsthicp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwaimuuo.html


<!-- 参考信息 -->