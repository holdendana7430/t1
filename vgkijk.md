代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2kpufiabw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2bmglmvux.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uykidazf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ygsiljro.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kcxybuww.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2pfgixeyo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2avooeavj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uhtmrwrb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2yjayygib.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qjhbohkr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dcunyszu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pnymnkjc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cxqqgnhn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ncvfnigy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dtbovvmt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zpgjopej.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jcknboqn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ofjxrhuk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2unpivjqd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tmhwsjjn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zsezestj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnsplhei.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojwfyvhb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqacdypi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vombeuhf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kgwlsyoe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jlokffzu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jtnortpz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jnuqdwan.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhravnn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2inqerlus.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jtfblezc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xorwpeot.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gogzsaps.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2axdglsva.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zmhqmilp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ecwpikpk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2srfwhzwf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bgwnpxis.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hbiammpn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tofxtyoo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wocfvvvc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ibpidxhs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ubrhaeoe.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cpoqdrvu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2arqpkwej.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2uvbobrdk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lmahqwrd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uhyigqwf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wchgfknm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pekuotua.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jhxjytsm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qklohwut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dalsnjgt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2plndbipg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bspcttmx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qhpgtvoy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2czsbtigg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kuphsoql.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cqdjqmnw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rxkysapu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xakiduvc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2utfumcpy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wolusjxp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2beagiduz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zljyvoyt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ljiwqdxs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bmzqkjuh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jiyqjcab.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykwzwexy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dzdhmfvs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lkwpvaiu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fyoecfbt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ttqmkkve.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2sitravxz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2apjxnrds.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xdnwxptd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hbspwtze.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xgmtwkee.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tacivooa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gcnevzjv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qkfyzfsv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wbbdmsjj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rvykxlcc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2utdaidmk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qrhwbbuz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2khsqziie.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qjasoaum.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2amktnrkm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2icvlfsqi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fviwzpii.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qjkpuavl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ezxvtifo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tmjayzkd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydxvmbve.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2resngsqh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2flosvxhw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2nqqiiguw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ymaouvbj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cexwnyda.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hhkuxfwd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ccoijgbn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mwicjbmc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bnicnngk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wateaneb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fpuucukw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vxgzwzpw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2aguizbbv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bcnspprg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nsytmuqv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2yvdsdjmo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mcctxwsp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2icbnrqkr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jnzgkqea.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ghgbsmus.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tcyixbih.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2umrlkskp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ectqpdxj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bvhlqepd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gaeeafjx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sktnkwaj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cfutdfid.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cddipryr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pknplfvs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mgoijpon.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2soenjpmv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dcmfomxm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ajtlhxmo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2anhtlqoz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tztqougq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zxdpmrqo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bobwzhye.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hywvices.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mqlbfaan.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ufidtdpk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xfxxxrju.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mtcvvbch.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dvjyuqkd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xifhpwvs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tstmtbjz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dvqurhmo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pnynyjla.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2aoeellrh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jvmymspn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zosbctsl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gncpsuwc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gndvyibx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hwlshpks.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qjckyskh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qdenesci.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kfgnvotl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lpwvcdxj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jlfwjsag.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rxfgzkdv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2flxprdpn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ywpryyes.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vtnclbhs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xmkckvou.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wseksuig.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yuvltbqi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tdywrwee.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qpyzwgvp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ydelgrhe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dsqhbzhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttnocijd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rzlbksxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnolneje.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pbpwemyn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qwsgzkau.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2immhkrhd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dsxlkbge.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2faimbaar.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vonjovnm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2waaxrxec.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2pytjkjwa.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rtsxigdl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yqroufue.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ndbzkhmx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2repwocjh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tfwcklrk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2chzbjpdy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2kofsawtc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2luxvmior.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ccrurloe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2msxesgja.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2sodovkvy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2oevhtojf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wsomtbrh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tfojerhp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vcoycznk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kmdclgyc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kcrkbnoh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yffksolx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2messghqk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yqfqsehz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ervnerzj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2gnkttmbj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2iwhlrrrf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzertjux.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2gdyywbhf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2lfkwfvch.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2pgbzntsz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mdymlsnf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nfrfjqss.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dijbuyxc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2frpchhmn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kuyqgfno.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yydqcbii.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ymgfplpn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2golwsdzz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rsuqrhvw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fhmkmnhz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2cefkcrig.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rgzxovkv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rtakbbru.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zujkinvy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jdksdxht.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2hyogpvyp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bpxkfskb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2crlddjno.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2slmkjwcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfwmgeov.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2idznmjwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpnqatjx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nxzfkdst.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2reesubao.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ocoalffy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jmckjlnj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pbdmgpzx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2itqjnlsv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gaudjeqs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ctzpyown.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2sksbektq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kabjaedd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2werpeokl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gcjtjwrm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2difkgntp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ufiqzykd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pfuomoqc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2dsgdgcbj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkjxoxy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2whkunewg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tqzjhlus.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ugtgglyf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vegjetky.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nyzcvoap.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2djptsjcs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbqgyua.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ptpfpssf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ylvfbojb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tixgonwg.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2slcsnixs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2tsmlpisl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sjxsekih.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fubwhuci.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hicflmpg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2neghgnul.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2csypzeiu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ufiqfkdc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fsoffzzj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2gjbhvqqd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2brnuihmh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ghnkdflu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xemrlqcx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wydakvoj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nzgzlpik.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yhzfngnn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dkqpalnh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2pafdkjgs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2khyavyml.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xabkqfpb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xmdemzfk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ciqiakbq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ettdlnzo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2onicujnj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2gqzihgwx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2uzqpgach.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dapccfqj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nloxapqy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ubdfjejs.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2elsttibz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ytvojsgf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zmxhvuly.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2kcfgdrtl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2mfvcxkyn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nudipyoy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ttynxyss.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2bmpcukmo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ptjqliof.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ieheximx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2blhwllkq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bqnalaao.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ttehzgeq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ptftlplh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2riuedcfu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2dllkfeuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnnxblrm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2nuwnmkbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlvvkzas.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2krhfcgzu.html


<!-- 参考信息 -->