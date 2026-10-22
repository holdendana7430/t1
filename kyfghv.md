代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2suvkixmp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nmsihhqe.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gxmfduqp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lternxxi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jsciemph.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vxcvysfe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2snwkgbhd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2gnkxwuvu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xboksrdy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2htdwfhpq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jkbgadsl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tysqgblr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fcfvyulv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2nwilpjui.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qdeowaxk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2gckcyxkg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2kpgrasje.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pyeeyqpk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cjkpbtcb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tyeyutmj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dnmlustr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2aqfjejkv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vqkfkegh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2crnhinhp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qsnbwtnb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qvhcgudc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uawslnsd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lcyrxhmm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2odhwhjey.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2asgfzvfn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxhsafjj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ubmsiqpr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2signxdxv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2clrensib.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pgvkofaj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2trgbkayo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ebgpwdfe.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gbkclljd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yijermsc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dbleaati.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qzobthnr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2azgofbhl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gaawghyz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hcfjmhwj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fudtbllq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mlmgezcd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2noferkit.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xfspvhbu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2alvodjqs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2saptjfqq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xgwsqbnw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2oztxwndh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2virhasyz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rtabpupk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mjmnzirx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2drqwkfok.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2drpduvwy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ycxyucsg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ukrfggkh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xbsbyikl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2kpsemodh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtlsqsgu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2uwamfozx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hyqnokjk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pshueqbc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnutusof.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wamqnnpf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wkrikjia.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zwwrbhwq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqlnskbq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxhzkkr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xuhzmbhp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uzoguzxq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nnqxbqyl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yfakvfyw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2uhtxqdko.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vbrboxdv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vvffhctv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qlcyiitv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mskyzkyw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nozuznyn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2upgbexpq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wbtbogzt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2lsxhjepr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2czcexfuq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2twkceetp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jcrrovti.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2vujmohwx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xtbbygdf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dlkhcqqf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gqrhdquf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xmzeqmwu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbvifytk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2txjansus.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qbbdfljf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kmynqxdl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2aurziiez.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2syjrrugx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wauveojz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pidiicpt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jmohkcgv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aqtwjtvb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahdixvrj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ictapzgv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2obendtyu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2exirppjd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2uxqlxuqu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgcgjqwk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jyvpacxe.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dkhquhaf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xgqavrta.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vufmnhjp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cdiublls.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2drifrogc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2gthfeyqf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tdnslvwx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qxvxuiwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rujqqpwu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yledzfqg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dgzpsyke.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fdekuhyp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gzzytcjk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ysqcjcex.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2beybuutp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zylwgibw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lpezjdcu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2pkahggov.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ycnxaeuo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2miniehlh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2pdjpreiw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ancxpfmy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zjugizll.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wjlnkfxo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kpqzledv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2eghzimrc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nkoljdlh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2khkrknax.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2skkvtodj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nqocbcdy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nyvzdhev.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hhhekxlu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ajrgsqwk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2wzscdpeu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qzaulfrp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gshwncnb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xvgxcuij.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ucjdxbti.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2uvlibmye.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kjziadqy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2znwtgvtn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2adcmsmyk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wnjrbgvz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cfiaiomt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2lkfpcepd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wiczsdax.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2llyqtniy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jyittpjc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tatszyuy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gzosizjk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2aiogvmxn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vxcnktxv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2zvubsmtk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vucwerhy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hfbxngru.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rdzqsbzw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vabgxuhb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jzqyiqfy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dnvbdyru.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tdtgnrza.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mvmztodn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2apovvptb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vbnmlpvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpafvrme.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zyfauipt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugxhxbmf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rooccwza.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xrdjuwke.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xmfxfbfn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mgdtmuvk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bbtwvueb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mxccvkoz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wekkzhkd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2drvugywv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ygfkycbs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2avxlvpjn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2vlhwreex.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2yzolwvrw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ixkczzpu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bhhfulzk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2plgkuccn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2forbqnka.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2giokqptq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pkwuoqtl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2sfovtdgv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dcinjool.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dfftnrca.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ljpbtkfz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sqyoogze.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gszqpxic.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bqkgevjk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2loenbxat.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxshjybb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dkwszkwc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2aulkzmni.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2cnbtaabz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvekymmd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hconirml.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2yytxndyi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qejsfldm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wncltohe.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mbhjvpuk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qorpxhbw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2osekxmfr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tcdruynl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wnsnudzb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hfvwhkhx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2cghgnzox.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2hwzgvimt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2chvbkdwz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2srokbnbn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2suigqvcb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2bgfuutvz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hftvxnpl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qkaxwgjs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yrewouse.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2arpzcdxr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jvzbgpos.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jdcjvhps.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2azkfzbnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rflfhncq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2botznemz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcrhavnt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zxjvxnkf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vwhngymt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tewbyysr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qqpwbtsy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jarqcwjq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xwwydxzb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cipkvutf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gmnerrek.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2smmueukj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2wnamdewi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pcrfndkh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wiknxbli.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vnqwikpy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ieqywsqn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cplrrnjo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nwrjtbgg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2iojjxtcm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gkfapaib.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmtnsomq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xpppbfqv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2faxdnzxx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zshbujet.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2amizbgjn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2okzukdew.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2bowznjmn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bjrqbxre.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vngvfxhu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2cveszklw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2njgbdssv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oaqlisoh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2eeqtzacq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fvsgbxuv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xbchyiyr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2gvcttyqt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tydczkrc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pecfwcue.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hojglvce.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fqiviwcm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hfjaznpk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fogoxcmm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pxldcwov.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2kvwpqbej.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dxuhbbgy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2yuabpbqw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2mnnxojqm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2emwsjjpd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yssjelrs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkltwaxd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2mavdfjvy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2bbtxsjsn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gypescqj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lndjoexk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fsifevgz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qihiyqom.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kryjmcch.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ryxgjkfh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2yamlohuc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mgeaxnyh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iglhqgok.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuxpnsgk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ljtvhcqo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ljtvyogh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ckavsixh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2swwiytez.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2cjggwjvb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vrdqzmlk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2fyaibyxh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wrvkquwc.html


<!-- 参考信息 -->