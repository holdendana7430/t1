代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3betpvchh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ulsnyrem.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vzdmqjpu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qgitejfp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3unpemoyy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hllamewg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3safiwjeo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3denchscl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kdlfmrhn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hogopmku.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3puhqrdzb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3llrienlg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wgkaumyl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ghnbwuca.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lgzpbbbz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xbbjsehj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dzvxhipu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3iiqyljgf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qiskienv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ierwgqxz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hifnerac.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3agofxexj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pcluqykm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3rinhazwd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lvkryxmj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jpjisyri.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gngvirxm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uxiifkkd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dqfblqcq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fqcvvizh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ijjlslrd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tfkpcccm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rbwafwgb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ehbktqbp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3trkrxdww.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vpctrzkr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wlfxaexo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3foovccfn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3othmxpzk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3avythrxl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3egkwsmoh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qaszngjy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dnvszisw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tenuxfrr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rsqiwzka.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kfrazbrj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cignnjfj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3resjjpgg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ouwguhol.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vhwufzne.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ufecslvs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3alzcyvjv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3cxpxnaup.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rwgnuorr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cjagumbo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3keakhfsq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ishvmcsm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ghcvfagp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xaevgnhn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3tuzntocf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3basqjzjq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3clkxuakl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jblbchtl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yzdjpbiu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hpuipgdh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3putchxgs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qwwhryfj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3phtwunst.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3dqnepshm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nndgxrpb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ydcjwcdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyeqblzw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3khvqecdl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tnjqsngn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3furwrryp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mxfgdgvn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ciufpadm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qorzjccu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uhtymbft.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3dixehigw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3porrsevx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ymrhgbkc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3overyuhh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yeotyffd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3icvzeoxw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3klksjesq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3oykjxmkh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ksypcjom.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kwjykbri.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ujycscvl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zunfrwld.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3delcorsz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dzitazyk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tjutwymt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uaossqjd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pqgaycsx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nnabfiku.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3czurclzu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vmepixly.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3eoucjlkq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nqecsnun.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwiacape.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iymfdikl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ohhukmyg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gsmccdwa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xzakrveq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3elpnyerw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ownofveh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3uopcllll.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jeuxdxom.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rxhuntgs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibrkgfbb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jebfwwdy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pqdsfdcu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pjaleesr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zixoeuuc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ewiqxtvt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hfmudaxc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zketohzz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gdmvfuiu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zxcwgkpc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rcjereby.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pcqxdocz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3tmsxetcc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3woltvmxs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vfgylmzo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3grpexvyx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3uhfqfyer.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3gmbxyrep.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gzdqazuq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zfambkdt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mksybjcl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mijopzdy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ubdpmbms.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3uzbnmeyu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3moiitgyk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3skqrkzsk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ycsbfdfp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ldggfdua.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rgxhslxc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3frlrzmvb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vseuqunx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bleubkea.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3giwippdv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gbqkbhpm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3mqnbjqfj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ibgfevik.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nfpxmtao.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dawtgsim.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kwrzgqfg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3shmxsdjh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3urfxrmcs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qjpjuyqq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vgygvbov.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nkkgfeer.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3motoklms.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jkdyugqq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ubahbaru.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaisbymh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3suwmqwbi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3todfkqgi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3esmytnnn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3glhgezry.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3pilflqcg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3iqkswxiv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cdolkhcb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pqqupvvh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ltdavann.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yywdmitm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wuockeji.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xhfamxju.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bdwuhmoq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hclclwru.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3rlqstsaq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jvaosafu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zrvtrikv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dnpwkrhp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ihfzltag.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3gdbchjxl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yrmqmwei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmbhvamh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3dfbuxwwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnyyugie.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ndfzhxzm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3juuusbsx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jpixuugj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3aavnghtm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qsnivhul.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qnzsptju.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kykffmvr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3sohpnleg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3sdmpdkgr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rwgorian.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dczahepp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3aahupgfj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zsivvpqo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sxoeulip.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bxtjssvr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lmcscljs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zvasvbqj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3krxgkoro.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wfncirfd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ukziuedy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rorehgda.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ntrpuumd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hqbaaoms.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwxrqdle.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3hcrppwgf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ghpkkozv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnjffkkf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3zxnxqoer.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bttsoobb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nhaztqtv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3irlkeqnc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3axsonenh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rkxsdfwu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3fvtbjnng.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3svpfptse.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvijirdi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bvsmnrdb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gpzlnthm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3zjlkcdsc.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sbihnssy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3twqizxol.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qbyzniiw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xcxqetvc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmywokr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3emppjvpm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3thlnqjsq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3dnwlfjzu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3idtovyka.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tfqvubpj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pxdybbyq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3relwmnem.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nxjghafw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zcwnqelu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3gqdnwovg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgtobuhf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3pkglhajt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zluzwgyl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nzxqzfwf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vswqqmnc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wpcrhxav.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kmafzhae.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qkcbrqbf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xwxfqeqs.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3poqyxneb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wprzrscx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ldqhfqkz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hzbwljvj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3amxhiryi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xaltvcna.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ufuaeinr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rxzozefl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bisggruy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xjuggjli.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsulcmzm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jmhqjxct.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qajuloyz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vgcvqlmu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3pyslrqak.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vwntfpbg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fajrwixf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mhkkqjgo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qmyjgopk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wjwwigup.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3buobrlbl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3oyowzwqj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3pfuhxfsx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rwwmxzvu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wwpvekkd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tiwbxcqa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jcguganb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3okwdddxg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3sjwgzxii.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aayfmsqd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3kdsxvguk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3spjdtvzt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rdyxvaub.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3txfdxfna.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ezcwcpyt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3pejgbdgz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pqdxduxu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3chhkjxsp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gjubewlo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3qxiwygiy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ulgftfwa.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nnqoikuv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3eikkcupn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3popacjma.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wjggeqtk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxifsdlq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3zzhwqrsa.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xogzzpwa.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yttvftwc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ivhnrhwz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3iidamowg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tlcfzgbi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wjnciagm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ofqlhfji.html


<!-- 参考信息 -->