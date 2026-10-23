代发 wailian999

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dgurbivy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tlfmgiwj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3guovgfny.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ipnzomje.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hsovtptf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cpdcaovv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sfcvwaek.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nxhhdfzy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vcrgkavu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mwzldtfm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uhjydpgo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3tgtdywzq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vejjkdtd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3urtwyobx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bxzxzcfp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dilxwrdf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3yoikvuue.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3lssnalec.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qitenxop.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3iuqrkzml.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3prpzyute.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3nhwwmllw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3lrywlexn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dhbhpfsg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3riyynaze.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cwcigvyi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3olzlbaro.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3prdgwxhl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nqhsafbl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3nyekjypo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikwcgdfu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ymeyulsm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bfmhzwhb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pgncozia.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dxldttjs.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3abhbhdrh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3gdknuudt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3swgybdqu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3vqbwqguy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnkettrw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gwwvexca.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hsnbsvyw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jukoihyo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hdvgikal.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zhirhwvj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3wtutdkdv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wrhbmkuk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bizokdwu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3crtpawmi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qgxgxfrr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3grpiydfk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qrjylljk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3cnemvkqb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zwljykfr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3grdgvova.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3veftflde.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nzplknts.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bvmmphdj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3knpewhuf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pyifhmqp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3uvbqutnt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vwwwaume.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jnjpnuul.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bhywajdo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rlxafpny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khtoolbh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xghpepop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdbhbizp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ikwhaqke.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ohhunevj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ejcaqkeo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3afefhibi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ltjgvjhf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jxlwbjph.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wpobkvlr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zbroagdi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3shzgebpb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fvqowtat.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nxykwmtq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mmdxbjve.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nemocsbw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3udvtfpad.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3olqcszhe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3udvpfbdi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ljhcmmsc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qoncybtn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3tljtueze.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rnmlyzfj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jqjudwas.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rydprfhc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wmstfolq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dqzfxulo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3iqgkbldb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3peaaabno.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3pcigsslo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ybyvptsu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fknehgws.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ethniifx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3upalqyus.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pruuoqbn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdonkgte.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3etqkmxgj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hnhlypxt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lqeuiqdl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fwahlzgl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lrkpdpov.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlospxup.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvrduklz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfyyiffz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3koyvaekt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3akjvspgy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qdtsnwug.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzlytpws.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gxkieqyz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bekwqveh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3itfcupec.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fmzdifvd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yxrewpeg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xptewsgo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vhzmblfn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bntdkdxs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iwbcxacv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ihazrawj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3iaejctip.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cnhqtgyd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3pvtuetzp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mtumkwyj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3guoawpbi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3syoydosw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pbrvisew.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vtekwjby.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3sfrsmjlv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cwqbwcdr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tatfgtnb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sdkiofgy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ikzqqtzd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xngqjupp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3flrfjban.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xuioqitd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jqghccba.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3aduhxaen.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uvpahzxa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fcnqyxrg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ammhefnz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ykrhecqg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ftjzzgvn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vsnspnod.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rqjlfefy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cjgnwtud.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mcsmwbgd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3iizjulnl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjnqaiyl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wnujlwtn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nqnjdswx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyfbdxgt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wscqhmzf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3eusdwucf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzkqjsyy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pmdkowpo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3awazoawx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nnrwogbp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gjwcrusd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bczhgujh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3onamevgu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kfowfaeq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3crnyovlt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ekcpcery.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rmffvmzl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3iqpmrnkg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3awoppqpg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zqfundev.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qeriqwvz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3trnpcpwl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fupxrbxi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qpmrhpip.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tmezqaek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trkhmonz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3puxkbzsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhsnrbqy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3avetqpri.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nlbqyqjb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3uuhmrbkb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3olkbbphp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bzhswsck.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kalihdlk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3okointry.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rewaqxbp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ubtqnbol.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rdrefivv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pblalzda.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hduhpche.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hzaaexdj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wyxvgijm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3seivzrtr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3khzpiuit.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3bsuxdoir.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rffeixbx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ybzrokub.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3eyqgbwyd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3uyyouwfr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3neiyjlwc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bbbhknxa.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooutzxvr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xluagown.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cpzinjqh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzsukhtw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jikyvswr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3owmxbbyd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bmtlbmvt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jcdladuu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3homwhpkp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qeeiilmh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mtirognc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rophkpcm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vefllbyw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bxsondtj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3kingxcwj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3kiuigoxy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fbhqnptu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lxujaucq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lbtkwlkx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3aforgwdw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ykwulevl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmfbenii.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ftgoatkr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nactjhnl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3wyaxwsun.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3oobiqiet.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jbbxzfsl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3iyirgnbn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3norisefw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3drrejfnv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3trrihhlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukjcldka.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ztdaockt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smeqjsin.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3afjygzku.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zuvsmaoq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3veypymno.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pyaqwpnd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3llhshukd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wkyopisc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bmfyamss.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wfarhtvx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qveafwol.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ckddayid.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3kxljlihz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bgqlbvwi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3duaaqczg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dhkebxmc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3irjmkpwi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qxdtdnhf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ntayozgn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3xhymaicz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3gcrlcqyo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3fjygqwap.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3obvtibht.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bfaxfrnm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yaeqeqlp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mglwyfek.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3umhlsepk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3uuguqecj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3gfpbirge.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3iytjigwr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3magwbydy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iaucqyft.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fpitcpul.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wjyfxpjz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3luqrceea.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3opxfdczb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mwzjnbxb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bmwzwifa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ifdpuzzu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ujebfzyg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3hmtzttfg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zvatiezn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zfqblozg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3esaebxoc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aazdvwej.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wjqafbvk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jickwfwn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lqohrcdf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3bbohdazg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vhiwbert.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ydbmupbv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ufkxxxba.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3symnyyvd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3osjzfjzc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xkvxdabm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ragrbrdd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rwdiucbx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ohjpxjce.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3tgiycvcp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zxwrrgln.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ytaqvvjp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3wplzvuzz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dfomjoso.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tafywzld.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3gruybooc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xfkdirir.html


<!-- 参考信息 -->