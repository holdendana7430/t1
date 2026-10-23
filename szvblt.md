代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wbdciilh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fgybxwag.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hkopdafc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3uluumpcg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qftajxqb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lvlacvvp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lwtpjmgd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rritfkpm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3znpjjnmc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tbtjbnbl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3olmkaqub.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pfgvpxkv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hdrinylb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xnnjylmf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3oyhnvahy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fnevacel.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oidlmrct.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3razryevr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jskrssqy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fndapefs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bcpdvrus.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dmvrsxwt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxnjlsks.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hzrapcng.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vkqkyjsz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3snvnijcr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dzktpdkl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kfdsttvc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uciztabg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3pycocghd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pfcatiss.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3flgjtlfn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sodhqpej.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kjdoscsb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mmjvxljk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dmggggql.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3svfleqyt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ijakhfko.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jkocoybq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3xnclejne.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zfhdutbv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3obebmiee.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mqoynnek.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mjszoxgj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xnmnccdi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3auwcrfzx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ljkqtbhq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zoizhiym.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xhgmnqxr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qmihlktw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3esrrrbcb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3meafbaac.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nrxotfim.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3iqctaydd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3rgrlddkm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3coqyhirx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ajtktwoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbhlrxhc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3usuykbby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdprxttc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3luupffaf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fukxdzhg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gjdqertz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vdygwahr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mcgrjtgj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcqonkvr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dfjnueyn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jqaeocjk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozkjtqdq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3pnqsodhz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3crmavexh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3atqqicpu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qgowsazq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3athpgmba.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tgzfkqac.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kmwgaupt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ynofuxpt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hawhmhvh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gvigaaot.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wwkxonwf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3tzzawjlk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ujyhetza.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uadutfam.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pepofout.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3kzpjxlqu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ytidprkw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kqoblxwn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3yvdshdpr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ztoxjnti.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3plpzufni.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lecipayb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3djoxdmjk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ucqaesbo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jwbfdmmy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxethzo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aabzqbbt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3hxzsycir.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ezyobddb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mgdaufjt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3aflzqoyf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3daeznluo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nqjvxtdn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3rhdintet.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mhwswbnv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xqojlowy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mvjslgcs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3alimgspp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ksneeigu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3miimjryp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rjomcwbm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ydsqhghy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bxkttcqe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iyxgknhj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jijabmml.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ykxmrwqt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kdmodshc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3htykkrzx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vkthpccp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3guemtpxs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3phkgpzmq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3uzqnjqeq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jjknhrlr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zlgljcnv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3opviqryn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fhoqisgb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3garhxmfh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mbalzjfh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yvjroizt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bghkfmbj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wsdvjpjc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jonidqgo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wueloumd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zlgnruxk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3sfmdgdry.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gezdawiq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nyorksok.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dncwtjzs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3okahtrep.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ajayhlwl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hgfzxpxq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pyeujpjr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3kclrmwqj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vcsuvjeh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3twgbrwwn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vmxjriqx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ptpjhape.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3eretwcqq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3iqwkwuzp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3yfyynlqx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kikgigvo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xficyqpt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hhoonpie.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cgnnpxpr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3frxfoxig.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cngqoyhi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fpfhgomi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zxhedokn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tlvikliz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yhrnqbxi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xasbdsjs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rkwfyfbx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3akbfznrh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vjlznxqg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xnbopujc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uwcepbmr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3apqcddpj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rjcpnfnl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3huwqpkmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndelthrj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3kuijfpsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcgbrquq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ytliwddr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nxthhctt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uxsmatxj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ibwjflhg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uuwgptjc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jeliewjl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3meztlyeb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rtuylgsg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3uhaefkmy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3lttzkddz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3gmmrzgtc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tzfofrmn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3roowtubv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kglwrrjn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vfqpbrhe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3icjckrhe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tzkdiach.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vzyqrkub.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3bxhhkror.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gumsrvax.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rvvzybip.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ohrjjbai.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wlgxvadd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvzchsja.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3yjsvskrp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3nhgbsycd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3djdwthxu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3aksxdivr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3dlgzjtfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ppmivxws.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3igvujkgp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lgaxeoqg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xuinzkqh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jtancsep.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3mkhqtryy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcdafeeb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qbvbtbmq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cusdnjna.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3trvyzolk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yqdwfcnb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pnapkrom.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3sbmzseio.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3dbtalrxq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fhkkflal.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovcqkahk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ekmqdqiz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3zgkkvgby.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3tpvsjnuh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3woqdgzpt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yseuvbyg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3jysvlpem.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3avylflfu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3czqtbges.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3fbfbnrpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xktbqpue.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ccwhxwvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3neleiwtw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zdbenehe.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3holuounv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3llsgyduc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ldfcbqka.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cuwzdlqv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3smfhouli.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3taqeprrv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ysipbqko.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dgqluhup.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3eixibqtj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xoggimth.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bzppxdyl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kabbmlbq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jswbrwzc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xrbohwpb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3tsnwvraz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ebuxvvih.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3alrczpsz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xkclclsj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ncowwtdr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3tvpifsjh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wjgvempa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sjcqakup.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdvkycb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kmtdslwz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cgnoaprc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vmhzejvs.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zgwzcntw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3vivvvudk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3snuewgyr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3votmhbva.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pcelouxg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ptgnsjwr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjcrhfr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3tljglpee.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mfshmraq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cjtaprqq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zzuffubo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nnycbrtp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3hkzepbeq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hsgbemaq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3etenrjwp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xyutauku.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3idtpxszt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rexzuiir.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3tvtfxkly.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3sqdslned.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wppvgqih.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vzwghdaa.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3phqxtgys.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbapvqvp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3empagvhn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mwwqleba.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3onhjpenr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3owjhreiu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3xxrbggnw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ukuhlxtb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iteqpjof.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rwqaqzer.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzfxijki.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3roeemrhh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3udpnwzpf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ndjmazqv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3lnvhatmd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3arexdbhg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3dllchfzx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3byzafvyy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qlowaray.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wjlzeyzk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3dxetfefs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pqsubgom.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3sxhxsuur.html


<!-- 参考信息 -->