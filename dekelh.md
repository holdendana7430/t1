代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zbrerbxh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2myqinugo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cksemwlw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qxhyjdwg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gpydbdka.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2nbcufzfm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ngqiugnj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zffyjhip.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hegkvyha.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lshmtfbp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zwptdwcf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jfsomwbr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pswkpgiz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2cotlcwky.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ehhmrntx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rauffygh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iwcpxzwh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2moqmhbin.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bakqidcy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gqbglvuj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fndzgdsq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2djgfxkvl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjmjzrln.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vgnafkhh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2alchssjf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xwtwofvz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kvvcifqz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bxybyucd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2agebfzpa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2czogddnm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zzbbjwkk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfysbimf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vknrtclx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zvlmluks.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qzzqamqo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fdahfoja.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yszeueti.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2utkngktn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mhuczmin.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2yuzvzwll.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tokbxqjr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ekzsxbbf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2crhjtanr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2axazeslw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2xcaqxaen.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nrlreccd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pmacntah.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2scfjbufs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fasynhlw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2nfwktdqc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tsrrqxud.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2draqzcej.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2expezhij.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2fxrjxare.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2emkfvzyr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2klxboqff.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xxbbcgcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxnwkwjo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jvtjyifa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trxqnxqi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2glkrbzgf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xywatkac.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uanncdnr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mhhzvshg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2evnymvem.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mkcoosla.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fwgtiwzx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2qgnnjxwq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2needcjkr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nckmtwnb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vssahayr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2onjwhadp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jqrydeai.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jdvudgwz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pjsztlyl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bhahqxvd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bjkhxjii.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ijdhawfh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pduupuyl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2brwbolzk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vywuwbua.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dlncfgyr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ontkmiop.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2uqungtdm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2nykngzyw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nptzipru.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gptkevoh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rlrejhho.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fbqwuheo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pcpvdujr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ldmivmty.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rubikkze.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdwfvtfl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cbejhibb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcrlvknf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gjltqiyu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bxzkvrqj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zpkhihfv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxkqfkji.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndnhnxfm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2puizqhhk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2whueotgu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vvfcmrqi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dnrrownb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2okkmpxdk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nzdukjaz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bobdchhc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2enpmjlyd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wbxbhmbn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kicdexqi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2mpfdoogp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rsepdmvr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cvhglyag.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pirulaxf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rmyvryzs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gpibyzfs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2guhrvmee.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tgwoqdvu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dpxrrpwz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ofevxbhg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2rpjceidl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2itluxhdq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hhjonkdy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kluqmlha.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijrwyqof.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cxrilbpy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ddaipewa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tbjlmohx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2djypsmoi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ulspppsl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ebborksw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pkmjyqfl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lnggfxjl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2aseoqadq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gutkhcfu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xbzfclkj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2sxnercbs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2edgcqhsv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ggekzqta.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pfprmybp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dzcdtfbk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2biwrkwbz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ududqkut.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdxjhjpq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fywhdtnv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ichqmiaf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mzhuxlxj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fnhcpffs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hqhnmlex.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cydixrwp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wotyntta.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fnjvvepn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2bwkkjskn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dbsasxeq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sfbpezka.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ativzklt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fxgorycm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2cmofoyfi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gnxfwppy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2tqpjlmxo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ywuvvzfu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vxxjzezg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zmmyjsxl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2etmtullh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bmncbgeh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gywetcrc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wfxrqaqd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uyqvtact.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oztyfirh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2klqchefq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iflgvqll.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dqpstrtb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kwdoipfl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ozokvgto.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2uivrwbnk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dylqzdkc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2klsvdoem.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2sqniqmmu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2jgdiukdo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xdmwrnfr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oaetxrop.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ejprfwwf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2pzzppdqy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2otxvjmyx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cvrduyyj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ycpgcote.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mhkwfjxj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tblsquye.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2oopvxvnn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xjgbpkfk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rrwvztgo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fupbuagc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2cvrebzds.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zwbhymen.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogyqdxgv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jnbegzpb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sdflznne.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlvfjvrg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2tpzyjgik.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2fevoydfi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hkesjrjw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2aiittqnt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfkjrjdp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2elwuxiph.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2dgqgqloc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2njidjeny.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxfebekm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nxvatikk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2yceovxpu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jxxznlgq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ipjgryvz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mpgrovgp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hjdjuwqw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2udxojljp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pziolnwv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jiyrdrch.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2fgfeurhr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nlmddibu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2nfwornta.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dfmmvpji.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2eghhcsoi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2noqagrhm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2mpmllchm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bdkwvbhl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2owpayuyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skyqvrgr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2yedfcmow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqwpqtcs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2impgpdxn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2oqvdzhqw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2thpicxak.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bluchgyp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uwyhujmd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ndcvkahq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hpnkigcl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ojccmdfn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2pmkhcely.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2hovtqqtm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xskcbbwt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2chcahfgs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2isrzpkzm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2igfgbzly.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jfktmsbw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2iihrucon.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jwdclanl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2vmfcnbru.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oiacyvod.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hbixqvcx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2eqcboxmq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jovddxoc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2quhthrck.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fxscolwj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bdvxjecy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2eetcixwa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2uocpskhm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jokcyuen.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2nkcfvvfa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dredqmoy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jfxbrzxu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wfccizki.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2avbkjxax.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tioapwbz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wcrhvfsi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qybdhzfk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nurkxqrl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hapvutlf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zfcauhob.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jwpbcjfc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tkvpwusk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2pivojzhj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ooxefefd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2llrozprz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2czxvfydk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ympzlyne.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hkhpxmph.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zfwbnxcf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xwyssfxw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfhhyjse.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmogcufq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hswbmhls.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ephpqlps.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jgdzpcow.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2laptqcfh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2cufqddsq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mculnkia.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fayowjyc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kforhpou.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnhjhevp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2rfvnnwdy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tagbpaof.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2alrnkrfx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jiishsys.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2gvhlsvbt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ajokhnfv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bvcfpfhu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cimaikfi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ijwxkdqs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2dctaxkpj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bizlzxfo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2kmsswnfh.html


<!-- 参考信息 -->