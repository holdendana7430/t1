代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zcbpxwgy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gnzaqpyd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2enihxmut.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2bxvncvmx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fxrgexwm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qguqwjlw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mpbtpayy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rbifqecq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xyfxxkln.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kxghtmbo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fkcfyxpt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pqzsdpwc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wbznufxm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2veamelng.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2imxkamly.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kjpmuxbs.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dddwofob.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rpfwemgm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lfyoihea.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mfwkeuum.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ksqwgfnq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zwipfjhh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xszsyxwp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xsepicas.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pixjwkuo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yfcectyj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzigkjam.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lvvqlwqz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2piytayzu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2whahbafc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2eprsacoc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qavgkzlp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zcvqmbsd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bdyxqmlf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xunknkno.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cbqanlfg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wngsryly.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2acimavvv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2svxsmcbz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uxnrmzge.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2taxzxfyn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gasqyeif.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uebrkfvv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nijcbtqa.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2sxqcqsmt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ltxfuygz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2wpxwkbid.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lbtlcfac.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2dfasrfyd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ygjdckok.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cqsgcfui.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xtlnbxne.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bxancvym.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2uprdxsvr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2firemwqx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2igwwkqem.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2myukuooc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttsumrkg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jzgfwuew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nugavykg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2scmkiuif.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnklzjnt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aqretmuv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sqmfnaxq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hawuwaqu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jwtcvrgx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mjhtqmfy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2kydeavmz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jabcpzcs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2yjextizg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2frhjemxu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vduwkrvt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oiyutmkv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fxgwzobv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2skgevggd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrkvegdj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gmbupevu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ephdggfg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bxzuifjy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2oqyflltt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vljtynjs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vcqbhdzy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2paqmpsfh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xqoqcevf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2izlmfgzy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2cxrkdvei.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2divgakzd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rztxcfqh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2czntbcre.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kzahrujf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yirkbjba.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2evfydsuk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bjutfqwm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rupagdrm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsmaabbx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2asodwypj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xebzthsk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zbdnfiia.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2sgoosick.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fjdtihay.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wnlpqwec.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2giwfwlpd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fdbgjtxt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kqmwheqf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwytormp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vtcqhhpi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zmpsloec.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lsplftrt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2scnlhxyp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ncnkojls.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yghamvim.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2llumnjso.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kkirvlfl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zkstshwo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2oodhkulx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2nqnujika.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gymejlpt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wvkybjim.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wfisofrh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qswoqmdg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rtrcyicv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2duccypxd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uxhkzftv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wzprhugt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2epaehjii.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2auruzspx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ztfcyigv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2chjxyior.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2psrfsexd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vhoeqjhx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qmgkccls.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xmpviuva.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pxjtxwqs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nlwrxmbp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lpntdmty.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2oeygwrss.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2diydgldp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zzyssasm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nvjfyqmp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lqrjujcw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2adychfcn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nceyhmxg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gqpxjigk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gehseion.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kplaiukq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wywopdok.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwxaeyro.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wgtooxpz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wgkrohzx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2whdsyduc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mkmwqflm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2qnhbjwok.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lzytopuj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jpvdpngj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bwxhshlt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eulpfrzc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ajkrvwzs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2neixwkux.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ztfqbckw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2urzwjvgk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xiyjlggz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mtqcdrzy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2plgosnbt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dlftubsy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vfadizyt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2nootxotd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vinbryvm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oythkiam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohgvihch.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2aqpoihla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzuiwbug.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ezwqqksu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2seohcyww.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dqysyakg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ushdctrs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2izsothkt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fuwoeanq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fzzhjcrm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2xqfctlcp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2laprykqb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2txxexhey.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2kearyulv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2grnosylq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fdhnndbv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2muxzdpau.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2bdzwslsr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bymspjif.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yitvgbqo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vxyzphoh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2jpjqrlhq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hqyggtgo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zpcgqzeu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hripmhol.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mdblrrlp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zglpzrvk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2muirtfvg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tszcagpo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xelliexy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hqlupmnn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pkrcvajl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2abcrjixp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncrwnnoo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2njmbedwv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uqthqveb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2sebhuzub.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2tbvpoarx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfdacxqs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2fayjower.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mnqbhbkc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tdgybwkf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uvaphafe.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rbcarksq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2svvytwnh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2rvpteclm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ultwatyr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ypugutrh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2napmskun.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qiayymli.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vznijgbw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ryauyrra.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ugouorey.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qmairubj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wbjsxesg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2hkfkpigh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xzckxudn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abxylajd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2inzgxybb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrmuxkoz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2urixqjlc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2iyhqwfrb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bqzuoiee.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jhwkhnhn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zeeeqkyl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ywyftnoy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2sskwazkv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2pjmzvvun.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xmqshllc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2lgmhcyie.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2byipvfwu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lmfgtalr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gghlwabj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nunegwcg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hgzkffwb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2gjbmwkxc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qabszwcv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2edaoontl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zgpoiqhj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hduquidh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cxjxqlrn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uqmqvbys.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pcllwqdx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2kzjhhxnm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2grwedwkb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2spdltxee.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2iivohmmp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2erltljog.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2enppmojj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fozihttl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zpagfhvg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ghwzvbei.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nvtqyikp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2hbnqrhgc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cbfbfutq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nhjlnnlb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qjvsmstq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vcfrkwku.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2urctwlnv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kynradmm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zlihjpmv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2kwuqbqmb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ewyzdhbs.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2aerovzus.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2teuchact.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ytpmmbmv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2swgskmpk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogycjqzt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wqjizmol.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcxohhsi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lrgfgcmh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2nrzmmnhx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qymonofo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eihmzwhr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ffpqjpkz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ecttjyoc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zxebcwdl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sapjygbm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ppqlnoem.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rmtfjmaf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ojiunytb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2engmhjnf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wbkgggle.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2tcaygtow.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2fqkjvzue.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qicgokra.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mtaszgdc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2feerivzc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2rgjmeuzy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2nencqdbu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wppeysgx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bvpuuhjh.html


<!-- 参考信息 -->