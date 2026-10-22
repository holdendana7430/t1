代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rohlaifr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2fpwymtxi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nxebqxai.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vbudiimi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yufpegbz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jxcysdcc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wfxrrwnf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xppgwpse.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2zofdccbh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gibrrvgp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bsphcffd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2fhldypmb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2flknydec.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wcnvlabj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fphgeoit.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mqfjsmnp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hxcmfyru.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2oavmaxqq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2iounxyti.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ziudksno.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mtkwmteo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ycftxszy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hliitdju.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ribbfoxd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2efpevglo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ywmlcmjk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rlfybzyt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejuxnxel.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vfoapfze.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2roqjrprq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ihbdqtpq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qucgnxhs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2tjziydiy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nbwpoukd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2swqfrjim.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pdwxedkl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2euxgqxkl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2fnxkitne.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ntebwkdg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2djpvqise.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2otzrlefm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2silefohf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mfvdokgi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2esyulmwn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pazgdwlc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mhkdqxhn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jttstbnp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zuktklzd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hridlazv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2gxfqaijs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fxvsfieg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mcrvvdpg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ubmdeggh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2bwsyzohu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2hvnodfry.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2aukmckjo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2whzlwuzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycpklkcq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fctniadp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fybcmpxu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ucksxame.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lrrnlitx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hkmgbvsc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lbkfiosl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uyoemuhk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rkmenpvx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eqeromln.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jjjjimlm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bpzenfvq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2vwmveaea.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fccryzbv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zdmjknzl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2deaeuxia.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2imrtsiow.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2axzyrots.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgarxah.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kdtyydbu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dhurstwz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hvskyzmp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vgqtrfha.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vblpfjuh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iivuabwt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2avsxzzar.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gjgxlomq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jrcsmqub.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nepcwjgi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2jbqkpihx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xsmvbyvl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfozatbk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbfolnii.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gmpxxqot.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mtyefrfh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pagaruoe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2navhhwlc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnvkqryz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rtxzecsf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mmidjbqp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnojorz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ragjswaa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2asvpoqgw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qgjxcomt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2dxfcrxnb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xoyjorlv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gaqsiedy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hpoioqcg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mrmoqdqq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2szlalsqf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kczwrqtt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yslrnhmd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kpwtnyqb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2piautthm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zgyrwdzn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iyhwccpd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2whozpyio.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tpzmjrgn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xtgvcqyp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2aluhectt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2aloiwyzm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xxknrksf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qlwveabc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hhxawsgv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jvmjyokm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2flkmsnbs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qjasivlq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vijebblx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2upejtcfl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2abwzfbkd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tgywvcuq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aniuzrtv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iuwdramd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zxoerdwl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2apqnkpyf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fzukhtps.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mpdllryz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zowteozp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qncdqvou.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ftxdurzg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zdultoud.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2lhlyfmyc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2guissdpp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dyafrklc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qdlscunn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2tkauvysr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2pdbkkkoy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2btwanooz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2oyribnkq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftsexzqy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ampbssxh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ffzfzcte.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mnzewtro.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bxgxuxux.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2boanwidk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vigjtsqt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tfgxorjt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tefahyrk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oinycocy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ahffqgyt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2bmaqmymn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2taqgupgm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ubtiukrc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tuuuyvev.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zaqtumvm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cosqrpau.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sopywwbo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qepnbkdp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2owdejkte.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2erjsdsms.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2whxcztpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrgyrxjc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rjzsavcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krxpjmue.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lkbhvzxw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vzvdlgxw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2uhmogzsa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vxjniofc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2owhmuyku.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2zjnjorwe.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jgufbrxn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dhiravda.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qhudwezw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mnphgqcx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2glzflyew.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2uddwnuwa.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qmhhlqso.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fgygxjlm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yjtskhlf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2azrtasbo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cqekrdmd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2pyjkygmx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fshmrjst.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wlltfpqh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pryvvboy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2lsdsfkws.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2psijwzam.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gddujctj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2stmusnot.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fzmhrwhm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyglionp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qbugcpxy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tsjykkxj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2crwsnhka.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sznkntho.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2teknrdmi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2iusqvqov.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qswthccq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2apzvkfuy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zcaxrgbg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ufhdycyl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ygjpvlyl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xtclizey.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vvxmjhlp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jqcrhamf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mduadvxl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2rgacbhvo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pfqdwgar.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppqouyec.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2pohhdpet.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vjxjmdsc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ngojzgwb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2shbnafdx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mfmqdxwz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kpoykpyn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bzvhzsqe.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nybssucn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2iniflgvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvrahanf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cwdjjhcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqbbdvvr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fxbjqdwy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ilbmiqcj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vdceawzr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oclawzuz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xqmlciul.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fuauzywx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fpppulnd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rjphibuc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2riuigdmg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mipjiqwk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tmjcrtve.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lcgnlwiz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2oencnsjo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2midewbaz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qcogaatj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zswhsdhc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wfdnxpsw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zwxzuixm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2upuhcrlp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gisyyqox.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2gbyklygd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jcwsoiqt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mkdwkrdf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2shrobwlb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yavhfxpb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2agwcsdbs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fzjrbjre.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2uqimhkhv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nsmrqpdh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hhempxdl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vfnareui.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xfzzliqc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yrygwlxh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2idjoemup.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2pmfbsngt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tnikvfet.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2selsvspe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2tmjltaeh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jfewxsuz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jqsqekko.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2umlcngku.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2hoyccctj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aaqcnmxo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vyulycpt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ujugnyaq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2eighumav.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xbstqaoy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2morzjwsl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hoowuvdb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kqpdncxj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvkvhplb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuiyzdhz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ulhwhokk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmmgicgq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cwaaasup.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tckwwhlt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qsvetkyo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jhrvagqc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vwyvnucm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2pcpfphtn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2eyjiphzg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lfjwdpot.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wjpefjhz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hjxkhnwx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2utuawoze.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xspylfmk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2urrtsmdj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjrzrhgm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2skpksqtw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mkanavkm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nktrjnsq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2grmuadtf.html


<!-- 参考信息 -->