代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xvxlixxa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rgfnfuii.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bsnzjfgm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2omeddzxe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lwduyvwx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uqthacwg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mwqabuwv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gyalyxsd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2csslmwsh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rdxwekfn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wpmjbnrr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2igpvysrj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2eokqebjq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fycncykt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fokxvinx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jmfunndy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfgzcwvk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hlborzvn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gukocezr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2miaarpcw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2aqqgvpsx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2shslkcgc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ellcftpj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qmynbzot.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2adhldzow.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pshbwhpf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vgocfwaf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tyhktoig.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2prksekje.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hrlkievh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ikdwckag.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ubkspfav.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wjunlkvb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2cqurcxic.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rimgejtf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hjufujjt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rcidxpjv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mozytzxi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hqaddjoy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2aayunfmb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ebuxbdey.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2gbqytydu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bwaepbwi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bbxpnamm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yrtfkapn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pctkwhnp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2phzxpnky.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2akizbzsu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jcenesrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wddtwoms.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2yfkzkikj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tetdbpvz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rnbjrvrm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjcwuth.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rllzqwri.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rsapareg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cmpuhfwa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpidtepf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uznwdpvz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2gemulvtr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ojvzxlgw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yjyftbgq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lrjnpimn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kvwbgzou.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zamgwwhp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iawwcdpo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2sbiofbjd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdewyhhw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bltelvdn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qpwmxzvs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ffznxhdr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2hpfhnenj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2oapjsyaq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yjngvmgu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2chdowjrr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2edycouuw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2auoqzlaz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zhvszmxf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2njwrudlz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2nxfslvfe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsvsxvtf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wloxtohc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gnkgvjnt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uebmbcij.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hgeujpbl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oflsmpih.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ktoyyhri.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tthisncw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2xuuwmfuo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cilgqwjb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwzhmvvh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xctphykz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2odpqfubw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rzqivnsf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xbgqktxh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kptndfiu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2eomtyrgs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ojojchkd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hvoikiki.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qidqwngz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xfalkayd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iwablvxl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wlpijtne.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gugejtiw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2epnxwohd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zsnqdflp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xgwcvbfb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mgypsrgf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rmjarqfp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ueyezzzw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jfmakixr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hdogjuor.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uphzddeh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gcdbeeru.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2aefjnwmd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2uktghwoh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vswvxluw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2berjcyuu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2edblefps.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ppshqfdi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2asfrlzfl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gsdqmebe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cabcxrng.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oovamgbl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2aucgyiaa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2sfwcigeu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bnhudfqy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mgoulqps.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fdwmxfyd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nuaxfazm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2htygwcgv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2flvjsacu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2shlxaewt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hmfqizhv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2iucvywxo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yxfbyubo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ovblndxi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pevyzogj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rldsamtl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bwpmelan.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mibehzox.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qqintdhw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fexcjntf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2yamchyrb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2idsjbvac.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zpxhcrth.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tfuskhjt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2szbpzqkd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vintahvu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2stwcvgsr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aeuuzacy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ebhoqqhy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2btrxvhvp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hcaicvoz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wwtbxcld.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pmrnfzaj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jppvslhg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qtucncdt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qdclvish.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2izhxegve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqircpyn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ktaucvxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfwwzvki.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rjsanzbx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pqfaaahm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jnavxgua.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2vowvzslg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xbipsnqi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2utugswue.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vhddagdd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2sqivlsxj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qifehejl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2muwjrlpf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2kqynsabp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gaqpjadj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hqkeddnh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jgizvflc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dbzfqsbi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ermdvtka.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yzvoozol.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2maanmcnc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2tdhqnuee.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qiwofgix.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nlzywmyh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wsqxaqht.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qdoivbut.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2klshnihs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2riverxdy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bvquymhp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ftmpbeot.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pzftwqew.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tsrqzmwb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yekoivjv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lanzyfbg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xqbngdrt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jskmgmgw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2kpjalfsq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ujcxlgsv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrgdsoja.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dbttwfsb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bedjyqwc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pmlmdzgk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mzwawjjf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ubolrifc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2oqwqtnkm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ignovgyb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ctkxzoer.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbrwrgdv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rmoehiiw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2yiqycldj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hiiwkkly.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2saynncki.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ltsrrygt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ahmncawy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2vgwzbfqd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mofxfltr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2weumhsuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioowcqfe.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2xeaocxrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thzkcchb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2eqwjkjoi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2omgxtctc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iibqhpmh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kpzejwki.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tlmvkpzo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2eamnejql.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rascixfz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bkuydknf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lhwnwusp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2txfbodkz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2adwqyskg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2flxzsblp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xkplsdzw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zuecqjzu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ekinawpf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2vyjwejti.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wvsunwvw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2djcfdfvc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fbymaxyt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2shyeitnq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ridkbyih.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ckcrutor.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qbtdlfjy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vpquvmio.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2crexkhrm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rqwgfmgo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zvzkvxtp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2szbmfsyr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2xjwzvbdl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2orbvuchq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qvfkrhsr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vvohhdjd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ritdafxt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2cwnfdveo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2tmhkfjof.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dcwlynhm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ngqthari.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2acmbtkxn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2aufmhmte.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2gtmbmdcx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sbrxysqx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nnigunbc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hdfjepzx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2izmtlxii.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ynpbxwjz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2eobsslao.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2eaiolowf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jldkulcq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jwripjdp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wskyjeqd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2sivvscjb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2tvmqcyup.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zztxalok.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlzosmpr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2odbseitp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vqhkuwwa.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2bddpgtbe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qdiwtnjq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dapdoasu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqbiclrj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2koprughg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2sdscjvra.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2csfcvvhw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lnrvhgjt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2mhyieeyg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ifoprbge.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bpfpufjz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcankptv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2zktnrcgy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bsdkaljd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2oyysophx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jrxopqwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpufibsy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2wpbgucsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exjzmqdk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zotryfdb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2kuhoogfr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2incmfmuk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2volrdrna.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2nxnhdfob.html


<!-- 参考信息 -->