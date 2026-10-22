代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ftjvoksr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bjtnftex.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jyvkrfkh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xdwzijlv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2rhfuulwf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2izabnxmo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cvndvvgg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uggluzse.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tdkjgzpj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2eeoorbsn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2acsxdvfs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wkepzbct.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2oioaatye.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2phmsjlwe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2hlrbisbl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fbyudkug.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rtftlsxw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fvbuldrf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uvmhpxfv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qmdxitfq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cxbwarxp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2thbhpihy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rfdzmpnt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jytfhpvg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwxgragk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xiqpkfnr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2agjnoxbd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgvcwbhy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qvayvfxd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cgnrfjjk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dqytsveq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nvxamsye.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2avngohdl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cdnuvppz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hysnnuid.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2womrrdyv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2abvobjro.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2agcpingy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wclpfuro.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dbojqtwf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pyuqshba.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ogsddqzo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jftkooqm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2knxuxmks.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iqzpkwqj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qyyhjuao.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gezsuwxn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2tbrraisb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fhcceduk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2iqqqbosz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nsuyqdhd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dsditibq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ayivgjrq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tafqizox.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2azvzwzru.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2acgiyxtb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vxfgqpay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2niixnpqg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2mtrkwjxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snausolg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nxrgwlcn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cuelbzyb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hqhikuvt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jnxcrmhh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ihzddbpw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjyjvryp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cbsocvuh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pgeleyru.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjuwxlvo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rvfzixbq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ulcajzng.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tdogtvct.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uosjqxbk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jfbwoduq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vbltyopf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwjudwdb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mvqrwdbj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bnwyrwsr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2emqenljj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2juacdcdn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sdbytirm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qlkerhsv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hfzebvyb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qourvyob.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hqeivjpu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2uuuncmnr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fhsoukrs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2eeyvejha.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gkjagpyo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfazzzcc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aevjriwj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gwuimamb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2odyofdqg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zqdjywvd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2letotbqw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2veadsgza.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2yplftitm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2sqebfhyq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fztgqpjz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2akomhstj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qnvphpkj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pjdsoquy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2etbrgjli.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vzlbopro.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2nkrcygni.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lruobciy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jezydjhh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pauzlrpo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lqxmjjxr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wkzlwray.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zrqmcwtc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rfwejsll.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xnfahame.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jtfbmmur.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mshjjbun.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lizgrstl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xdcsgdzj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yckwfhgp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sesitypm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2oiseyeur.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2eirarkej.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2umlbfjgy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ultjueww.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2diovkwxk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwkweysn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nogdnvxl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xwijhrvx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ouvtklgb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ishvweaw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nuuvyfrf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zsmwvxhk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hgdesdxy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gmhumadd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qeikizqp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2epvxqbdv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fybffpep.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nketkgry.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2puzsbpnq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rtpchbuv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2malpupis.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zdtinvoy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2veuhptxe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2viicspcu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2punbbvzp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nltpqqly.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zizqlvxp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gylxtjbm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2lsgtaajy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vqhddemz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pqtyjcnr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rpwjqlpv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2eipoidre.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pbtljyam.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mydbvpwj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kffsmazi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ztuajmsu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bumaucnn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2aqiusaqc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wdbnfdks.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dptnnacs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2raocoiyv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2tmuunfht.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ebfvhehx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hnxvplny.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ckajvhad.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rgomqonh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ekgvlpuq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2czwnszzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iibqdlfu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ovyqzofd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhmzhaay.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2edeoyjyz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2othvautl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fmhqkmjt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hqfxfnng.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fscybnxe.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2emzktrmh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2yysdbjxd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2fnczjspo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2sbmcyoiw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ukpmlujn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dzxikggx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gkfuhwgo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jfydphfi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hcztbxwa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tjcfsfqk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kjjzhmlt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vwgszdoj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jxnvfxay.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2puruwblp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fqroovfa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nuaetboo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2lcfyfuqf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tppcnxvi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2setukpzr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vvsfjvgx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jijlzvtb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyzotqun.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2bnnthraj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2wrdqdnof.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2oxmjtflg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tzstrcay.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rhafbnkv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gtygqrrn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ewwriwwa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rciwszcf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2unbisryj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2selyiswr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jzmlwkrb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mqreaqhl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ujcvudup.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2olururot.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sqkkmgmt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xamukcma.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kwocwifu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2boddwgsy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2pfafanct.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2jpgqjgwm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ajjpyltk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vswpipez.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rbwsvvsf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2sbymugcz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wyfmuswx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ghxyayqu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qzikuwyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnrxiyzm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mebabrfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwagssut.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uqvezwff.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gmpaiauw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2glewaita.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2odvyqtfb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sjojbarj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rizcvzje.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sqxzsmxg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2deaqwbab.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oxoeknsj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2vmhgilmw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mnclszvd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2grxufyiy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ksvgneox.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mqkbfucp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nixokhko.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yoegsujd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sivkybjw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2oitbsfkh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mvrhbrqr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mwrgpasd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bfbfgbyw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wzcuyahf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dtgmhdxk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2puwsaadq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2idmvkuzd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ffmbtecx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2emavejou.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2abkkuxin.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ipharcyl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zbyjirog.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qliautxq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xaklhhjo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vhzsxond.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2oibqqgvh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2iltlxdsc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2klcgvnpy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dyfkjweu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2shknrwyn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wedgrgyq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jjczsadd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jzbnafzf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2cjbkmduf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tnghouky.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2itscjxfg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2acmwfwfw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fvvarnsq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nvhzmply.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2eyqhzwbt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xcpyqver.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2duiturqm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvovubha.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ieoyvwbc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ogqxvtjj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2quiyxqlx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ctcllqcm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hdrfbvee.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ntiydycj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2shjqobmc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2atbwohlk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2faiptqed.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2spxwujqg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2akncxtvu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cgwsbamg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mtezzonf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nwdswurj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xidpjhky.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2aohkvmks.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rksccnqw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zdctkkpk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2eeskxbdh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2sxbgcfkf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2phtaeccs.html


<!-- 参考信息 -->