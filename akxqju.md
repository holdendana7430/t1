代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yiohbjgu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nxnqlcpd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3grawkbtl.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bnvbcmrb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hpfqusam.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3stahnsuw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dprwlpnn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3oembqoan.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xxstibfc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fpjchmmw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pbiezlmv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3euielnhy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3juwdfkss.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ujexpaob.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vbfktpax.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3uzejlzyx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3yhypwxbn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qcftlurk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3mgcgswvm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eogzmaxe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3okxplqjw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ejufhcli.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vhopdxhm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zvqtorvd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ghgipkmt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3mahhhgam.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pxlsltwp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3womriyrf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncjrmkde.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjtsjxdk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ankgqtpj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmdobff.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zvzsszje.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tikqjebp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3badfwoxu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3potnpkbh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iprqditn.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3okvbqedd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3splmjgui.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iqnsncai.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3bwfwhzwp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3raxgwlqn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hgcjvpqz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3baolanif.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3znutuqvr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ugetkihx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3likwsvhn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ffchcmkh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmjapbx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dnrxgkjd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3trixdpac.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ycghfwrm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xtgvbqpn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3gahpzaha.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dkqmvoyh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zdfdiszh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gsldhalv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dhczldef.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mtrvmesz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ipgnmhqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rmfephry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ignyrcgv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ikqrthmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmdnjdrk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3btsjwocb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdqfrltb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gsumuvdu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pqsvldbk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3saakhwrz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zckvftud.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3swtyuqvn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3smogljei.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkoxcdyv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3vjxqfekp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nuzkqcvo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ysrpwxow.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3acilpqjz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ynrllnyp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wyfproti.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hnxrdzeq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zyfbsgwk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qnphtcbb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3dhwrjhtt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3mudoodud.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rmwpsnkd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jrhbdaro.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mwcgatix.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3yrpnrqth.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3koadsaiv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3oliizcgz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xsqmjrxu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bnicopdk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ytrpnmag.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3onlwhfjd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sszfcuij.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3otctocns.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3laeasxhn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3iiqogbjc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sckyvpwh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3whayrvsd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vjmbrssg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dijjfiql.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoqleqak.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkeoaxxf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yfttfdza.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qfqgheru.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3voejocoz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yolvoglm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptzpamfn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3krwzlfan.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rscxvbar.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zceztbdb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ykybdqxo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dsnivdtt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3isvkbygc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lrkupkbt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pbgsdrob.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3capnhaxk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3mtksqnpa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3vucgnhdz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3nsfztedy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kafflhdf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dypprrhz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xtyfdvqn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ujmxfquu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fqydggal.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zldgydit.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qjgudkzu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjfbqnc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3nkwcomji.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xcbcnmlk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3drklhddx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3esomkywd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pjynmdbt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3opblprak.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wcbqdqde.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ugkyhduo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ptzsdllw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3civtddnx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3phxdaios.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3shrlunvf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gaudfeec.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3apaogerb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3inkhdqvl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nmtclofe.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3llihakil.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ffalxpsk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ksdbbjky.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3btusuevi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cbevbtii.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3roelppmn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3isboeevf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mhlreaye.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nprjizeb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jeutoukb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3lcpammty.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qslhsbwn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gjtxhlbp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bnmiudxj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mzibhfew.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ivvonvlm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3sbgeisaz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hpfdlozs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3cumisfhz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gqpbspoi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hzusdfmk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lsopihtn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kdkhdjbx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3amsltnzk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3spdiklgw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3cuugcbgq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ltvhadfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyevamcm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3cirkgaks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwttmefn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fgyvicfz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lfmrggpx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3saihubdc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3famkvhgp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rwiqupug.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3fgcpjyrj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3glfqznbi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dikdzflw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vejkaonx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nvsxbucu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ludroyna.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xwelfhoa.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dvmdnyfy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3agoivsam.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3tnjvxhmv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3rcxrljkn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nbaqwcuc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ngyseiua.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pohlculr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kqvcfovl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3diqiojkz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cumpskjh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jasfxlik.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjjqvgqm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3oijdcodf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jdngjogo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgochizj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3frucqfgg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kwkdugdp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yfmzhllx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcdtbtue.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xcbdirtn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3sckgnhht.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3csfzkvuz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nzzfktfg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpsfonpt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qncfyjdh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3pqeiijih.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ajsdkjpo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zqnbdiqd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hxarcebr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ppwbuogc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ykqknyby.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3duzodbkw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xuxgqfga.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3znnpwefw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ntvthtbo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3cekfgcze.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cbcwoyzg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3irnmykfw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fqmolzaf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3kwpnrkiu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3smftkwsk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ffbybovc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rllrdgur.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3cztcrhcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exszhasv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nkngyfhk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rhgnryyn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3opvulnoa.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ytpftlot.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nbgleglr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wchwzxlm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wjggaflf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wquqmpss.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3prauycji.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rdrkghhf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3fbycjzek.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ylpeginx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hhkajbkr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qndznupz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lvhqknan.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3yhdxgtcg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nrubsaba.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lohrzbho.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lajmnrdn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3cvszclnr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zprlegeh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3igfbtiyh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3izocssng.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcjnrrn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3lvghjhyg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3krsujbxz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3izgmiilt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wjpgthdp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3igqiembw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3olrvvgwj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3whvllvmg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mtqhipsk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qnwqgxxb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3flecjbyj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gqtrbwqs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vlfsuvup.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vgkwwbda.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3lgqzolen.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3guvazueu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3axnupiqi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3digkzhjo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3evdnrlci.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tvqzfacx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xqxqqaqy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xyabfine.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mfzfjcbx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3oikxznlv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qeupfgom.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3hdtggjdk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpaawsoh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbpwojdl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzcoumyw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ztodouqb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcziscpa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ljrkracm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3pasejdrw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kwjzykwg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lbpslhzn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dtfxpjud.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3tleebaxp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3oqobazwg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3rqblbszk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jrocvzua.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qakvnqjn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3swvgjynt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3waphdemm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3eqvfqazm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kvawkggf.html


<!-- 参考信息 -->