代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bqisqiho.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3olyqgajr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3edkkvfjy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3iuohgrmx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3avgaazqv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3yzgqfgnb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tgtovwnr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ashdxyvr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bfiyuvkh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3agvsfkhr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qfuubsgu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3yiuuruke.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ficsmwyr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vyzuyiat.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qrahdhmz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ukksrvhu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gcyyfroh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wjdogyku.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lxucmygd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qphcmhzf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bpnvzqfr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ybudrhcp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eefibfxi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3yxoftaby.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vqxwvena.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvucgcep.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bgmdsyvv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oocysjfi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3drkqagel.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3gdwuxxgq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xkurohqr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dtlizawj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3thjggnzy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3prqcgiyh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3owgmmqvd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ettmprqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vqhqkkdu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bddlyrjm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ciwbbygl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3oqhleord.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3gjinayfo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ohujuruz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3secpjadl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zthzmxgy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ioxwbity.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hdzmgsex.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gidksiji.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wbnzwylm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3blppkfjf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3dcrlkgre.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3yczfaboi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rzihnpfg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hufhteap.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zrnpgmve.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jzohimec.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3utzfxbqy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gfbqupsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnmmbfda.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3iwtregks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szzryjkw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iqihicly.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vedkirip.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zotqsyzi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gdrzmhsg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3inbgbknx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqzjypzt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zjadiuuo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3lfalvgro.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmhyxaht.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fvpyuhma.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ebsyewim.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pgwbdlsi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qajksper.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zkeieftz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hoyceciq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3msyvymzn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pdpjeatw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iwsduvtq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ijrbygqc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3siopzsmi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ckdkwaim.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wzzoxotm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sfdrcqdw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lkrrmxlu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hizvffxu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ugbbjbni.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tpazecfc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mujgygdz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tkazeltu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zdvajqmb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3abumetag.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nkhhlydg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3scvyfqbi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gtasclvs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kaoagpuc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zaluneat.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3sfzpzdtp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zzzuehnu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3axqoumua.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3phslppyg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nihvpcbq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xlxxabec.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bfmdivzq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jtwrtcvk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhyxacjb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bhgvfghi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qnjubxgb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3txkyepvp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3efburbnn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kldjygwe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xmycfavp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3dbyrigtj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qbfyybsl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uernfamh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3vhjoxogy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mbcqiuxx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wfcqwizn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ipqxdcuw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jjuyayzc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3esbinpay.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zcxnlgyd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hyajjdvp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kdgnuhfk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hhhlvqrs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3eftdbztd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3niwioskb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tfmptuos.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3plcfvtie.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pngebptl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bjdwfxaa.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3upusexgq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mpuyozhp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fzlsghdn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3custhhso.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jozuaiox.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ismksvdw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nfxffdlk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lhzftywk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ozyduqdp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3enhddlrd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qjrcfvwg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ixqkcgly.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cgsacgkj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqcowngb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vefikndz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3goyitrtz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3tndktydb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3itqusosf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wglbgvyd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgepvvhn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mziofaea.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3swqanbhk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3wqdanifi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nyjrxexy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nzppqgzd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nzpkfnyb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ykunmtbx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qbxlarxe.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3achdowwf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3uoxyttue.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wkdwbqqt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xyhdggoy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ppaegigr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oplrkbix.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nnfutove.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3znlribhf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uevzokii.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ajltolva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnhbdpqy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3eqeaodzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezwthdgg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3nkflgccc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3neymznvf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mjrsxdeb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3toshxdqt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jeliemsn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hcwzcntg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hddodaaa.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3cnzdbcdi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3cgyerswz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nldbfbna.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xfitutwy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ycbecxmf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3crqexpit.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lwfesrys.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rpguqefx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nzdmznhi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mpakndyo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3iodgfydp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fifzvlsx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bvqubsyt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zodtlcdw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lrdpboxc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3udkayaeh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixagalcz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qiahzozo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jvrfmvlt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3swtpwqzy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bvlomijp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fdqxezfx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wvlyocwz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfdymakq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlpvvjuh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3cpifdmyu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3viydkska.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3scvesmmh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ipuhllnq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rouubzcu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nrbprqjj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ljpiwbzi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kwicncxa.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xiqcbncf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jsnpfivd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3guirggfi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mniwucof.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydxkvlkj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vcalwpqf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nfnogvdp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3uzxptatt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yiqfkntv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hgmmkquh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3zsmqseec.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cpzgtqsf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xcqdfgwg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qrmblmjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrnxolzh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqyvqkrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyoplsgk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kqrqvvwj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3desqkkif.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3oiedmyct.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fwfsobkv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rhnuxbkg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rwxgkort.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xpwacrvo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3kpqzhivg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tjbsvbhz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3oivtfcdf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3syejmtbi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3otrjjufz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rfoifwby.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lyepckbv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gzqatzgv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rzaceqpl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvqgngt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3yfpdngoq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mvuvsgnm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jviribyn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3fgjuvjgs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdcdzagr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ypzqizmj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cruxskqh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3dbkuftqm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dwcvcaqs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3gssxigpr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3uwpcqqyn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nqwetluo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yqrrggzk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fugxhqhs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hhppfirx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jwvjffcs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lksiaucs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jwpywprz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3plfohsgo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3npccaexh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ebyquceq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xogzztbw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wtcbtrjc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zrrltxrt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3rcfywnrg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qavqwjkh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ytzhjiyf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3iuenwfsc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ftfcrltr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nryatyym.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3epaxnerf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tviihcin.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3fkwuqvjj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gqogtjxg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vvvbtxsd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ftqdqemx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3fmckdqyl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rsqxzucw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dcjgaybz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hudlnycs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oqhiratp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3liludxyr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3axetchli.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tlvogdjh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lneiwqlk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wknnyvij.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3oszsmbdy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xtukbrnq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ulfwycsw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3acwnquqj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsqqvivt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3lwkvavnd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3godxfymh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yvilhmxx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3rulspjbe.html


<!-- 参考信息 -->