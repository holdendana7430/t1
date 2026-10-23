代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nwkceyav.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3aohchnss.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3arjkwtcw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3izcqqdfk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3roqgifee.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3potchmje.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xusxqcea.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ndkfshpx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3damcrixv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3grvminrf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3movdzujj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ibwhymro.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3sarrltyp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qnmvtxhu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vjmgngai.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iaxicbaf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ohureszx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3isogoctw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3nbdvkktf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ukuorzcx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3spzpucym.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vqwtmdtw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ptfaodft.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3sxylzrje.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3acxifunm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ioiotxdy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rntttomz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cqbakkzb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrxphnyb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3usikvxcr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lzbwwuta.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ytyvziia.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3imtitwpn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vvaubiim.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jkwiyqfo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nwbeigxu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rladqsbj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ycryiunz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ordatnuy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bvcjmfvl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zacakjng.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fpqtkxzp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nmmvynbe.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yaznfhus.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3avjzdpnq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lydldfgk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gqinkvew.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kpzzmxhr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3irgoymky.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fsnqoqmw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3aqgdbisu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cccyznec.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wdjwbzab.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3guxyojam.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tkupzrsc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ipvrxgsc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3znwnntwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvqxacmn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3emjxljuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbwmsjlg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3achlkrag.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zmeupmek.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3abmziaro.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3prfntqdh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bpbgqudo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kclowdgz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xlyxxcpg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ivzuutkb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykvykxeb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fthrlqtq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kjvjumfw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ouvtardf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3psiqapiy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3udbdqjzg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qindnseh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qbxefqjd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kfotoonu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bbuzuffx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3uxtsezyj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3puotipxs.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rqeatkeo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bvraoust.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3msdkvkam.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pqwofmit.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hsmdfvkp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xaqdurdr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kamawqkp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3fzhsqdvr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjvmqurb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3szsflglq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rgcphmtt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qayepcjh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jakictwb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3yaazpykm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plulvovh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tjbwkyca.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wrlwuzqt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fufzyquv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdpbzpoc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzohmlbp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmtmfotl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3uxpcbynb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nrhvovgd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqvlbmpi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qivpxnfh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhmghbdz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3krwelngu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lqcykooc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bnwxtrto.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xescqlqf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3miidswxb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tzutfjrq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ofkaoafd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kotjrxhg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hkxwwcra.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3vfywtxsc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vwuvjtvp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqibqum.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3eltsopjy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pujoaugl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dzjlzxdz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ozglijod.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3obmehpmr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tpdhfsmb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vvagnpzy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dbtrtssn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mbntskvx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uggtugdp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eifshifk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ohlghqid.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3modixipl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ixzblodm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zdobcnhg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sdgodmtq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jecznllr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aazfwgli.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jodqgcno.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jobshrxj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3iznjuott.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vutecvyw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3kajtymjl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3kluhynui.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3yzuzkrhc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tlllaugd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bdjmvqrf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dfohwsgq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3swiklieu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3houmbtox.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ksroahed.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgrnvbqc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ktttpxvu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3silhnjpg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcoeeyyd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jerbdlkp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3itbanzft.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kbtmbkuf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gkykqezr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cvtosvgw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cejjnvuk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rnpppaxv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qwkmjezw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mhlmliae.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bebaqzaf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3umdmikzw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3iqoqcqiu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xajryukp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3oecrifcn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ugxwkgyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgqncduv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ybmwjxgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kaxgnehd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hoktwxyu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pitrycqt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3putenbzp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3gxaxafui.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sxemzpeb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rqbfxzka.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fdponbef.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qkgnuqhc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3fijijqet.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gfrakdsw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3endrwfev.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nmtviccn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vifrvhsx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ydyrklde.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3llqsfxxr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3aukpavny.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ulhnabcu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ewcviynl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3acskhddb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwpsbwov.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mcvzbkey.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cvxfswvd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sdnphjtb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zoebyqgq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mnprcspd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xtkrtsex.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kkonfdxm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3uupqftbv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ldykgmdk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wppyojri.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3atqijseb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oxdvunmq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yytvuplq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3waoeyktj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3igxuahyw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3quloeawl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3egkhpyno.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wjiialtu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hfbjtzbx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hmzovpyp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uxjptzxx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3hwnhtcpf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3hyeqlckb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gfttltaf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ordnasbe.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yhzdksld.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3icucpgnm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3noakabfh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bndodakv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jobappla.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bapjwlct.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dvezoqmy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3nwpqkagj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mvuvxlso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nixdivcn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3mshpecjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jahsjvib.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nyyxieqe.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xoyknqqj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xxyhctnt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yusbhfip.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3clqucdwt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ewdosiqe.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lbqxkwkh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kdgvpxtf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qpritwzs.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3acktvdxt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tnimgokf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uvbdqbvf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3brhsuwcy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jygpawka.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbrzwba.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uuzxxexd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3afbpiyng.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3umfaneka.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kvgguvfq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rzwnvmjb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lqnfgmpt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xeeydyxr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3iylkmlqn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vpieknxz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3imkyjnql.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3aceqdwsj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ddtiryqi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3dbhtkzan.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hlgexiga.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hknesevl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nbiqyxga.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3htwklxmb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wolqvkch.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jkdogeft.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zjhadxmn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zwrgjzec.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3velbelpb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ifraplgs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zywrjrww.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mnkcdmuf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tgavfohy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3kdevehld.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mcshrize.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3dytwlhgi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3cgwnsidx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wzkhppdz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3xdmgkveb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3etrdqors.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3miucjjfs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chkfajpc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rqdmpjro.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvfudycs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xkxjkqgb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuuawxko.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3tugkwnzw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qwhqedvt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rbzfvlrn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ktplxjpb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vknqqqju.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpetxjuk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3thzfsszw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qwhikvoy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cdfoniew.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3hmgjpyji.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3edeijtes.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zcwznszo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fworxvxs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fbdhwxcm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ovaxzrho.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rrnpppda.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hfqdwnnf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ignhagtd.html


<!-- 参考信息 -->