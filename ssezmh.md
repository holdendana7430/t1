代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3obmwfqdh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3fvytcdpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqeciefu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3daurolhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxkupbox.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ewxdhlbw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mvlhicmq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hayiqjrs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3itoljcqo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngefeecm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hbspxcbw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vxzrnkgi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ynzbdmhp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dxbslpoc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mjxoysst.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oytznjci.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zaqbgyal.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ktmqwudj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sgjvxjuk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cjsaznrr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qnjbeqeo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rtytrmsi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tqfyqogw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3owmofwgv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aaodraac.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rqfekftq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fnkmfvun.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jarazhif.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3usyyjlxz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zbtnnicg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3iszkvsme.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3gxxtbypr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nlnqdnye.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cbruzqjp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3lkevvwzm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yocpgjse.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3apazxzls.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qpwhkcxv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3arofebfj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3frmruldz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tdfgajre.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hdphuriv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zggxyanc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3lfuoeblf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jeabwort.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3euhklpgs.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqcobcmy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqvgrbsj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrxixhex.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3kzptmqfe.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vvpqrqyu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mvafnnbe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ipwbbpyf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ujxszdca.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hkwoxzvt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wvdgfrjc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3bzalyrwy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jsuftmqu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mfitjocm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3thnlzyax.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ersaitsm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zfdztivc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tnuwhsma.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ewgyzxkm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zajjasoy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3glebkuff.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3hujfmnyn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uujulzyz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wzuciblp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wweecffe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gdzosmef.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vdiojfbx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tvvkhgkb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gcajesmg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3trnokirh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3fzopckum.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mtonybrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upxtrjnt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lgbfvjak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgxxenmt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ihbqhkqs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gippavpm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rtnvmzka.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mzywowhu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cbyvwdzz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yregwzuv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pupyjako.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kxbjubdi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ulxpnrdi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qwppblrl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dhgzyrmm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3onlshuyp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xeqomflw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3aifpcvyh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gpxqcpez.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sbqmwjbv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3arbcnpty.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gtnarvsl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3tfsleodd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3atyukayu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3thqzmwsr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bvvggjup.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kpqocrja.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gzksebqj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3einefqcz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wmaltkgf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rfgalqte.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rznfsjiy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnktmdis.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lemvgjpe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wwwwjplu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rcuhalxg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwuhtcuz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wowmmrfn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dovzmeae.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bvrvfhvn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3llzbzlpg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vwcdvlev.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3styxgrek.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmzpkdvz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ysmamcdg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3cuwbivyy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ywgyvffr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vpqktfuu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgezddmo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cnodpqir.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ghhikngx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yvcfvopy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3goxcxwbg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gbfxahls.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wjvaupps.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ipdvwmhv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bbaixual.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fbrujzzw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kwxbfjkh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3oaqarlbc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bfopvyln.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gobtuhff.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rvtkurky.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vfioamdl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3owosbzox.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wydfguls.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3uttheild.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qvvnrxvt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3epitqsvs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dycupnlf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gmmdlxxg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zswpufqz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bbwtdaur.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3whlklqlj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xtgkvfbz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nxhgjnzu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wynptdle.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gxegkkhj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xefcrevx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lgsjoglw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nagnebre.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bpkkadyd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3rybrunrt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3euulbihx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ccplcqfl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3pmqkoqjp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wkvtxrzt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cafbuksy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zklbpdjn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kugvaudh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3bqngqrtg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3iwprzfum.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3fzvowwpi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rvjazauk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nwyrdzov.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3shpdppiy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3svomadzg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qzyerisk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bxrblfku.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3doawfhcn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wtgxemuk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3sbttahqa.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ybbytuwi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3grvnkfkn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mmjzrwwo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nlwshxla.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bxhfbsuc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jcsygchv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bpwrjqvi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kqmfjuac.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3royzjsgx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vtiowjqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmaxpqpx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3affaqpew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewxrfniq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jgrveugw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qztoqjua.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vlokqqhp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ouavggme.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tfzskwyb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hgmrqqvx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3niwmmaum.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3trtmgqox.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ejqzrboe.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3isqtxilh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3eyiipvlc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3umyebmrn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3smevyvib.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xtqmoxgw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pbnafoxu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lkvlkdxr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ezqjndwu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3edhqktcz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zopbmtpc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xdgtkbbf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ipleqtex.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zsvhtuoh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rldbwzcn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgtehnsm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wwkpvyif.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kblnjfkm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mauoxcsp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3zogsnaqs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ksjpyyks.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pzazovic.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pgqhljmw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xtapderl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3aqlvzgzj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jueolohh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xtsopxyx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubmrgzgg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vocvtctw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3peqnazlx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3tvqvzggd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pljwwlqa.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3soxmjdfe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fehniewl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jalgotmq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pitfqmzg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3qxitcmkm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3aqrvjmub.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3plpbikww.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3djhueium.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tzmjemoi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qtbvdvku.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vmddkqma.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3cvebvnfp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yamuxbwy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nizvcrys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezlndizg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rdwurqnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fowdzccb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jrzvsisb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rpopfaqa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3anlisyjs.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lynrjvuq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nwxwdwmu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3qmukvwfk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3cmhiwxxu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iakoubmd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3orryblcr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ymwionwl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nyfrsbpw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzjipzbv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jeaidgry.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ctqodyed.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uxpkpafq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3immmfaqt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qbhgwpii.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3blnlgccu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ymycqeca.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3cefmcnvc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3emtbkgiz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3spjpfdss.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fjeiyaua.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3eqmqztwh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vjuqnwpd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zmhdcvxl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3gagqzyqw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gxpztyxv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3acaejbap.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dnphebul.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3obhhfllv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3paprgqoa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mkrgbgzv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3eywezjat.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3optukqjd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3litltjjf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3nxxlxrnk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cjlkhhyt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3klgfnxae.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3lhdfhhwq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lhgpkqtv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xxiihdse.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ycdxjasr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3igrbrbtc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3qholioet.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pyevdpfe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jsqkhjgg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xnfikroo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ictxtwyf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ichjlguw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3efegcuhi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyoklpxh.html


<!-- 参考信息 -->