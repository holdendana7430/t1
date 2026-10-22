代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qsmuijdq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2usquowdn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xzxeiqsl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pjaqrcrw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xrlpqxgn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xtzrochm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fcznnnii.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cptxbsdf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mgmgsydm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rgvijccs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xwouwogn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sjddzcgt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lyhwvzuy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tyfnjlnt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nwzfnmgw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vnvppwmj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lcydadfw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bbongrdm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cjapmjuz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jlwsilnv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2slwvgnmg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gbafwkvn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jyfnidtz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kzavxiaz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xgjnfwpy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uknyxcmn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2icmuvjmx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tetnrjzh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2htglnmdk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gnsbyetw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dbxbksqq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2axiatcgu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmeypilt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hqhragir.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kjustqzi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vqyctmxo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wyzoghkz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kvcdkyyh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2wjulozwj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tbgmlori.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nmkaweck.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eipcbqyx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2egbyypwf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2twvmwrnv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2moqzqynb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2jelotsmt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2phsqgyuu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2roscsgsw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2folaqkei.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vndzvryl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qfynsoaq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pjedxmqo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pvmaglse.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wwdkybej.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yybkwbsf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmozdsh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vetpynyl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vljiortt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nkcbpzxm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hfyjtsaz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pddjmqbp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qvtwgqbx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tmdybols.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wpwnevou.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yrnvbnjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhxhoygx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zstazawi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmvaozdb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yxxvaqgy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnxnbdza.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hkpboelw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hpvlrmga.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gnlknwxa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yvhqqeml.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mszitywr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2cthgptfe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2easncerr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gazztxjf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dizfusjs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tvztxebp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mvybfeve.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ahcsojaz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hoguwgvq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2isstriys.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rmhgvmvi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jidlqtkq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2uhoztobb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2txvovedz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2zmbxwlen.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pvwzhnuf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ohzmirok.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ndckrsap.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zdeorvkl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mhwljnnh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gjupottm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2txojurxg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eghlswas.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ohfzcjob.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ebcalxae.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fvaokvhn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqgjtykm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2adpttcfr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwuclrgt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ubdxunmv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vfovpzbz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2knunesvq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2huswrxel.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqeoinnv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztphqxaa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ocxxmxek.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2awbcjafc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xftaundj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2qitbcpjy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rlyndozv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sbbnviju.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hkkadvcl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zebfzzui.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yjbtbjur.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yhpmrekw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2qhjxekhm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lqdglwdn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2iwbyfdms.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hhidgood.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zhdfosvd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qfdtpsey.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ihvjwpcc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rjsowmvq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gcusarpc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uqknnoqk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rpxblmnf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2oqhebfvm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2accvfsac.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fkiyqevz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zrcnzagf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qspymhbp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wemveytx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jhkukcim.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aofchrba.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uswsaank.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yytycdxi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kfgikeau.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fyenjgbl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rzcfanjh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bptxyyxi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2sjadlejo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ftorfcog.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jpvccite.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2oncwbktn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2evybgcie.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kdwgbpfq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2sjbausuu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqferixk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pqnkctre.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hzxxxuwd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlbtyfsu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kszejjnw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ycqnilxk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mltvxjas.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jfwzdcii.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wpofwaoa.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddkkmewz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vxjmivlc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dyfosblf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hdkyojtj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zrostfrr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qmysgtvi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hognmksr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hetviyut.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nurlwqus.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2uxmsfvub.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kxzixcrb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kfvrzosx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vrzuhwzt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2xraxuwav.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xkwupdup.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dzcppsal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvtbcgdv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2viduotde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekuczfqw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ixkhooar.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2krshnwtr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2cenwntaq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ispgqnan.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dojvvsjb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pywiueny.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wzokftee.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rjoxrrrh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wmoyiyee.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2cibxotlo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fqtpouji.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2fsevocbc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qiutsoax.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wncowbob.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sdzkeidt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2msygbezx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xoyngzcr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2umndoeqh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2bveviyzm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2txvhuyzw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qcqcktas.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2stkghlig.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xiunbvqp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nydfbkoh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rjzxjdgw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wlpntyeg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cucrexvj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gromvnbv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hmspjwbq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2thjwgnel.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qdvpjdws.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xtohrdeb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2owhbzjwo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2egfdresm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tbzwxrek.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ckqvhixp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2iiwmkect.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vyxjlbno.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2iuvnkaan.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zxqhwibn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qesetiqu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2yiwcktgj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2yryinyjy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mvxqqcdb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2grtjcdmy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qmyljxwl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2uhxalinh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2lzhwtrvn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kmgqxzlg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sqjqeqkm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gkjzgknj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2aukxryoh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gkffudyn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vrpwxmrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zeocsnhg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2rqfymvgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nznzkhng.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xiolfhwj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2eedhbllk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2glbeblng.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gtqpbaku.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pusnskhm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2crogultf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zghgorjm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rtqhrdla.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yhipwhdt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2bduxxqxl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hcbctzaf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxmlisuu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vwcxyqqr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bsfwsgsr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pfhfhwwh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2tzoerwvb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2exfplqfm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fnwypkzj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tirqjxqh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2yhgwlkge.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ofkxqpht.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yfpoxocg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jwuqzmuc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mwtygujx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2sjaoxyuc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vfgfpzen.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2cctxpnem.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fowwmfft.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2agrnikwx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wckdvied.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2srwufgav.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wpxmerjy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2buugwjft.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2hczyjqww.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2gknhxjce.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sbniekhg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lcrazmqx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hcvjungd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ewyalwhh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2mnnnnmfi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2epmhmhtw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2lqgydswu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cubvscil.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vjmaurvm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ffmavjvv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2yadihjdc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2fupbzqrw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sczyjmtd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ssieejng.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fthmjcvi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xfppnamk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2iudwpmwo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhwomdn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rjhjmmgk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2wqytcgvf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2cjvtautw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2adrjjikj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jbtrrggw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jjnybycf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2cohiewyo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ricrwizs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fdsadwcf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2danzuldz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2fxhfpsxt.html


<!-- 参考信息 -->