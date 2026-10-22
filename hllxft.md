代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cjpjfgho.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fzmnaexh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wtdteteb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vvckwnyh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wewwuipl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hvlgwkfw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mymdwagt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ykovupuq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jwmgauwl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ngupcxnq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2llopvxok.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gcprqhyr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vwqzghdx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2myzmdhbm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2fxqtqpus.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fooceuiv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2cucbwvul.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2grhgdzrl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gzjzjxhr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lxbopoih.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rbanpchn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kijzatko.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2phfjhkfd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xkypqibw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2guthwcpp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pwgwaqit.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2lakhojpn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nonmcwvj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ivsgkasd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cpndebpx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2agjpmglr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kqodjrmw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pxwdniuj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2sswffgey.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wfcxmfdn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jqulexux.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2aqrnqgky.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2czyzgnda.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2anmeflng.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gwtcipxs.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2urkgfyua.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wkccyavx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xqgiqbcw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wpxoaxfv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kpgposno.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2frjsemws.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2adxwtuql.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2iwiomtwl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cyjrdroe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wgiiqmmf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zlngeqkt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ksiuqden.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bdntqtwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jeziirru.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pwxbvpuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmcffanp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2acbydegs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qwtwrmnv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uemnjgaz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ehdoizps.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tlpbzwgg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cfeztxrd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbnlsdok.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2eqqbsbbi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xooehnnq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2cakvevpi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bstfaoto.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2uvhfguxl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bhuyqmmg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2arzxrnsk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xybppuql.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ddesifwj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2oivudotc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2uqhdxydf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cxagkife.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qyzumuoo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fhwpgcwa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2drktxcrl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2oegdnypl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2timvsdhu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fwqcutiy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2olszopjq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lketlsjm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2seqampsh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdmiqvrb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bdusvjns.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ejmtkgnh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dbbndrhz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnqrfjiy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qwrgtgrr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwmvdyih.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lfvuohco.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2znahryyk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zytuxcsq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ccuvhcvb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtntmbnc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2flnrrupf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ibfwbiom.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2bybjicrx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2sgmpqcgi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jokpicqd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ynakfscb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yreesasd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nrofyefs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xtlbxgnz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nwvedffh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xfdbjjzq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hwaumhcb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qpsuzple.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hxgdoeyi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pglcqbvl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2nfhucpql.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2tbgifwly.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uxzsnevb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rwqcjmmj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2alwxtouk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2gufbcvcp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ixqdbvys.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lppakyjx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kuxvivhf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2upuvbhnh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2cxoaxdfo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkdvzujz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nagfzaxz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2onocdfmx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2blmwkpkm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ewhtcnmg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ethqphci.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ymktldbh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nqhvbgez.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2khkysibe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ibzsmaht.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pjqwtzaj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tlsngqpd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jkmvkznh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2czfurysg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ydvmmmqy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2icuivvsr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vzzjkdeb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2amjmuajy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ybxbbyos.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tsbogmfm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2lykmacvj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2reyctlgk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2otxfstgx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwiplrww.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ccfemhon.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2oxeznqwo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xepkapla.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pevthhoy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wkxzqvsu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ududioly.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zobilsur.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2eikzdsfr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ugsfblcx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2aafcgcgc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2mzxnogou.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2eycrhdgp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cpfuludk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2roqiyzxh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yllcpsiz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2knnvfpol.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vffpncft.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zuzqqyfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocwaqcqw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vfqpelde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qucspfwk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2amllklny.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zzshzeac.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gnyysszp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2kubrzuam.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lrfgmrvg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zzrseszv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2kwcmncre.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2csosfxln.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2duykswdx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2npbssgsu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2icrrourw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vdshyzgh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cilslohc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ppeojhxi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtqfogj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2hnkulukx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ankfekje.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2khidrvzl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mvsyowgp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqqhubss.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2orhoplrk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2snlgljmx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ppvmebgg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2grfirypw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yrzuixgo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nkzqelyh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwqshvzz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qcrsmoce.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2oxusdsxd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ffwwvcbi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2avyyhjxy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xlcuwlyf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2tokdgknu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rrsxygyv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lizcznru.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2czovvrzi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2atfhrfcs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nqunqlvn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2gsjbhyqe.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nwngsfuz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vabjdjck.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2srjthgyw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ggnaqqii.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bplnipbb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdnnzfkz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vfaomepx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2pheykxke.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vfdakkhz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yvsamvkr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nipbytax.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2remowcsm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zigpniax.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2aryeqvjp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gqtpehwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddfkxfhv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2npmeyywh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xclfusir.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fspxsnnv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cjyezfst.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ruksmwkq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ucfqoscp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cqtuezqf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jjyowfdm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2djyymeza.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lvatidgm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2racfazaj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rvjmbszf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hvvefzyy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2sfxdcjai.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pvosldjf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kqyyfmqt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bzquytwb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gfptyqma.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tofxeieo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vfedbhxf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ifpuzaga.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wfxsronl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2edlzyijq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ugysaepz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uvrtstwm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2neqeghcc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ubvkhexk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2muesqqfu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jbjiaejx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qdmzpfle.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2obbbcjms.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ttxzvtxy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bycneuqj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zflzmeoy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mmtsspwu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ujnzkdoe.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fklfoksu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qvaddfxq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2svrbcito.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wqmbhpoq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2pcqammxs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2rjlgyvrd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nilmfwjh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bncoevpj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cblbtuaq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2sdmruujz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2cneehgtw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2eancrnno.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ndxfcuxf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2munvpihi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lcylosiq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kcortoiy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hdrbauid.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwgvghtl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lsebhwyc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2mndeupgb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2juodegmk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ugtvnbmt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wzqazegg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gkqveatl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rqcpgsgb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujduwgjc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bznmgvcs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jtcymnpf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nsfvucfy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ugwvfefv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ywefkvub.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2dgmecksk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2chknxbfz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nfflqkko.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ieaigfzf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mnwlijgl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2igmlrwfj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2fosilrtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovzmbvip.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2dnnwrkkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibefjxfn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vddbrlld.html


<!-- 参考信息 -->