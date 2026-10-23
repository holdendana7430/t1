代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ugwlvcps.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3avdjtald.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ikapyypl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ylomvtkv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ihsqcain.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jcuvdrjw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3obxnslpu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3knrqnhaq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wsqhnpty.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zvrrvhxx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ixprdexj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3itwhppzy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mpdctcnm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vhkdktkg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3olhlxfmc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rvuvlnum.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mphxupsg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3pctaxyvh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fdgqexwd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3pxeudtga.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3uqepvxcr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rebmjszu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xevyxtck.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qsqxninm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tzjynvzb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jhjzlwvm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bzzhphae.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vjpctmur.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3grljsffg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kjbtlljn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fohbblan.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wudpfzvg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3frkslces.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rnxnfvxp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hvgluasf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsfxbesu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpouiryj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rjzbpilk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fmkopyxo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ljqijtjv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hrqqiomw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fnjuzwce.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nneakqmw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rucoxuvx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jpklsrll.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ngmeubfw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3apahpqyg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uvwmwzul.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vmhlwlsa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tnopwowa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xpmdjxee.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dhpobvmt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oybnvmqu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hypqaycz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ofpgjmuk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3duiztbrk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xiheqsuj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3yrjtshqv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jicexqee.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mqckivue.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zasbshnd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3niynsadu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3egvzhrfc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jtusljlm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3augpmqwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzxryedb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bvorozsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxyxobfn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3oyupidzg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3anhmzizq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3snflptes.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ywtvcwac.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nklozdvl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eaqvbbyj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rtgfvqfj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ovwbjxdx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmucbeg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ffqfndhs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yarbqcxu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3goytlgwr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3exmslxdd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vtilzugg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ftxiqtia.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vllxrjsc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rgnhbhye.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dmtbfqkz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3lmjgtqan.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xanjmdrc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wtphzkuq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wcnaidpl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ywpfeufo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wjyyxsmn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3aknjyxux.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3icwnbtkt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3anerhwcp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3yvgvebby.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukfzbdij.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpowxywz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hpegepuy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ccwoiljb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3omtmeehc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3miojvama.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmtfetqb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yhyjnbzs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3uxznmfzk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3soyyntix.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuynrwsx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nrmojbhb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkxqrywe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pmasvyix.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mysccoey.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dztamomw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ojitpuhf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xmiinyya.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nqshiqoz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqeohzpj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wvibufow.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ftcbcyfk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jdqdnewy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3rtewxbrn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vktsltrk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wrgnuazl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qfbuzyic.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dpgzsiuj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3tzuinkib.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qcvixwry.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nvuhrytu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3sumgjvfq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ndtpfceu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3eezbsmjy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3szrvvnje.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mjeqmggq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gyqrdisy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3oopdqzom.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dvxooddb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bihgufpi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ahbcnvvt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jbglvjed.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vxbjquqb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jqukqchp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3crlqzsoc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3cliogxhp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wcayydkr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hjgjznxz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tbowrgrp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qixudtmr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3aazviwos.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yaidavjv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fzwvhmym.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3tutgaozk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wsmiuxvj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ujhfqkul.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rwkkbsqv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yuqvlqbo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ljbxfxgy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ondfrqpy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ntgcffnh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3csezzzsb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3qjwrzmph.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ujxtecmm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcsxeoaf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pohgsnlt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fegxwdpl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jnnykogm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bgrztjid.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hmhifcud.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uuuzvekt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3smgypfgm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xfzbrcun.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3etkikcge.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cgusyili.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3psfrrmke.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zfkatzlj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vfyvjxzj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iepzyugs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jdxnhptn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abhqkgpr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vrhzdbki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozvmthkw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3itsbhzwg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3stsvtscz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3gtmqujaw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xfkwvxmk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cgskndls.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fvwmwklr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jttmscdq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xfjmmrbg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3klexnjac.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nahzyxnh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kptbnhgi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3llwectrv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mhsnrrap.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nonuyfoc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jzaylrqw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ngpbftqt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ofmaseuk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3zvmxepsh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3dnmiaigm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lrjtomwa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lnmpuenp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3fbgkubra.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pssvrlnb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yhdpmmcd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3hwmrduzt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jichzscv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmlokmlj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ykvkebrn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3sozsbwdk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fmtefgct.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3emmvvxig.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uzaywiln.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3orcywbkh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vnuotnwj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3mzhfbbdr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jcacslpr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3iemdizpv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3enlgfyrq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hjokspox.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jtgptoxo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3skwuoyzy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jfqmyscp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qwfxksrq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kwrlnqcl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jfjuxyaq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3bxkyxvre.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3agwhunge.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3dbvfpwpt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jmrvpuhm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cuutokjj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ttvbrlnz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qowhrgvq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ymzbqkyk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pgfaiaiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlpibrqq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxgcquvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzptvrff.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3idalmdzl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ypufeejm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ytppfyhg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iaphbijf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bqbbcklz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nkozhvif.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3gtfywcsf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qqbtvluf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3nctyhlft.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hsngypjl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jejnxvst.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3slnyelbs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3thhzkqys.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wtuoldve.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ulqjlszt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3panelpzs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3cglmafvy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3deavvixn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3naxdwutg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lrsfjsme.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3tcgibkem.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3leybyhlw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ptkdyscc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lcqvvtwj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ievorvkd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zekiadfc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ndirjjnb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3otjcfaos.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3wkaskkxj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ockqrtkm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bofcaafr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hiphvcgb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ajlxfkyp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3fuyfdwlk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3zaojxmpw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vnyxlter.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jdrkvofw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mvtagpts.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3aekyugrb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qdlybgpd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3crhszepm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3rznyuguf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bcaorrrs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qhlktdho.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xtjlujjv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3thgbriyo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zfbryxuj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mplcaeyk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ngxsckne.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3bfgywjkl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hntextgc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3yahgylml.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3oxeyxzic.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifuuftbm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3tqfkmcod.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3umcjfzgr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zipkragz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gmygsdqb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qsxkovqf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmndrent.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3youipaga.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rolfjpwb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bcwqtlpk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3buzisgom.html


<!-- 参考信息 -->