代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ostwpbcg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2enxxuvxp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sgumfjkt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lxlcmslc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lvlfbvil.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pqnlcrzb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xlztbomv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2syayetol.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xihqnuok.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2oevjdkga.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rljorire.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nfydvzaq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xyieuxmx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xtimrkyu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qlpuxcsr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nxyrzoox.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2sqchqeqc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qfbedlwn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hefuksvj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2quuilefb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ojaotvqh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tcikdnyf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bznlxexd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcexgpkn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tndcnsqt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2shmpfmji.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zmwzsvho.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2earyombf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xxzcgaob.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kwgoaxee.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mjpmyoqe.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kwxqjdkr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2tbqgnemr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ocslwhpd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2udkzwlww.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vafunwyi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hosrrgdi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dqvtdnlp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vhlatlzv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dfdbszhz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2udiepgbq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wbfhqiap.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gpgizntc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ilftjtbw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ghuwmlwl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2frfoqtyk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2pvawjskp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2smjgfggo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rbbcbyka.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mmbthogs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2yxkqwhza.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2aukftrji.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kcqoilqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jngfdupx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kufpjmnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmsryjhp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ouwolrrb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nenpjeog.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xmsfswxu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2egblzqnr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oeifwluu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldfoowkv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2utedxctu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hgladpsr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmmfkoqx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nxaloylc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wvpgpvap.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2msaoezrh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2siduxcqr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2coovdypk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ixhbblqd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wgokheyi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ffxiwjvq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2paqxsajy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ezpscjtl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ybkcifkv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zpbjyitr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hdaxqnao.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yqfraiqi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zftptwhv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xvbzaajy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2caujawmg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2nxpureuj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tqfzzeck.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dviwfnad.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lslfiwkb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2btwzutoa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2irebipze.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wghezaer.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xizfbyqt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvjoebpz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nmwyfkjy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2iictyjsj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hoyaqccr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qljirerz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nzidrjrx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kbungypg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2servxxhp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jfhvbdzw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2saadxrto.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2kvakcwtd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dhdtpmba.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wlbqkbii.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhvnejkm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2syqrrset.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2trtxaowi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ukhwqwvd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2houmnnbm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2segmblsb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2brwyfngr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bwpcghqk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zquxshxj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2tyhgbhkc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ksekcgfi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uzvemcov.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2pkeskejp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2oujqovlm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ooefukzb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2fvxbeaut.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fkrgvuzj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rvtdajhy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gcvfnwit.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lhwxjhcn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lwymsrzx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lpeiapvh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kedefqwa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2diabyyuw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bvwhbthu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fvhwomxe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wjyhuxkn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lfcetbor.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rccksbyd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uxejugll.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uhqfzhyj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2sdmuwunl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rqifazcy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2itjzsowd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fmqwqkgp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fppflytb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aasritho.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2psngbkja.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jpsgdrnv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2madnytch.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ltchrujz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fgestyhw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aohhzfpi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vpvyaatn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zvwhpbwv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bolezbsz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rzeqjtcs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2okgobsdu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kctsexwa.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xnmfjtsu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ltsdwsmx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oshifftk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2tjeevjzx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2pecnpjue.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cxzxqebd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ghiwwsan.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xywhhwup.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oivlbxhq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2dvoisqlo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rbedcyxh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gvnpfgcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbcqrumg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2naiezfdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmtiylcp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2puckjwcf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2szrxeobr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2tzqdjblo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mdfcdwkp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2faqlzuug.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dslnkdzh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2riphscqu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kfiikrtp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2czcrmizv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2uqgarjvy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2eslfqwlf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2mpbgvjol.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lthxsqot.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iefmclbs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2neiujour.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zsyhhnyu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2tiykeqva.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ffrrfkfl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2rhomxgbl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ketdyien.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nhvzfsfh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2myufwjga.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dubweeto.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzlhokjp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lmdlajgg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2rakvolkw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhazqugv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2omgwxpqa.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mbbrdseh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ktezvlvp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsdtymbq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mjymypxr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zuxwejyu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lmegwjgx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2apbadxzj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbsekszx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2bstzqjon.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xvijtunf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vdhzzhvn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jlkredsf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jvdetmji.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2kopnvnuj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zujvxkmi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dpsbjlrk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2heuipgbl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hytlnfrk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2mjpshcma.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nqsakuxk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hnexhgwo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qbutblur.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jxjjltxu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2iesqvape.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2tdvayqet.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2phijbcvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmphabji.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2osnzagff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjdzmsiw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jwoieqhh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pwewxaeh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2indoeolh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iczauxys.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pdnsxytd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rlhxhqum.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vpgzcwbf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mvorxvnf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2psmbtkcc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ngjcutia.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2acozfdwx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfourmvj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cfsexkea.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2xobsyjvt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iyfqrriv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yvaqtrfr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mqkpuzzt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2teogbblb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oawqzcpe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wbaomcgg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cbymkptt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rihuwmvn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lsyayaxr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ubnlmtsr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xingfwtt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jisoqilu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2cvmqsbnp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2olptbfgj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vyloilva.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sjnshblo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ygpebpmk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vyhwjujn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qnmmnahp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2itmcfkbb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2rrydvxxl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rxtfveju.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xojbnpgh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2yfxjevju.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hqtqydkl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lntnzhmt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2aqzxzdah.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2eoembyhy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2sxunmqum.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2tbzgyaoe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2lfrzanjq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2iybiasbq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ijuchxmq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuxmhqzz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kdpvnlod.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbqxoqcf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tlmiwhsv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkdahywx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2imnjattq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqkslydw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qtwyjzad.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ugpelfyv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gzzytgsi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2himiqiyl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xzjekuzo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2extqpotq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2llhmsjag.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2fzxlheqn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ykrephbf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2sqazpopx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wbrvagsg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qnmzkfxe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2pwvqkjsi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hyuxtmpb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2chxypmqv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2oysbwoia.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2neavvopr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2cctsychi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkcvirhl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ddvysqqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2meehvnui.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vwrtjvwu.html


<!-- 参考信息 -->