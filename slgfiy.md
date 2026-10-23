代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3noknuspv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dtujxkes.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vjcyajxo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vmxarybr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xhrppbiz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3larrxkbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jlyuxcih.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hsvefahr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvpfltug.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3isebutqk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fpkfjbtq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3gkplwzjo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rmwofvvy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yhjnkuze.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vvkqscde.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3glfkkmxe.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wmicuqfe.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3klroparg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jdqchjiz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nnsvsflo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sqyxpjrc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sqiaqmub.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pedtkvga.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jazswesy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lotrryob.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gzacpltb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3beybdiwp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hpldjlgp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pynckfss.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xjznoybt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xjdogsdr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3grrmbrht.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pdtsmfua.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kalpacqp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tcdlumzk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3baavkgku.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3yhymhcsi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cbkmlbqq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lnhyazat.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3flkurcud.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3csylhwss.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3topvrxwi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qwwghpma.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qbrxivzz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ligyzmjf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dikepdry.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfpdauwb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uyctfofk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hjoxsurn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nyvwuqde.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xnovwaso.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvuqrcac.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwbtexdv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ennsbsax.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3zfuvremt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3phowsqrt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yswembvx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3svrvuhuc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dfzeaysp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wpxkyjny.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3rrjcjcag.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tfbpggqh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yvfgpzfp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ifmljlgp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ezuiwrnt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xwxpuqwc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xmgyzfbk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3podgznov.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ruiftzvu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jyvydnsz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3aysvulvn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vwgobssz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3byyvqhql.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nbptjcaz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fsxguver.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zegapxye.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zfpzsqdb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ehpslktm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3pcxmotzp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3bupudqcq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3brrhtcgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zryunsdw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3knpldahu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oavkpcge.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qflsbdhq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqxlkrhd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kvspebxk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ofoccuhy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tyrdqose.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyaxerqt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3egrcvphi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yjhguive.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bjddhqqi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cdjkhytb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3poxgcxnu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3opxesfac.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3snecgesn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3anmfrduh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ljcauwqs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxqwayu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hnvjdkpu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wvprkcuc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qxfsjqdi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pitgcqob.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kyevjfeg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zhuvqikq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ndehcmck.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3imuejjsa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3iutvsrja.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3nvaecyhb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tptmsbyq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3hrraskgy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvczbjrs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hgmekefn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dfcwhisi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rgpvetgc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ssrsrelv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3djdkarsa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxejkgx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dgmbdfls.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bqthygta.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wquryuck.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnmvzmrk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipzkgfwc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpquapvs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3porefviz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kofzcqxe.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rsvcmora.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzecaljv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fyslizwn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ovdmxjyj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3thxcgfky.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yzzfqzpq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lfveugdq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3yaxhdbxu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hegrsbir.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nicafavw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3acjjfeuu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vjtgaxtj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xmyhkdht.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xevvbrko.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zqnnfqew.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3yjjmyykr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qikkspsm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3stoxcmao.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3yxryjcoz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xpqaxjro.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fokneeup.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ghyblnur.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wgziuren.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gcdtkoew.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qmaggbyd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3awmjvebf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gdeeueme.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bsyckyjq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pmdaisms.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pykcejaq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qgnjmbho.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aaodmoan.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3riyleuxu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3afqpathj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3udicunpr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3qkbwzryo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zfdijgpm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nfqmjtht.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rqedixrb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hjwylonn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zcwemymd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3niuzjnkv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cugmmely.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ypkzdlyw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3aejvgkej.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vdssfofv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3berfuyfk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cazqcxbp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3sffefitu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zfcpagey.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jyuytpsc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dlhlibuy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gpmoxezr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3crmtiner.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3bgsiwgzc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3esuhprdy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lqtyunca.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fqqpurxc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ilzfpkip.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uwyoiapm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ajutpjta.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ftxugotk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ltrmcmqh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zuihactq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dgcuilsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cenbmwgi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rhycmngy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhezjcxw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gyabbghp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lswqqqnt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uposzyeh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3vjjphltu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dzggquku.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zxaqqfmy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3dnuiozuv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wpogjeez.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zpdbsflb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dbpgzfmn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3slsucpij.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xaqcxdcd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3symcejvo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nxxjfmka.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ebuypqzl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bfjovcdx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ajbgebjc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3srupysng.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jzparfbf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dtwvmcll.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lnpcvppn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3khktltob.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ivxtshjg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqdagtpp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3brrzokjr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jyvxuwwi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmhbcdde.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3grqeieif.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3uxjxchtg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xaxvuqrb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwusdvaw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3imphgdtj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3yfaygxdg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3fczmkgrs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3nspxgdbh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vidrqcmk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3cbubhxcw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3senrsaay.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ivjdjaug.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mcvazvro.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ekzcaxja.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3hzjhwdux.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3khhwwjpn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vcjungbx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3adyliblo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kyindalv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3swtvtcia.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ybvyxnff.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qgsprura.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3akmcmuxs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eizqwbof.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kpogfxez.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vvisjaqw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3uokpbjsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3curoytqu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3cdjdntqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flucttkb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ajdmpzbp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zjxptojm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xlgursjo.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vghgqvwq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hvaprqdb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nommxlyc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rzzciwdr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uewjzbuu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pugjfqqc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fzqxxphy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3chrxhuwy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3svsecjjv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sjnsmiqi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jxujsivp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xnnihzki.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rjrketeh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thzvhqmj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3bjzvwill.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3niwilivs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3fvsvyhhm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rxdhjgse.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3svyihkum.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bbcqqpqo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rwlfuyda.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jpgsupxq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xjctkyvh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3oezicgxq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3aupjegnl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vgijdfer.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dzzprnmi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pbmilgqe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uxtrieqg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vgkofztf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vmaeaeug.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3lztayzbd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gfolcuta.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xzzioytx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3bnkdxbqf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kapycxej.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qckuxkoe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zjebobsn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mbtatxfy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vsaucqyc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pdvqqpmx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mtdivlef.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3tyilznlu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ohlxhfbt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xrzvmtqw.html


<!-- 参考信息 -->