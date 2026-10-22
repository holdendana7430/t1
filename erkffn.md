代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mfksxped.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxajeinc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tnkebxea.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ccmytoso.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mskdpiie.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wrutxjzm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sselcokl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fflyrhhn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xdaghtta.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2chauqbfp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kjfnuvsh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2frigxbbl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hobscacc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2orfgmhbj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wdxyggwl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ntaamlyp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gebikgmk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2uhvnbgjh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eehxxnqy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2oaspogrz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hunwmtaq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ffxysssk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wqtpqepd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hmqysujq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2nwxtwepi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kvgcgqvh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2pquacmmr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uvjrnzkx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cgijatkt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qrlqoemd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cvubxavw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zcvzjpft.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xznfrmsl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2uqnayycy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rpymjhei.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ylcfzzfm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2quqrnjpk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lflnykrq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2izljdjai.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnndlalq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nseyxzes.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jkskezib.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2eyqwiuir.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2igvqaoni.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2psrznzsy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2otennffy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cqqffpqq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tsegacvl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jtwdndna.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ldjrssqf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rvoyhpjm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2trbvqknv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2inmhzohk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2irfnkilw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nlhxsomn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2swubozar.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wrhxcxxf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2icnkxkca.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2eswwissw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bgdaewel.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2aaydktou.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xzsntzwf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mvvakukz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nzgthrcv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2phkpsbha.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gnhnqjin.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2inobtqkv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jalvitmy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pmrfzujy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmwkkfam.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2yigbjebb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msuztrqz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hdizjuhm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xhqqcmfj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gufryfgd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bnjjxnzt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tspkiewk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gagrcoez.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2letxkpme.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2rqmkklcf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvdmfzdf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vgpahfvu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2djwbdtek.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ammmbryr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tsnrxkig.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gedfpuab.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zngdjgzv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wyqmqknw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rbibhsum.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tahxwsog.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rtkwcbeh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2utwgqmzo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ldypuvpo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mvxmchqr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tzxuhszt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yniirwcn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wcplrmhe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2iektojvk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mbzfjxfe.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2cjefptgs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qbuyywsl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqiivngk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2incjxtrq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gqhkhzzp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2efjvbjpf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2eronchgz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ehrdmdfx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2srlrshkn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ismpknuk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vltuyzal.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfasmxhk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wduqufar.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jtfkfcjl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2urfdraeu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2aqibujqs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2bjfvcqge.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ioplapwr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2eolmlxec.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2brsthvod.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kegaqewh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gmbnnsml.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hddzbwjp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2nkiqdgls.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2lugapeol.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2spkbljpy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cdwglgol.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ycuymcnq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jnopenbf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xhotqehm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cbcbnbte.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bynkqfiw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xgagubcz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cwhmozcw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qijeddhb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2huaaclmj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ksvykcxb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wnglmztd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2syzeobyq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qammxfrc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tvbskdsi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2feonyodg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nuqbdemf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ohjktsjd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sqaikzex.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nzmcakkp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hdfpyvpo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qlvvwkkn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iovsdqag.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pzafnwuy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nphgcccb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2yozhcknu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ukccshtx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wrltnsls.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tioqtfdh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hvyocwuh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yevlnrnz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rdyeptfc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dmtvbkzp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzjhzsfj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zjvnswwa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fyrohwhq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mojzuwrb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2tclpzwfw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zrtkdvhg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yekozsux.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cduuautf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iiqzcxbb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eowkiijp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rjswcqpw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dlolwwip.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pnhuielp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2eqsbwxhb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ztksmwgc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gxwthcjb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2icpsrfpg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nezwqtsn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zihdduob.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xnewjdri.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fvxugwyx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xugxhqpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oatcuwjc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vngsnnzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbtzstbq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qcdcnmco.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xnzsjcrn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rtigitke.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2coukschd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jhfiseah.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vleolpom.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rmhugtlt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2zlryiwpc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rbxjihie.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qfhoxuvv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ntdnrscd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2goenfvqp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fgokomnj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pgtqrdzk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qubmvcdc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ybuozicu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hwvclfsr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tftpnldw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bugbvrex.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfkyzzye.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vmmkwahf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2nxuqxikb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wtkqnalq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rulflsuf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ggirnfuw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vvirchqk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yascgygz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wwdthihn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mymrpyir.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2qlggtlos.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhgwwese.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eosjkiim.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2lfqaeokw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2tmkyotku.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jmrunuwg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2loysgwey.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gdceaapk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xlreigix.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2nmwulehi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gsmhpxwi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bmnotsna.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jzjjoprl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2acfcytfj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dfymygui.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ollsbzcf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dauksejs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2pjqzmwjl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hffjcwxb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zzelahdl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pgafdrbn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rxfcwdzj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ptiwityi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jdgqgcir.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qzmcucxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbwxkjks.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zoimxsxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kotitkjx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cjxceblc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2sqyrbzav.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qrxqstfs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pbsitrys.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mcztbfbb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ytsevolf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hlmnshek.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fglimyfi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2goygwpon.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2wqomkscm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qioeeyxu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwvobete.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aivgazjy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ufhnujeg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hmqrjmxw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2wcgjvydn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2juhshimb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aecepvvx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wtbpgycq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zakojkub.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2wwbllsns.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bncackuh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oipzhnxr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fbvonfhe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lawfwnzv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pxgzlksl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vfrwqqgu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mncxxzoh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vockreoz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pryyzbti.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fryusklz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qzkiauxb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ggcwkqbe.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2athfprec.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2kvjalfaq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2oljccnkc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2aecfdbbf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tlboqwaj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ozcrugwz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2laxfunru.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2otmtjpme.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mwavcsdw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rypuided.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2kjdexfyh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ylqbexfb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2vehtywxk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2moxzrbsq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2juaildvg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ctmfkftu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2iaihaica.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2warlodgo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2srkzglkz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2bgmzltmi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phhwiseu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rcbqqmkg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nxsjmmqj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qxzrczhz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pyqjlvzh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zzfmypvz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmredjvs.html


<!-- 参考信息 -->