代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrdcejip.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwvzlxac.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bmqpgrrr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xtviklzy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2amvkkwav.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2osmwwiar.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tltisury.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2shnxocrk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vuskycfk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fkvzkcru.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uycscqok.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gutrxciy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xrunfsaj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hbljmsui.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dmzfxphu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zwatgorc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2diofjyzv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2eenlfuhe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hovvwxai.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2weqklsii.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ukabdsdr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2tlxwnoce.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ghbvxfdl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2upoqtxsy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2cxwcljwr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rbikvxna.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pseblxcs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2egngeekc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hnrreseg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ewiuivsy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ticxmrcc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2etnnegyy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ilenufje.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2iefrwcex.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xgjcttsn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nakxiequ.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2avnubqzo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ocmjrxnt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgwuedyo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sqpfvftk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lsulhdmt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hpiqapyw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2exyfbaph.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wixelvnv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lhozdzjt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zztlzckb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kjsxzzmi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rstuntkf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yfqayfzt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mgvxarns.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dvtdjuwo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wjzgcdpe.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nwvtvenv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2svvsnvpp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zbfpbicy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rztoikuz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mvbgoarh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2eetijmrj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pqilkhdi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nwvxbauc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kwwnwtww.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2enhvuank.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wnwugjwm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lxvfmdlk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mlcbogzr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ocomqvmg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2imriebvp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xfemyfar.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vsamcuhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocynbbep.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2tcrucxhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yragqtft.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nynmkuiy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2olhjmvjy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ludpyxpa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2thwwwsky.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hvzofmmp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hugzjcic.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xpqyazqo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xlmzgcdk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2egeqaxqh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2poiozjxz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nnqxfbfj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2iupqmrep.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2daudjdai.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2agkmbgkc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2mshdbidl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ovbnpchm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uoqiegrl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vlgqkgpy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2msulzcct.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2odnhkbpt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2uampityq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wtokjcve.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gbrcekrt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2opfpnsyl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2grqepwvl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wsvbqskv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wmelxkah.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cqafbywu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvdiccqs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vgmefzre.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yienkvcw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gvyiprmw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwatdrix.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hzwfxjji.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oawghtxu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2knnueshj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wqblrtdw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2iwuolbaw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2evlnigwr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bhkyaowl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2opemssyw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bwimuqoq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2yotatcxf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qnuappkx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mvsoexxt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2cbvujroz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ywpfdcmz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nzhdcqtt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cbkgkgfm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rpijbekz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2czhrhpnm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pnyqpeqp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2umbfvcnf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vpgmydev.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vynrscdh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2sqdzzgvf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wlmpjghs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tlfozzrq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2psmkdtpm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kdqfrzke.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2jengcgzb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wjlrubag.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2noyptnpf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xjovdabw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2vnrqiuzv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ndukmdib.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jnryzjtw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iwnflweq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jchmjghz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tncmdenm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2epnnasxu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wuxemiof.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kolgncby.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fpimpugg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lncgnzwx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hwaqcobi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2slkxovwd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oxgcfaoy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qgjdvqyw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kdywwqtt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2llxfakqc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xigwzuzf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2oixgaqyu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hxndefyt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ifvwovka.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bnzbwelh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzidbpok.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cqzdlaiy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2cprdjzib.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ueqivbur.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2axlsrtrt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xawouflo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cmiuzlpj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sxivdtwa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kztyaewc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hokbxlqn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2apfnsqtm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2enrxvufe.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2irxktgha.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2podoppwb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kweosatj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jsgvjheb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lcbzghhv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rleuqdgi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2swcchxzz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2oqxylzmk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xlemtasg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uhlojdbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqvozecx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vfbfmxqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecpsogrv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2udgmqekw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2azaztqby.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2yyzldoup.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2soazayai.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2amyolvik.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2buvhyzkj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mnztiunz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2horukino.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xjxtokvt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fzxgzsdr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hddeemcp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vqzandtj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fhxuoubm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vkxdrlhj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hpsoibqq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yotxjtkv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2aajhiulf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2axsoivvz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qtxjpmmv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lcgnynsl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jbetxlgp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2websaxwk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2llecgdtt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfibmlom.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lfdjzbqh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2njhyihup.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbcvgktk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ptgujgey.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2khwghggd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2xudxfjvu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xypyvtxh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfcjvydl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2krvtvjub.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yrcnxcnz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2itosheql.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nptjwbjm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lbymnsew.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bwmyyjbf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2tqnskaes.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wyxozuff.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vgonkfcm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mbglpvki.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ikqohdak.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pbpkzmoy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptkscedo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2adtiyzfw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2avmxpdwc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2dpwyyywb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mbkwozno.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vbthogrz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qeraydgz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2dglstknx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2sdmezofr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uerkechn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flzjgcyk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2usidxhvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfplwxin.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wvxzoqfp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nptffmqm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nntncbsc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fodwvbfl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mnhrmzfj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kbgxqllk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vncmpdpm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ahpjiomu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2meozibrv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pdfxycvu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2xlqfbfyz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2pbdvogcc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gtibjxrm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ptzguaui.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2efjvsbuk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qnesslma.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vsspsrae.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2wmdgvfbi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2apvevbpb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2oaoqvkbr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2evertjgo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pwzxlvln.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nstjtznm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lcuieshx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nyyjyzxu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hgbosgft.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jffdjqry.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pkidrlrf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2olgfwsum.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sqxuysbj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cedypxoi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vokvfaip.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hncmnbii.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2rladtoul.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2sujmvsri.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2btabzzmx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ootvfwvf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dtluegtl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ybyaiahb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2pprjjvvt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ytcowskd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gdbvqtun.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2habvvwsz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2stxklipq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2igjbvvpl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2swxgqrge.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ukehhlwo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2forkbcif.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2scoecoaw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2zdlrwymt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2oqvypoxj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2suckjcrw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ykavwciy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hdqdmfoh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2zvulfhev.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xnhicvvk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qpfvgrzs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2snedocwf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hlwhkvfq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmmyutso.html


<!-- 参考信息 -->